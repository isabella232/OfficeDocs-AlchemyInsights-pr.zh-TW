---
title: 錯誤代碼 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果您正在時啟用遠端桌面服務 (RDS) 部署 Office 2013 收到錯誤，請考慮啟用 ADAL 藉由編輯登錄。
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/24/2019
ms.locfileid: "29499373"
---
<span data-ttu-id="a243b-103">如果您正在時啟用遠端桌面服務 (RDS) 部署 Office 2013 收到錯誤，請考慮啟用 ADAL 藉由編輯登錄。</span><span class="sxs-lookup"><span data-stu-id="a243b-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="a243b-104">**登錄機碼**</span><span class="sxs-lookup"><span data-stu-id="a243b-104">**Registry key**</span></span>|<span data-ttu-id="a243b-105">**類型**</span><span class="sxs-lookup"><span data-stu-id="a243b-105">**Type**</span></span>|<span data-ttu-id="a243b-106">**值**</span><span class="sxs-lookup"><span data-stu-id="a243b-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a243b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="a243b-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="a243b-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="a243b-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="a243b-109">^1</span><span class="sxs-lookup"><span data-stu-id="a243b-109">1</span></span>  <br/> |
   
<span data-ttu-id="a243b-110">如需詳細資訊，請參閱[Windows 裝置上的 Office 2013 啟用經過驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。</span><span class="sxs-lookup"><span data-stu-id="a243b-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="a243b-p101">在 Office 365 ProPlus 和 Office 2016 預設會啟用 ADAL。> 遠端桌面服務 (RDS) 先前命名為終端機服務。</span><span class="sxs-lookup"><span data-stu-id="a243b-p101">ADAL is enabled by default in Office 365 ProPlus and Office 2016. >  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

