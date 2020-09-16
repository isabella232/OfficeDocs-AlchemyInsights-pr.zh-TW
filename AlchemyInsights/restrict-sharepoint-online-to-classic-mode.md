---
title: 將 SharePoint 線上限制為傳統模式
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.custom:
- "1835"
- "1889"
- "9000225"
ms.openlocfilehash: 1887bf64df98bf90a1902250633d5774178dfa2f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47751413"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a>將 SharePoint 線上限制為傳統模式

有些組織仍然需要傳統模式體驗。 雖然沒有任何計畫在細微層級移除傳統模式，但無法再將整個組織 (租使用者) 至傳統模式，以供清單和文件庫使用。

系統管理員可以使用下列方式，以傳統模式管理個別的清單和文件庫，其可在下列層級提供：

- 網站集合
- 網站
- 清單
- 圖書館

此外，使用一些目前不支援的特定功能和自訂的清單，仍然會自動切換成傳統模式。

從2019年4月1日開始，停用租使用者層級的程式會退出現代清單，而文件庫會在5月 31 2019 日內開始並繼續執行。  由於承租人自願退出，以傳統模式表示的清單和文件庫會自動移至新式。

如果您需要傳統 [模式，請](https://techcommunity.microsoft.com/t5/Microsoft-SharePoint-Blog/Delivering-SharePoint-modern-experiences/ba-p/315023) 參閱此處的詳細資訊，並 PnP [在這裡](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries-optout) 描述您可以用來使用傳統模式體驗之選項及工具的 Powershell 說明。
