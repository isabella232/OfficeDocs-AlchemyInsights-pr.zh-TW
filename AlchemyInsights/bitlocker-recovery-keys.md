---
title: Bitlocker 修復金鑰
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685877"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="0f155-102">存取 Bitlocker 恢復機碼</span><span class="sxs-lookup"><span data-stu-id="0f155-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="0f155-103">設定 Bitlocker 設定 Intune Endpoint Protection 原則時，可以定義是否應將 Bitlocker 復原資訊儲存在 Azure Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="0f155-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="0f155-104">如果已設定該設定，則在 Intune 裝置 blade 中，以下列兩種方式將已儲存的復原資料視為裝置記錄資料的一部分，以供 Intune 系統管理員看到：</span><span class="sxs-lookup"><span data-stu-id="0f155-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="0f155-105">裝置-Azure AD 裝置-> "Device" 或 Devices-> 所有裝置-> "Device"-> 復原金鑰</span><span class="sxs-lookup"><span data-stu-id="0f155-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="0f155-106">或者，如果有裝置本身的系統管理存取權，可從提升許可權的命令提示字元執行下列命令，以查看復原金鑰 (密碼) ：</span><span class="sxs-lookup"><span data-stu-id="0f155-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="0f155-107">若在 Intune 中 enrolment 之前已加密裝置，則復原機碼可能與「Microsoft 帳戶」相關聯 (MSA) ，用來在 OOBE 過程中登入裝置。</span><span class="sxs-lookup"><span data-stu-id="0f155-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="0f155-108">如果是這種情況，  https://onedrive.live.com/recoverykey 使用此 MSA 進行存取和登入時，應該會顯示已儲存復原金鑰的裝置。</span><span class="sxs-lookup"><span data-stu-id="0f155-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="0f155-109">如果是透過以網域為基礎的群組原則進行設定的加密裝置，則復原資訊可能會儲存在內部部署 Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="0f155-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>
 

