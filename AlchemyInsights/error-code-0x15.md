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
description: 若您在遠端桌面服務上啟用 Office 2013 時收到錯誤 (RDS) 部署，請考慮透過編輯登錄來啟用 ADAL。
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100753"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>在遠端桌面服務上啟用 Office 2013 時出錯

若您在遠端桌面服務上啟用 Office 2013 時收到錯誤 (RDS) 部署，請考慮透過編輯登錄來啟用 ADAL。
  
|**登錄機碼**|**類型**|**Value**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

如需詳細資訊，請參閱[在 Windows 裝置上啟用 Office 2013 的新式驗證](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)。
  
> [!NOTE]
>  在 Microsoft 365 Apps 企業版和 Office 2016 中，預設會啟用 ADAL。 遠端桌面服務 (RDS) 以前稱為終端服務。
  