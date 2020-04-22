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
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>在遠端桌面服務上啟用 Office 2013 時發生錯誤

如果您在遠端桌面服務（RDS）部署上啟用 Office 2013 時收到錯誤，請考慮編輯登錄以啟用 ADAL。
  
|**登錄機碼**|**類型**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1   <br/> |

如需詳細資訊，請參閱[在 Windows 裝置上啟用 Office 2013 的新式驗證](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication)。
  
> [!NOTE]
>  Microsoft 365 應用程式中的 enterprise 和 Office 2016 預設會啟用 ADAL。 遠端桌面服務（RDS）先前命名為 [終端機服務]。
  