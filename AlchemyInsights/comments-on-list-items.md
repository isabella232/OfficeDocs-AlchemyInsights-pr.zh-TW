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
ms.openlocfilehash: 5940d1a96324c5ca77331485a115689abe547ef7
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 11/09/2020
ms.locfileid: "48947488"
---
# <a name="comments-on-list-items"></a>清單專案的批註

使用者將很快可以新增及刪除清單專案的批註。 使用者可以查看清單專案上的所有批註，並篩選顯示與專案相關的批註或活動的視圖。

**計時** ：

**目標版本** ：逐步推出于十月，預計會在2006年11月完成

**標準版本** ：逐步推出，在十二月的初期完成

**首展** ：整個組織的目標發行

使用者必須先注意下列專案，才能新增及刪除批註：

- 批註遵循 SharePoint 內做的許可權設定。
- 尚未建立以顯示在新式使用者介面（像是工作清單）中的傳統清單，將不會有這項批註功能。
- 在此版本中，不提供對小組中清單的批註。
- 不依搜尋編制索引的批註。

系統管理員可以在組織層級停用此功能，方法是在 **Set-SPOTenant** PowerShell Cmdlet 中變更 **CommentsOnListItemsDisabled** 參數。

目前不可能停用網站或清單層級的批註。 我們希望在後續的更新中使用這些控制項，這可能會在第一季度2021。
