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
如果您正在時啟用遠端桌面服務 (RDS) 部署 Office 2013 收到錯誤，請考慮啟用 ADAL 藉由編輯登錄。 
  
|**登錄機碼**|**類型**|**值**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
如需詳細資訊，請參閱[Windows 裝置上的 Office 2013 啟用經過驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。
  
> [!NOTE]
>  在 Office 365 ProPlus 和 Office 2016 預設會啟用 ADAL。> 遠端桌面服務 (RDS) 先前命名為終端機服務。 
  

