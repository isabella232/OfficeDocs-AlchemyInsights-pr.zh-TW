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
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731230"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="4f038-102">使用 Intune 啟用 Bitlocker 加密</span><span class="sxs-lookup"><span data-stu-id="4f038-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="4f038-103">Intune Endpoint Protection 原則可用於設定 Windows 裝置的 Bitlocker 加密設定。</span><span class="sxs-lookup"><span data-stu-id="4f038-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="4f038-104">如需詳細資訊，請參閱 [Windows 10 (和更新版本) 設定，以使用 Intune 保護裝置](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption)。</span><span class="sxs-lookup"><span data-stu-id="4f038-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="4f038-105">您應注意，許多執行 Windows 10 的更新裝置都支援自動 Bitlocker 加密，而不是在應用 MDM 原則的情況下觸發。</span><span class="sxs-lookup"><span data-stu-id="4f038-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="4f038-106">如果已設定非預設設定，這可能會影響原則的應用程式。</span><span class="sxs-lookup"><span data-stu-id="4f038-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="4f038-107">如需詳細資訊，請參閱下列 FAQ。</span><span class="sxs-lookup"><span data-stu-id="4f038-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="4f038-108">如需有關 bitlocker 問題疑難排解的詳細資訊，請參閱 [疑難排解 Microsoft Intune 中的 BitLocker 原則](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies)。</span><span class="sxs-lookup"><span data-stu-id="4f038-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="4f038-109">**常見問題集**</span><span class="sxs-lookup"><span data-stu-id="4f038-109">**FAQ**</span></span>

 <span data-ttu-id="4f038-110">問：哪些版本的 Windows 支援使用 Endpoint Protection 原則裝置加密？</span><span class="sxs-lookup"><span data-stu-id="4f038-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="4f038-111">A： Intune Endpoint Protection 原則中的設定是使用 [BITLOCKER CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp)來執行。</span><span class="sxs-lookup"><span data-stu-id="4f038-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="4f038-112">並非所有版本或 Windows 組建都支援 Bitlocker CSP。</span><span class="sxs-lookup"><span data-stu-id="4f038-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="4f038-113">目前支援下列 Windows 版本： Enterprise、教育版、行動裝置、行動企業及職業 (組建1809和更新版本) 。</span><span class="sxs-lookup"><span data-stu-id="4f038-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="4f038-114">Q：如果裝置已使用 Bitlocker 加密方法和密碼長度) AES-128 (預設值的 OS 預設設定來加密，將會以新的設定套用具有不同設定的原則，以自動對該磁片磁碟機重新加密。</span><span class="sxs-lookup"><span data-stu-id="4f038-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="4f038-115">答：否。</span><span class="sxs-lookup"><span data-stu-id="4f038-115">A: No.</span></span> <span data-ttu-id="4f038-116">若要套用新的密碼設定，必須先解密磁片磁碟機。</span><span class="sxs-lookup"><span data-stu-id="4f038-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="4f038-117">**附注：** 針對使用 Autopilot 註冊的裝置，在進行 OOBE 原則評估之前，不會觸發在 OOBE 期間進行的自動加密，這可讓您使用原則設定來取代 OS 預設值。</span><span class="sxs-lookup"><span data-stu-id="4f038-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="4f038-118">Q：如果設備因 Intune 原則的應用而加密，將會在移除該原則時進行解密？</span><span class="sxs-lookup"><span data-stu-id="4f038-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="4f038-119">A：移除加密相關原則不會導致解密已設定的磁片磁碟機。</span><span class="sxs-lookup"><span data-stu-id="4f038-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="4f038-120">問：為什麼 Intune 符合性原則會顯示我的裝置沒有啟用 Bitlocker，即使是？</span><span class="sxs-lookup"><span data-stu-id="4f038-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="4f038-121">A： Intune 相容性原則中的「Bitlocker enabled」設定會利用 Windows 裝置健康情況證明 (DHA) 用戶端。</span><span class="sxs-lookup"><span data-stu-id="4f038-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="4f038-122">此用戶端只會在啟動時測量裝置狀態。</span><span class="sxs-lookup"><span data-stu-id="4f038-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="4f038-123">因此，如果在 Bitlocker 加密完成後裝置尚未重新開機，則 DHA 用戶端服務不會將 Bitlocker 報告為作用中。</span><span class="sxs-lookup"><span data-stu-id="4f038-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 