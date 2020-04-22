---
title: SharePoint 線上術語存放區中遺失的字詞
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 54ac2dbc1f45f88541c2338f3b55a777b4b57123
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766844"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="cd65b-102">使用 Intune 啟用 Bitlocker 加密</span><span class="sxs-lookup"><span data-stu-id="cd65b-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="cd65b-103">Intune Endpoint Protection 原則可用於設定 Windows 裝置的 Boitlocker 加密設定，如： Windows10 （及更新版本）設定中所述，以使用 Intune 保護裝置</span><span class="sxs-lookup"><span data-stu-id="cd65b-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="cd65b-104">您應注意，許多執行 Windows 10 的更新裝置都支援自動 bitlocker 加密，而不是在應用 MDM 原則的情況下觸發。</span><span class="sxs-lookup"><span data-stu-id="cd65b-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="cd65b-105">如果未設定預設設定，這可能會影響原則的應用程式。</span><span class="sxs-lookup"><span data-stu-id="cd65b-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="cd65b-106">如需詳細資訊，請參閱 FAQ。</span><span class="sxs-lookup"><span data-stu-id="cd65b-106">See FAQ for more detail.</span></span>


<span data-ttu-id="cd65b-107">FAQ  Q：哪些版本的 Windows 支援使用 Endpoint Protection 原則的裝置加密？</span><span class="sxs-lookup"><span data-stu-id="cd65b-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="cd65b-108"> A： Intune Endpoint Protection 原則中的設定是使用 Bitlocker CSP 來執行。</span><span class="sxs-lookup"><span data-stu-id="cd65b-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="cd65b-109">並非所有的版本和 Windows 內部版本都支援 Bitlocker CSP。 
     </span><span class="sxs-lookup"><span data-stu-id="cd65b-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="cd65b-110">在此時間，Windows 版本： Enterprise;支援教育版、行動裝置、行動企業版及專業版（從組建1809向上）。</span><span class="sxs-lookup"><span data-stu-id="cd65b-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="cd65b-111">Q：如果裝置已使用 Bitlocker 加密方法和密碼長度（AES-128 XTS）的 OS 預設設定來使用 Bitlocker 加密，將會以新的設定套用具有不同設定的原則，以自動對該磁片磁碟機重新加密。</span><span class="sxs-lookup"><span data-stu-id="cd65b-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="cd65b-112">答：否。</span><span class="sxs-lookup"><span data-stu-id="cd65b-112">A: No.</span></span> <span data-ttu-id="cd65b-113">為了套用新的密碼設定，必須先解密磁片磁碟機。</span><span class="sxs-lookup"><span data-stu-id="cd65b-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="cd65b-114">附注：針對使用 Autopilot 註冊的裝置，將不會觸發在 OOBE 期間進行的自動加密，除非已評估 Intune 原則，才能使用原則設定來取代 OS 預設值</span><span class="sxs-lookup"><span data-stu-id="cd65b-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="cd65b-115">Q：如果裝置因 Intune 原則的應用而加密，將會在移除該原則時進行解密？</span><span class="sxs-lookup"><span data-stu-id="cd65b-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="cd65b-116">A：移除加密相關原則不會導致解密已設定的磁片磁碟機。</span><span class="sxs-lookup"><span data-stu-id="cd65b-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="cd65b-117">問：為什麼 intune 符合性原則會顯示我的裝置沒有「啟用 Bitlocker」，但它是？</span><span class="sxs-lookup"><span data-stu-id="cd65b-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="cd65b-118">A： intune 相容性原則中的「Bitlocker enabled」設定會利用 Windows 裝置健康情況證明（DHA）用戶端。</span><span class="sxs-lookup"><span data-stu-id="cd65b-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="cd65b-119">此用戶端只會在啟動時測量裝置狀態。</span><span class="sxs-lookup"><span data-stu-id="cd65b-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="cd65b-120">因此，如果在 bitlocker 加密完成後裝置尚未重新開機，則 DHA 用戶端服務不會將 bitlocker 報告為作用中。</span><span class="sxs-lookup"><span data-stu-id="cd65b-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>