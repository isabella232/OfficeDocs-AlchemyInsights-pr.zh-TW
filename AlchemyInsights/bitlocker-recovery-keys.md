---
title: Bitlocker 復原機碼
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908806"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="7b6bb-102">存取 Bitlocker 復原機碼</span><span class="sxs-lookup"><span data-stu-id="7b6bb-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="7b6bb-103">當設定 Bitlocker Intune 端點保護原則，就可以定義 Bitlocker 復原資訊是否應該儲存在 Azure Active Directory。</span><span class="sxs-lookup"><span data-stu-id="7b6bb-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="7b6bb-104">如果設定該設定，則預存的復原資料應看見 Intune 裝置] 刀鋒視窗中以兩種方式中的裝置記錄資料的一部分的 Intune 系統管理員：</span><span class="sxs-lookup"><span data-stu-id="7b6bb-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="7b6bb-105">裝置-的 Azure AD 裝置 # A0 「 裝置 」 或裝置-> 所有裝置-> 「 裝置 」-> 復原機碼</span><span class="sxs-lookup"><span data-stu-id="7b6bb-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="7b6bb-106">或者，如果沒有管理存取權，裝置本身，都可以看到復原金鑰 （密碼） 從提升權限的命令提示字元執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="7b6bb-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
<span data-ttu-id="7b6bb-107">如果裝置已加密之前在 Intune 中註冊，復原機碼可能已經與 「 Microsoft 帳戶 」 (MSA) 用來登入裝置 OOBE 程序期間相關聯。</span><span class="sxs-lookup"><span data-stu-id="7b6bb-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="7b6bb-108">如果是這種情況，存取https://onedrive.live.com/recoverykey，並且登入該 MSA 應顯示哪些復原機碼已儲存的裝置。</span><span class="sxs-lookup"><span data-stu-id="7b6bb-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="7b6bb-109">如果裝置已加密因為透過網域型群組原則設定，復原資訊可能會儲存在內部部署 Active Directory。</span><span class="sxs-lookup"><span data-stu-id="7b6bb-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

