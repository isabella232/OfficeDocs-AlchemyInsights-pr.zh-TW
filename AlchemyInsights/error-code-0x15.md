---
title: 錯誤碼0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果您在遠端桌面服務 (RDS) 部署上啟用 Office 2013 時收到錯誤, 請考慮編輯登錄以啟用 ADAL。
ms.openlocfilehash: e2249d8ebbd2313c64dda5656a3243fa76d97a9a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35388236"
---
<span data-ttu-id="70205-103">如果您在遠端桌面服務 (RDS) 部署上啟用 Office 2013 時收到錯誤, 請考慮編輯登錄以啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="70205-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="70205-104">**登錄機碼**</span><span class="sxs-lookup"><span data-stu-id="70205-104">**Registry key**</span></span>|<span data-ttu-id="70205-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="70205-105">**Type**</span></span>|<span data-ttu-id="70205-106">**Value**</span><span class="sxs-lookup"><span data-stu-id="70205-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="70205-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="70205-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="70205-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="70205-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="70205-109">一級</span><span class="sxs-lookup"><span data-stu-id="70205-109">1</span></span>  <br/> |

<span data-ttu-id="70205-110">如需詳細資訊, 請參閱[在 Windows 裝置上啟用 Office 2013 的新式驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="70205-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="70205-111">在 Office 365 專業增強版和 Office 2016 中, 預設會啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="70205-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="70205-112">> 遠端桌面服務 (RDS) 先前名為終端機服務。</span><span class="sxs-lookup"><span data-stu-id="70205-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  