---
title: 錯誤碼 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: 如果您在遠端桌面服務 (RDS) 部署上啟動 Office 2013 時收到錯誤訊息，請考慮啟用 ADAL 藉由編輯登錄。
ms.openlocfilehash: 6d4076ecb5c6ee3c3cf4c4610ad4aa29ab477d8a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402730"
---
<span data-ttu-id="7196d-103">如果您在遠端桌面服務 (RDS) 部署上啟動 Office 2013 時收到錯誤訊息，請考慮啟用 ADAL 藉由編輯登錄。</span><span class="sxs-lookup"><span data-stu-id="7196d-103">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span> 
  
|<span data-ttu-id="7196d-104">**登錄機碼**</span><span class="sxs-lookup"><span data-stu-id="7196d-104">**Registry key**</span></span>|<span data-ttu-id="7196d-105">**Type**</span><span class="sxs-lookup"><span data-stu-id="7196d-105">**Type**</span></span>|<span data-ttu-id="7196d-106">**Value**</span><span class="sxs-lookup"><span data-stu-id="7196d-106">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7196d-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="7196d-107">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="7196d-108">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="7196d-108">REG_DWORD</span></span>  <br/> |<span data-ttu-id="7196d-109">1 </span><span class="sxs-lookup"><span data-stu-id="7196d-109">1</span></span>  <br/> |
   
<span data-ttu-id="7196d-110">如需詳細資訊，請參閱 < <b0>Windows 裝置上的 Office 2013 啟用新式驗證</b0>。</span><span class="sxs-lookup"><span data-stu-id="7196d-110">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="7196d-111">在 Office 365 專業增強版和 Office 2016 中的預設會啟用 ADAL。</span><span class="sxs-lookup"><span data-stu-id="7196d-111">ADAL is enabled by default in Office 365 ProPlus and Office 2016.</span></span> <span data-ttu-id="7196d-112">> 遠端桌面服務 (RDS) 已先前稱為終端機服務。</span><span class="sxs-lookup"><span data-stu-id="7196d-112">>  Remote Desktop Services (RDS) was previously named Terminal Services.</span></span> 
  

