---
title: 錯誤代碼 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果您正在時啟用遠端桌面服務 (RDS) 部署 Office 2013 收到錯誤，請考慮啟用 ADAL 藉由編輯登錄。
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29929079"
---
<span data-ttu-id="42bd4-103">如果您正在時啟用遠端桌面服務 (RDS) 部署 Office 2013 收到錯誤，請考慮啟用 ADAL 藉由編輯登錄。</span><span class="sxs-lookup"><span data-stu-id="42bd4-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="42bd4-104">**登錄機碼**</span><span class="sxs-lookup"><span data-stu-id="42bd4-104">**Registry key**</span></span>|<span data-ttu-id="42bd4-105">**類型**</span><span class="sxs-lookup"><span data-stu-id="42bd4-105">**Type**</span></span>|<span data-ttu-id="42bd4-106">**值**</span><span class="sxs-lookup"><span data-stu-id="42bd4-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="42bd4-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="42bd4-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="42bd4-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="42bd4-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="42bd4-109">1</span><span class="sxs-lookup"><span data-stu-id="42bd4-109">1</span></span>  <br/> |
   
<span data-ttu-id="42bd4-110">如需詳細資訊，請參閱[Windows 裝置上的 Office 2013 啟用經過驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="42bd4-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="42bd4-p101">在 Office 365 ProPlus 和 Office 2016 預設會啟用 ADAL。> 遠端桌面服務 (RDS) 先前命名為終端機服務。</span><span class="sxs-lookup"><span data-stu-id="42bd4-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

