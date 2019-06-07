---
title: 擁有郵件功能的公用資料夾修正電子郵件傳遞問題
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1956
ms.assetid: ''
ms.openlocfilehash: 900b6cc2765937ee005c7e7dce5d33bbdf582601
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752659"
---
# <a name="fix-email-delivery-issues-to-mail-enabled-public-folders"></a>擁有郵件功能的公用資料夾修正電子郵件傳遞問題

如果外部寄件者無法傳送郵件至擁有郵件功能公用資料夾，並寄件者會收到錯誤：**找不到 (550 5.4.1)**，確認電子郵件網域的公用資料夾已設定為內部轉送網域，而不是授權網域：

1. 開啟[Exchange 系統管理中心 (EAC)](https://docs.microsoft.com/Exchange/exchange-admin-center)。

2. 前往 [**郵件流程** \> **公認的網域**] 中，選取公認的網域，然後按一下 [**編輯**。

3. 內容中的頁面，會隨即開啟，如果網域類型設為 [**授權**將值變更為**內部轉送**，然後按一下 [**儲存**。

如果外部寄件者會收到錯誤，**您沒有權限 (550 5.7.13)**，請查看在公用資料夾的匿名使用者的權限的[Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell)中執行下列命令：

`Get-PublicFolderClientPermission -Identity "<PublicFolderIdentity>" -User Anonymous`例如， `Get-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous`。

若要允許外部使用者能夠傳送電子郵件給此公用資料夾，請新增 CreateItems 存取權限給使用者匿名。 例如 `Add-PublicFolderClientPermission -Identity "\Customer Discussion" -User Anonymous -AccessRights CreateItems`。
