---
title: Intune Win32 應用程式部署
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: 5ccbf37bd3f06da2f8c3955d87e449ea58caab1c
ms.sourcegitcommit: 9fd002ce49ad9a7e58c3eb997a8063e2e1feab55
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/06/2020
ms.locfileid: "48366505"
---
# <a name="intune-win32-app-deployment"></a><span data-ttu-id="7c541-102">Intune Win32 應用程式部署</span><span class="sxs-lookup"><span data-stu-id="7c541-102">Intune Win32 app deployment</span></span>

<span data-ttu-id="7c541-103">Microsoft Intune 允許在 Windows 10 裝置上部署 Win32 應用程式，包括但不限於MSI和.EXE。</span><span class="sxs-lookup"><span data-stu-id="7c541-103">Microsoft Intune allows Win32 applications, including but not limited to MSI and .EXE’s to be deployed to Windows 10 devices.</span></span> <span data-ttu-id="7c541-104">使用的部署機制要求目標設裝置有 Intune Management Extension (IME)。</span><span class="sxs-lookup"><span data-stu-id="7c541-104">The deployment mechanism used requires the Intune Management Extension (IME) to be present on the target device.</span></span> <span data-ttu-id="7c541-105">由於將 powershell 腳本或 win32 應用程式部署定位到使用者/裝置，將自動安裝 IME。</span><span class="sxs-lookup"><span data-stu-id="7c541-105">The IME will be installed automatically as a result of targeting a powershell script or win32 application deployment to a user / device.</span></span>

<span data-ttu-id="7c541-106">若要部署 Win32 應用程式，還必須符合一組先決條件，其中包括：</span><span class="sxs-lookup"><span data-stu-id="7c541-106">There are also a set of pre-requisites which must be met in order to deploy Win32 apps which include:</span></span>

- <span data-ttu-id="7c541-107">支援的平台：Windows 10 版本1607 或更新版本 (企業版、專業版和教育版)。</span><span class="sxs-lookup"><span data-stu-id="7c541-107">Supported platforms: Windows 10 version 1607 or later (Enterprise, Pro, and Education versions).</span></span>
- <span data-ttu-id="7c541-108">支援的結構： x86 和 x64。</span><span class="sxs-lookup"><span data-stu-id="7c541-108">Supported architecture: x86 and x64.</span></span>
- <span data-ttu-id="7c541-109">裝置管理： 已加入和自動註冊 AAD (包括加入混合式網域和自動註冊群組原則)。</span><span class="sxs-lookup"><span data-stu-id="7c541-109">Device Management: AAD joined and auto-enrolled (including hybrid domain joined and group policy auto-enrolled).</span></span>
- <span data-ttu-id="7c541-110">應用程式套件格式：由 [Microsoft Win32 內容準備工具](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)準備的 .**intunewin** 檔案。</span><span class="sxs-lookup"><span data-stu-id="7c541-110">Application Package format: .**intunewin**  file prepared by the [Microsoft Win32 content Prep tool](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare).</span></span>
- <span data-ttu-id="7c541-111">限制：</span><span class="sxs-lookup"><span data-stu-id="7c541-111">Limitations:</span></span>
    - <span data-ttu-id="7c541-112">大小上限：8GB。</span><span class="sxs-lookup"><span data-stu-id="7c541-112">Maximum size: 8GB.</span></span>
    - <span data-ttu-id="7c541-113">不支援的結構： ARM。</span><span class="sxs-lookup"><span data-stu-id="7c541-113">Unsupported architecture: ARMs.</span></span>

<span data-ttu-id="7c541-114">如需有關這些步驟的詳細資訊，請參閱[「在 Microsoft Intune 中新增、指派及監視 Win32 應用程式」](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)的文件。</span><span class="sxs-lookup"><span data-stu-id="7c541-114">Review the doc "[Add, assign, and monitor a Win32 app in Microsoft Intune](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)" for information related to those steps.</span></span>

<span data-ttu-id="7c541-115">有關 Windows 上應用程式部署 (包括 Win32 應用程式) 疑難排解的詳細資訊，請參閱以下文件</span><span class="sxs-lookup"><span data-stu-id="7c541-115">Details on troubleshooting application deployment on Windows including Win32 apps can be reviewed in the following documents</span></span>

- [<span data-ttu-id="7c541-116">應用程式安裝問題的疑難排解</span><span class="sxs-lookup"><span data-stu-id="7c541-116">Troubleshoot App Installation issues</span></span>](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [<span data-ttu-id="7c541-117">Win32 應用程式的疑難排解</span><span class="sxs-lookup"><span data-stu-id="7c541-117">Troubleshoot Win32 Apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)