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
如果您在遠端桌面服務 (RDS) 部署上啟動 Office 2013 時收到錯誤訊息，請考慮啟用 ADAL 藉由編輯登錄。 
  
|**登錄機碼**|**Type**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |
   
如需詳細資訊，請參閱 < <b0>Windows 裝置上的 Office 2013 啟用新式驗證</b0>。
  
> [!NOTE]
>  在 Office 365 專業增強版和 Office 2016 中的預設會啟用 ADAL。 > 遠端桌面服務 (RDS) 已先前稱為終端機服務。 
  

