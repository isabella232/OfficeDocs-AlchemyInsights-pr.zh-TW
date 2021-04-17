---
title: Bitlocker 修復金鑰
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: ec90e412302c74748e253f2e5430fa4205466f0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820277"
---
# <a name="accessing-bitlocker-recovery-keys"></a><span data-ttu-id="3c303-102">存取 Bitlocker 恢復機碼</span><span class="sxs-lookup"><span data-stu-id="3c303-102">Accessing Bitlocker recovery keys</span></span>

<span data-ttu-id="3c303-103">設定 Bitlocker 設定 Intune Endpoint Protection 原則時，可以定義是否應將 Bitlocker 復原資訊儲存在 Azure Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="3c303-103">When configuring Bitlocker settings Intune Endpoint Protection Policy, it is possible to define whether Bitlocker recovery information should be stored in Azure Active Directory.</span></span>

<span data-ttu-id="3c303-104">如果已設定該設定，則在 Intune 裝置 blade 中，以下列兩種方式將已儲存的復原資料視為裝置記錄資料的一部分，以供 Intune 系統管理員看到：</span><span class="sxs-lookup"><span data-stu-id="3c303-104">If that setting is configured, the stored recovery data should be visible to an Intune admin as part of the device record data in Intune Devices blade in two ways:</span></span>

<span data-ttu-id="3c303-105">裝置-Azure AD 裝置-> "Device" 或 Devices-> 所有裝置-> "Device"-> 復原金鑰</span><span class="sxs-lookup"><span data-stu-id="3c303-105">Devices - Azure AD devices -> "Device"  OR Devices -> All Devices -> "Device" -> Recovery keys</span></span>

<span data-ttu-id="3c303-106">或者，如果有裝置本身的系統管理存取權，可從提升許可權的命令提示字元執行下列命令，以查看復原金鑰 (密碼) ：</span><span class="sxs-lookup"><span data-stu-id="3c303-106">Alternatively, if there is administrative access to the device itself, the recovery key (Password) can be seen by running the following command from an elevated command prompt:</span></span>

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
<span data-ttu-id="3c303-107">若在 Intune 中 enrolment 之前已加密裝置，則復原機碼可能與「Microsoft 帳戶」相關聯 (MSA) ，用來在 OOBE 過程中登入裝置。</span><span class="sxs-lookup"><span data-stu-id="3c303-107">If the device was encrypted prior to enrolment in Intune, the recovery key may have been associated with the "Microsoft Account" (MSA) used to sign in to the device during the OOBE process.</span></span> <span data-ttu-id="3c303-108">如果是這種情況，  https://onedrive.live.com/recoverykey 使用此 MSA 進行存取和登入時，應該會顯示已儲存復原金鑰的裝置。</span><span class="sxs-lookup"><span data-stu-id="3c303-108">If that was the case, accessing  https://onedrive.live.com/recoverykey and signing in with that MSA should show the devices for which recovery keys were stored.</span></span>
 
<span data-ttu-id="3c303-109">如果是透過以網域為基礎的群組原則進行設定的加密裝置，則復原資訊可能會儲存在內部部署 Active Directory 中。</span><span class="sxs-lookup"><span data-stu-id="3c303-109">If the device was encrypted as a result of configuration through domain-based group policy, the recovery information may be stored in the on-premise Active Directory.</span></span>

<span data-ttu-id="3c303-110">如果您已設定 Endpoint protection 原則，將復原金鑰儲存在 Azure Active Directory 中，但尚未上傳特定裝置的金鑰，您可以從 MEM 主控台旋轉該裝置的復原金鑰，以觸發上載。</span><span class="sxs-lookup"><span data-stu-id="3c303-110">If you have configured Endpoint protection policy to store the recovery key in Azure Active Directory but the key for a specific device has not been uploaded, you can trigger the upload by rotating the recovery key for that device from the MEM console.</span></span> <span data-ttu-id="3c303-111">如需詳細資訊，請參閱 [輪替 BitLocker](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)復原機碼。</span><span class="sxs-lookup"><span data-stu-id="3c303-111">For details, see [Rotate BitLocker recovery keys](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys).</span></span>

