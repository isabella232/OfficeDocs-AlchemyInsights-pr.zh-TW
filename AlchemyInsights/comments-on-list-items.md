---
title: 清單專案的批註
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003821"
- "6841"
ms.openlocfilehash: d72e3de6da9f51ebd5dd8a4eb06e94d7bc5cca81f86bd61902a9587b00f7b7b0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53995468"
---
# <a name="comments-on-list-items"></a>清單專案的批註

使用者可以查看清單專案上的所有批註，並篩選顯示與專案相關的批註或活動的視圖。

使用者必須先注意下列專案，才能新增及刪除批註：

- 批註遵循 SharePoint 內做的許可權設定。
- 尚未建立以顯示在新式使用者介面（像是工作清單）中的傳統清單，將不會有這項批註功能。
- 此版本不提供對 Teams 中清單的批註。
- 不依搜尋編制索引的批註。

系統管理員可以在組織層級停用此功能，方法是在 **Set-SPOTenant** PowerShell Cmdlet 中變更 **CommentsOnListItemsDisabled** 參數。

目前不可能停用網站或清單層級的批註。 我們希望在後續的更新中使用這些控制項，這可能會在第一季度2021。
