---
title: 設定 Microsoft Defender ATP 掃描的排除
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
- "6027"
- "9001464"
ms.openlocfilehash: 5eb18f4133aca93c1506f4975c8d0567bede8d57
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543676"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="2c51e-102">設定 Microsoft Defender ATP 掃描的排除</span><span class="sxs-lookup"><span data-stu-id="2c51e-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="2c51e-103">一般來說，您可以從 Microsoft Defender ATP 掃描排除特定的檔案副檔名和資料夾位置。</span><span class="sxs-lookup"><span data-stu-id="2c51e-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="2c51e-104">您也可以為由特定程序開啟的檔案設定排除。</span><span class="sxs-lookup"><span data-stu-id="2c51e-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="2c51e-105">如需詳細資訊，請參閱[設定及驗證基於檔案副檔名和資料夾位置的排除](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus)和[為由程序開啟的檔案設定排除](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)。</span><span class="sxs-lookup"><span data-stu-id="2c51e-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="2c51e-106">若要為 **Windows Server 2016 和 2019** 設定排除，請參閱 [在 Windows Server 上設定 Microsoft Defender 防毒軟體排除](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)。</span><span class="sxs-lookup"><span data-stu-id="2c51e-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="2c51e-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="2c51e-107">**Mac**</span></span>

<span data-ttu-id="2c51e-108">如需支援的排除類型和為 Mac 設定排除清單的詳細資料，請參閱[支援的排除類型](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)和[如何設定排除清單](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)。</span><span class="sxs-lookup"><span data-stu-id="2c51e-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="2c51e-109">**附註**：您也可以使用 EICAR 測試檔案來驗證排除清單。</span><span class="sxs-lookup"><span data-stu-id="2c51e-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="2c51e-110">如需詳細資訊，請參閱[使用 EICAR 測試檔案驗證排除清單](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)。</span><span class="sxs-lookup"><span data-stu-id="2c51e-110">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="2c51e-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="2c51e-111">**Linux**</span></span>

<span data-ttu-id="2c51e-112">如需支援的排除類型和為 Linux 設定排除清單的詳細資料，請參閱[支援的排除類型](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)和[設定及驗證適用於 Linux 的 Microsoft Defender ATP 排除](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)。</span><span class="sxs-lookup"><span data-stu-id="2c51e-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="2c51e-113">**附註**：您也可以使用 EICAR 測試檔案來驗證排除清單。</span><span class="sxs-lookup"><span data-stu-id="2c51e-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="2c51e-114">如需詳細資訊，請參閱[使用 EICAR 測試檔案驗證排除清單](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)。</span><span class="sxs-lookup"><span data-stu-id="2c51e-114">For more info, see [Validate exclusions lists with the EICAR test file](/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 