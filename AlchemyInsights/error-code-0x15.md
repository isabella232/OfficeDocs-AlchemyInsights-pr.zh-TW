---
title: 錯誤碼0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果您在遠端桌面服務（RDS）部署上啟用 Office 2013 時收到錯誤，請考慮編輯登錄以啟用 ADAL。
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703129"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="44751-103">在遠端桌面服務上啟用 Office 2013 時發生錯誤</span><span class="sxs-lookup"><span data-stu-id="44751-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="44751-104">如果您在遠端桌面服務（RDS）部署上啟用 Office 2013 時收到錯誤，請考慮編輯登錄以啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="44751-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="44751-105">**登錄機碼**</span><span class="sxs-lookup"><span data-stu-id="44751-105">**Registry key**</span></span>|<span data-ttu-id="44751-106">**類型**</span><span class="sxs-lookup"><span data-stu-id="44751-106">**Type**</span></span>|<span data-ttu-id="44751-107">**Value**</span><span class="sxs-lookup"><span data-stu-id="44751-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="44751-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="44751-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="44751-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="44751-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="44751-110">1 </span><span class="sxs-lookup"><span data-stu-id="44751-110">1</span></span>  <br/> |

<span data-ttu-id="44751-111">如需詳細資訊，請參閱[在 Windows 裝置上啟用 Office 2013 的新式驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="44751-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="44751-112">Microsoft 365 應用程式中的 enterprise 和 Office 2016 預設會啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="44751-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="44751-113">遠端桌面服務（RDS）先前命名為 [終端機服務]。</span><span class="sxs-lookup"><span data-stu-id="44751-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  