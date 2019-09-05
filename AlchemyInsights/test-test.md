---
title: 從 SharePoint Online 字詞庫中遺失的字詞
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762043"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="eba2c-102">使用 Intune 啟用 Bitlocker 加密</span><span class="sxs-lookup"><span data-stu-id="eba2c-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="eba2c-103">Intune 端點保護原則可以用來設定 Windows 裝置 Boitlocker 加密設定中所述： Windows10 （及更新版本） 來保護裝置使用 Intune 設定</span><span class="sxs-lookup"><span data-stu-id="eba2c-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="eba2c-104">您應該注意執行 Windows 10 的許多較新裝置支援便 MDM 原則的應用程式不會觸發自動 bitlocker 加密。</span><span class="sxs-lookup"><span data-stu-id="eba2c-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="eba2c-105">如果非預設設定，這可能會影響應用程式的原則。</span><span class="sxs-lookup"><span data-stu-id="eba2c-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="eba2c-106">如需詳細資訊，請參閱常見問題集。</span><span class="sxs-lookup"><span data-stu-id="eba2c-106">See FAQ for more detail.</span></span>


<span data-ttu-id="eba2c-107">常見問題集 問： 哪個版本的 Windows 支援裝置加密使用端點保護原則？</span><span class="sxs-lookup"><span data-stu-id="eba2c-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="eba2c-108"> 答： 使用 Bitlocker CSP 實作在 [Intune 端點保護原則設定。</span><span class="sxs-lookup"><span data-stu-id="eba2c-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="eba2c-109">並非所有版本，也不版的 Windows 都支援 Bitlocker CSP。 
     </span><span class="sxs-lookup"><span data-stu-id="eba2c-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="eba2c-110">在此時間 Windows 版本： 企業;教育版、 行動電話、 行動企業和 Professional （從組建 1809年以前的版本） 支援。</span><span class="sxs-lookup"><span data-stu-id="eba2c-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="eba2c-111">問： 如果裝置已加密使用 Bitlocker 加密方法使用 OS 預設設定，且密碼強度 (XTS-aes-128) 將會套用不同的原則設定會自動觸發重新加密磁碟機使用新的設定嗎？</span><span class="sxs-lookup"><span data-stu-id="eba2c-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="eba2c-112">答：否。</span><span class="sxs-lookup"><span data-stu-id="eba2c-112">A: No.</span></span> <span data-ttu-id="eba2c-113">若要套用新的加密設定的磁碟機必須先解密。</span><span class="sxs-lookup"><span data-stu-id="eba2c-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="eba2c-114">附註對於裝置註冊透過 Autopilot 會自動加密，就會發生期間 OOBE 不會觸發直到評估 Intune 原則可讓原則以設定，使用來取代 OS 預設值</span><span class="sxs-lookup"><span data-stu-id="eba2c-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="eba2c-115">問： 如果裝置加密由於 Intune 原則的應用程式將其解密中移除該原則時嗎？</span><span class="sxs-lookup"><span data-stu-id="eba2c-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="eba2c-116">答： 移除加密的相關原則不會導致解密設定的磁碟機。</span><span class="sxs-lookup"><span data-stu-id="eba2c-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="eba2c-117">問： 為什麼 intune 合規性政策顯示我的裝置不一定 「 啟用 Bitlocker 」，但它是？</span><span class="sxs-lookup"><span data-stu-id="eba2c-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="eba2c-118">答: 「 Bitlocker 啟用 「 在 intune 合規性政策設定使用 Windows 裝置健全狀況證明 (DHA) 用戶端。</span><span class="sxs-lookup"><span data-stu-id="eba2c-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="eba2c-119">此用戶端只會在開機時測量裝置狀態。</span><span class="sxs-lookup"><span data-stu-id="eba2c-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="eba2c-120">讓 bitlocker 加密已完成。 如果裝置有已重新開機自 DHA 用戶端服務不會報告為作用中的 bitlocker。</span><span class="sxs-lookup"><span data-stu-id="eba2c-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>