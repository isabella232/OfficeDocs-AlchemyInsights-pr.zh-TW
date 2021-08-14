---
title: SharePoint 大型清單
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: c67632e323f2068faba06779b94ba4fd8e9f319e18cefb7977bd3038ca770210
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53941559"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a>使用 SharePoint 中的大型清單和文件庫

SharePoint 清單和文件庫最多可以包含30000000個專案，但是當其具有超過5000個專案時，當您嘗試使用這些專案時，可能會看到清單檢視閾值錯誤。 此閾值存在的目的是為了維持服務效能。 您無法對它進行變更。 若要避免達到此臨界值：

**使用現代**

顯示許多專案在新式體驗中最適合運作的視圖。 [使用現代化的經驗](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) ，避免您在傳統體驗中所看到的錯誤。

**新增索引**

當您以沒有索引的資料行篩選或排序時，可能會看到錯誤訊息。 從 [設定] 功能表中的 [從 **清單設定** 手動 [新增索引](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0)]，然後再將索引 **欄** 新增。

**編輯清單視圖**

如果使用大型清單時發生錯誤，請 [編輯清單視圖](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372)。

下列四項變更將會移除清單視圖臨界值錯誤。 進行四個變更，以移除所有的錯誤。 如果仍有錯誤，請參閱 [管理大型清單和文件庫](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59)。

1. 從 **欄的第一個排序選取 [** **無**]，**然後依資料行排序**。
2. 從 **第一個群組** 中選取 [**無**]，**然後按該列進行群組**。
3. 選取 [**總計**] 區段中所有欄的 [**無**]。
4. 取消選取 [ **欄** ] 區段中的 [所有] （顯示一欄）。

