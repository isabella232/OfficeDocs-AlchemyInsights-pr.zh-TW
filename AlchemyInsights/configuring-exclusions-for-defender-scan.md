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
ms.openlocfilehash: 912e77b9b1a149fef373f2d0814fb2f0671a48c6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "49768403"
---
# <a name="configuring-exclusions-for-microsoft-defender-atp-scan"></a><span data-ttu-id="15fff-102">設定 Microsoft Defender ATP 掃描的排除</span><span class="sxs-lookup"><span data-stu-id="15fff-102">Configuring exclusions for Microsoft Defender ATP scan</span></span>

<span data-ttu-id="15fff-103">一般來說，您可以從 Microsoft Defender ATP 掃描排除特定的檔案副檔名和資料夾位置。</span><span class="sxs-lookup"><span data-stu-id="15fff-103">In general, you can exclude certain file extensions and folder locations from Microsoft Defender ATP scans.</span></span> <span data-ttu-id="15fff-104">您也可以為由特定程序開啟的檔案設定排除。</span><span class="sxs-lookup"><span data-stu-id="15fff-104">You can also configure exclusions for files opened by certain processes.</span></span> <span data-ttu-id="15fff-105">如需詳細資訊，請參閱[設定及驗證基於檔案副檔名和資料夾位置的排除](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus)和[為由程序開啟的檔案設定排除](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus)。</span><span class="sxs-lookup"><span data-stu-id="15fff-105">For more info, see, [Configure and validate exclusions based on file extension and folder location](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-extension-file-exclusions-microsoft-defender-antivirus) and [Configure exclusions for files opened by processes](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-process-opened-file-exclusions-microsoft-defender-antivirus) .</span></span>

<span data-ttu-id="15fff-106">若要為 **Windows Server 2016 和 2019** 設定排除，請參閱[在 Windows Server 上設定 Microsoft Defender 防毒軟體排除](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus)。</span><span class="sxs-lookup"><span data-stu-id="15fff-106">To configure exclusions for  **Windows Server 2016 and 2019**, see [Configure Microsoft Defender Antivirus exclusions on Windows Server](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-antivirus/configure-server-exclusions-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="15fff-107">**Mac**</span><span class="sxs-lookup"><span data-stu-id="15fff-107">**Mac**</span></span>

<span data-ttu-id="15fff-108">如需支援的排除類型和為 Mac 設定排除清單的詳細資料，請參閱[支援的排除類型](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types)和[如何設定排除清單](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions)。</span><span class="sxs-lookup"><span data-stu-id="15fff-108">For details on supported exclusion types and configuring a list of exclusions for Mac, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#supported-exclusion-types) and [How to configure the list of exclusions](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#how-to-configure-the-list-of-exclusions).</span></span>

<span data-ttu-id="15fff-109">**附註**：您也可以使用 EICAR 測試檔案來驗證排除清單。</span><span class="sxs-lookup"><span data-stu-id="15fff-109">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="15fff-110">如需詳細資訊，請參閱[使用 EICAR 測試檔案驗證排除清單](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file)。</span><span class="sxs-lookup"><span data-stu-id="15fff-110">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/mac-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 

<span data-ttu-id="15fff-111">**Linux**</span><span class="sxs-lookup"><span data-stu-id="15fff-111">**Linux**</span></span>

<span data-ttu-id="15fff-112">如需支援的排除類型和為 Linux 設定排除清單的詳細資料，請參閱[支援的排除類型](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types)和[設定及驗證適用於 Linux 的 Microsoft Defender ATP 排除](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions)。</span><span class="sxs-lookup"><span data-stu-id="15fff-112">For details on supported exclusion types and configuring a list of exclusions for Linux, see [Supported exclusion types](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#supported-exclusion-types) and [Configure and validate exclusions for Microsoft Defender ATP for Linux](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions).</span></span>

<span data-ttu-id="15fff-113">**附註**：您也可以使用 EICAR 測試檔案來驗證排除清單。</span><span class="sxs-lookup"><span data-stu-id="15fff-113">**Note** You can also validate exclusions lists using the EICAR test file.</span></span> <span data-ttu-id="15fff-114">如需詳細資訊，請參閱[使用 EICAR 測試檔案驗證排除清單](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file)。</span><span class="sxs-lookup"><span data-stu-id="15fff-114">For more info, see [Validate exclusions lists with the EICAR test file](https://docs.microsoft.com/windows/security/threat-protection/microsoft-defender-atp/linux-exclusions#validate-exclusions-lists-with-the-eicar-test-file).</span></span> 