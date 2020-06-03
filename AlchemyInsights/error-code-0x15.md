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
ms.openlocfilehash: 468d13e59602cf173ed2e17af44c66babfc28703
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506837"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="03182-103">在遠端桌面服務上啟用 Office 2013 時發生錯誤</span><span class="sxs-lookup"><span data-stu-id="03182-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="03182-104">如果您在遠端桌面服務（RDS）部署上啟用 Office 2013 時收到錯誤，請考慮編輯登錄以啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="03182-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="03182-105">**登錄機碼**</span><span class="sxs-lookup"><span data-stu-id="03182-105">**Registry key**</span></span>|<span data-ttu-id="03182-106">**類型**</span><span class="sxs-lookup"><span data-stu-id="03182-106">**Type**</span></span>|<span data-ttu-id="03182-107">**Value**</span><span class="sxs-lookup"><span data-stu-id="03182-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="03182-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="03182-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="03182-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="03182-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="03182-110">1 </span><span class="sxs-lookup"><span data-stu-id="03182-110">1</span></span>  <br/> |

<span data-ttu-id="03182-111">如需詳細資訊，請參閱[在 Windows 裝置上啟用 Office 2013 的新式驗證](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="03182-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="03182-112">Microsoft 365 應用程式中的 enterprise 和 Office 2016 預設會啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="03182-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="03182-113">遠端桌面服務（RDS）先前命名為 [終端機服務]。</span><span class="sxs-lookup"><span data-stu-id="03182-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  