---
title: 在 Mac 或 Linux 上安裝 Microsoft Defender 的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 39f180852fd0438597fa1ce665b2703fbc7b1aa4
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52539671"
---
# <a name="issues-installing-microsoft-defender-on-mac-or-linux"></a><span data-ttu-id="68573-102">在 Mac 或 Linux 上安裝 Microsoft Defender 的問題</span><span class="sxs-lookup"><span data-stu-id="68573-102">Issues installing Microsoft Defender on Mac or Linux</span></span>

<span data-ttu-id="68573-103">**Mac**</span><span class="sxs-lookup"><span data-stu-id="68573-103">**Mac**</span></span>

- <span data-ttu-id="68573-104">安裝適用於 Mac 的 Microsoft Defender ATP 之前，請先確保已符合系統需求。</span><span class="sxs-lookup"><span data-stu-id="68573-104">Ensure that system requirements are met before installing Microsoft Defender ATP for Mac.</span></span> <span data-ttu-id="68573-105">如需詳細資訊，請參閱[如何安裝適用於 Mac 的 Microsoft Defender ATP](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac)。</span><span class="sxs-lookup"><span data-stu-id="68573-105">For more info, see [How to install Microsoft Defender ATP for Mac](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-mac#how-to-install-microsoft-defender-atp-for-mac).</span></span>  
- <span data-ttu-id="68573-106">檢閱此檔案中的資訊："/Library/Logs/Microsoft/mdatp/install.log"。</span><span class="sxs-lookup"><span data-stu-id="68573-106">Review the information in the file: "/Library/Logs/Microsoft/mdatp/install.log".</span></span>

<span data-ttu-id="68573-107">**Linux**</span><span class="sxs-lookup"><span data-stu-id="68573-107">**Linux**</span></span>

- <span data-ttu-id="68573-108">安裝適用於 Linux 的 Microsoft Defender ATP 之前，請先確保已符合系統需求。</span><span class="sxs-lookup"><span data-stu-id="68573-108">Ensure that system requirements are met before installing Microsoft Defender ATP for Linux.</span></span> <span data-ttu-id="68573-109">如需詳細資訊，請參閱[如何安裝適用於 Linux 的 MDATP](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。</span><span class="sxs-lookup"><span data-stu-id="68573-109">For more info, see [How to install MDATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span> 
- <span data-ttu-id="68573-110">若要確認 MDATP 服務執行中，請參閱[安裝失敗](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed)。</span><span class="sxs-lookup"><span data-stu-id="68573-110">To verify that MDATP service is running, see [Installation failed](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#installation-failed).</span></span>  
    <span data-ttu-id="68573-111">若要疑難排解並解決服務未執行的問題，請參閱 [mdatp 服務未執行時的疑難排解步驟](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running)。</span><span class="sxs-lookup"><span data-stu-id="68573-111">To troubleshoot and resolve issues if the service is not running, see [Steps to troubleshoot if mdatp service isn't running](/windows/security/threat-protection/microsoft-defender-atp/linux-support-install#steps-to-troubleshoot-if-mdatp-service-isnt-running).</span></span>
- <span data-ttu-id="68573-112">如需檢查用戶端設定 (其會驗證產品的健康情況) 的步驟，以及若要對 EICAR 文字檔案執行偵測測試，請參閱[用戶端設定](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration)。</span><span class="sxs-lookup"><span data-stu-id="68573-112">For steps to check the client configuration, which verifies the health of the product, and to run a detection test on the EICAR text file, see [Client configuration](/windows/security/threat-protection/microsoft-defender-atp/linux-install-manually#client-configuration).</span></span>  

    <span data-ttu-id="68573-113">**附註** 如需即時監視活動支援的檔案系統清單，請參閱 [適用於 Linux 的 Microsoft Defender ATP](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements)。</span><span class="sxs-lookup"><span data-stu-id="68573-113">**Note** For a list of supported file systems for on-access activity, see [Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/microsoft-defender-atp-linux#system-requirements).</span></span>