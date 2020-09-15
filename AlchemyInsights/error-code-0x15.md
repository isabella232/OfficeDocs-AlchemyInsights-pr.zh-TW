---
title: 錯誤碼0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果您在遠端桌面服務上啟用 Office 2013 時收到錯誤 (RDS) 部署，請考慮透過編輯登錄來啟用 ADAL。
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709178"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="281e5-103">在遠端桌面服務上啟用 Office 2013 時發生錯誤</span><span class="sxs-lookup"><span data-stu-id="281e5-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="281e5-104">如果您在遠端桌面服務上啟用 Office 2013 時收到錯誤 (RDS) 部署，請考慮透過編輯登錄來啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="281e5-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="281e5-105">**登錄機碼**</span><span class="sxs-lookup"><span data-stu-id="281e5-105">**Registry key**</span></span>|<span data-ttu-id="281e5-106">**Type**</span><span class="sxs-lookup"><span data-stu-id="281e5-106">**Type**</span></span>|<span data-ttu-id="281e5-107">**Value**</span><span class="sxs-lookup"><span data-stu-id="281e5-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="281e5-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="281e5-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="281e5-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="281e5-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="281e5-110">1 </span><span class="sxs-lookup"><span data-stu-id="281e5-110">1</span></span>  <br/> |

<span data-ttu-id="281e5-111">如需詳細資訊，請參閱 [在 Windows 裝置上啟用 Office 2013 的新式驗證](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="281e5-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="281e5-112">Microsoft 365 應用程式中的 enterprise 和 Office 2016 預設會啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="281e5-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="281e5-113">遠端桌面服務 (RDS) 以前稱為終端服務。</span><span class="sxs-lookup"><span data-stu-id="281e5-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  