---
title: DataProtection-Bitlocker
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
- "1802"
- "9000220"
ms.openlocfilehash: 0b305931a7279d8f1085c411cc9b47c991e1ee44
ms.sourcegitcommit: 9c4b4853ff53f21c0177d48821846070bb00637c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/06/2021
ms.locfileid: "49768808"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="e09d6-102">使用 Intune 啟用 Bitlocker 加密</span><span class="sxs-lookup"><span data-stu-id="e09d6-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="e09d6-103">Intune Endpoint Protection 原則可用於設定 Windows 裝置的 Bitlocker 加密設定。</span><span class="sxs-lookup"><span data-stu-id="e09d6-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="e09d6-104">如需詳細資訊，請參閱 [Windows 10 (和更新版本) 設定，以使用 Intune 保護裝置](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)。</span><span class="sxs-lookup"><span data-stu-id="e09d6-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="e09d6-105">您應注意，許多執行 Windows 10 的更新裝置都支援自動 Bitlocker 加密，而不是在應用 MDM 原則的情況下觸發。</span><span class="sxs-lookup"><span data-stu-id="e09d6-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="e09d6-106">如果已設定非預設設定，這可能會影響原則的應用程式。</span><span class="sxs-lookup"><span data-stu-id="e09d6-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="e09d6-107">如需詳細資訊，請參閱下列 FAQ。</span><span class="sxs-lookup"><span data-stu-id="e09d6-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="e09d6-108">如需有關 bitlocker 問題疑難排解的詳細資訊，請參閱 [疑難排解 Microsoft Intune 中的 BitLocker 原則](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)。</span><span class="sxs-lookup"><span data-stu-id="e09d6-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="e09d6-109">**常見問題集**</span><span class="sxs-lookup"><span data-stu-id="e09d6-109">**FAQ**</span></span>

<span data-ttu-id="e09d6-110">問：哪些版本的 Windows 支援使用 Endpoint Protection 原則裝置加密？</span><span class="sxs-lookup"><span data-stu-id="e09d6-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
<span data-ttu-id="e09d6-111">A： Intune Endpoint Protection 原則中的設定是使用 [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)來執行。</span><span class="sxs-lookup"><span data-stu-id="e09d6-111">A: The settings in Intune Endpoint Protection Policy are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="e09d6-112">並非所有版本或 Windows 組建都支援 Bitlocker CSP。</span><span class="sxs-lookup"><span data-stu-id="e09d6-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>

<span data-ttu-id="e09d6-113">問：如何在裝置上啟用 Bitlocker，而不需要使用者進行互動？</span><span class="sxs-lookup"><span data-stu-id="e09d6-113">Q: How can Bitlocker be enabled on devices without requiring end user interaction?</span></span><br>
<span data-ttu-id="e09d6-114">A：只要符合必要先決條件，即可透過 Intune 啟用 Bitlocker 「無訊息的加密」。</span><span class="sxs-lookup"><span data-stu-id="e09d6-114">A: So long as the necessary pre-requisites are met it is possible to enable Bitlocker "Silent Encryption" through Intune.</span></span> <span data-ttu-id="e09d6-115">請參閱裝置需求的詳細資料和範例原則設定，以啟用下列檔中的無訊息加密：以無訊息方式 [啟用 Bitlocker 加密](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices)。</span><span class="sxs-lookup"><span data-stu-id="e09d6-115">See the details of the device requirements and example policy settings to enable silent encryption in the following doc: [Silently Enable Bitlocker Encryption](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#silently-enable-bitlocker-on-devices).</span></span> <br><br>

<span data-ttu-id="e09d6-116">Q：如果裝置已使用 Bitlocker 加密方法和密碼長度) AES-128 (預設值的 OS 預設設定來加密，將會以新的設定套用具有不同設定的原則，以自動對該磁片磁碟機重新加密。</span><span class="sxs-lookup"><span data-stu-id="e09d6-116">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="e09d6-117">答：否。</span><span class="sxs-lookup"><span data-stu-id="e09d6-117">A: No.</span></span> <span data-ttu-id="e09d6-118">若要套用新的密碼設定，必須先解密磁片磁碟機。</span><span class="sxs-lookup"><span data-stu-id="e09d6-118">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="e09d6-119">**附注：** 針對使用 Autopilot 註冊的裝置，在進行 OOBE 原則評估之前，不會觸發在 OOBE 期間進行的自動加密，這可讓您使用原則設定來取代 OS 預設值。</span><span class="sxs-lookup"><span data-stu-id="e09d6-119">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="e09d6-120">Q：如果設備因 Intune 原則的應用而加密，將會在移除該原則時進行解密？</span><span class="sxs-lookup"><span data-stu-id="e09d6-120">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="e09d6-121">A：移除加密相關原則不會導致解密已設定的磁片磁碟機。</span><span class="sxs-lookup"><span data-stu-id="e09d6-121">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="e09d6-122">問：為什麼 Intune 符合性原則會顯示我的裝置沒有啟用 Bitlocker，即使是？</span><span class="sxs-lookup"><span data-stu-id="e09d6-122">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="e09d6-123">A： Intune 相容性原則中的「Bitlocker enabled」設定會利用 Windows 裝置健康情況證明 (DHA) 用戶端。</span><span class="sxs-lookup"><span data-stu-id="e09d6-123">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="e09d6-124">此用戶端只會在啟動時測量裝置狀態。</span><span class="sxs-lookup"><span data-stu-id="e09d6-124">This client only measures device state at boot time.</span></span> <span data-ttu-id="e09d6-125">因此，如果在 Bitlocker 加密完成後裝置尚未重新開機，則 DHA 用戶端服務不會將 Bitlocker 報告為作用中。</span><span class="sxs-lookup"><span data-stu-id="e09d6-125">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 