---
title: Project Online 處於唯讀狀態
ms.author: pebaum
author: pebaum
manager: pamg
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1776"
- "9000205"
ms.openlocfilehash: 988d87ca43f5394728b77561edd8e26fa0668f4ad876a5fcd09cf739092a4d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063007"
---
# <a name="project-online-is-in-a-read-only-state"></a>Project Online 處於唯讀狀態

Project Online 會達到唯讀狀態有三個常見原因：

1. 組織只有 Project Online 基本版授權 (s) 。 這不足以讓網站保持在活狀態，最終會進行取消布建。 我們會將網站設為唯讀狀態，讓系統管理員知道問題是否正確，而且可以取得正確的授權。 系統管理員必須新增 Project Online 專業版和/或進階版授權。 該網站會在該點上以唯讀狀態退出。 如需詳細資訊，請參閱[比較 Project 管理解決方案](https://products.office.com/project/compare-microsoft-project-management-software?tab=1)。
2. 已達到指定的配額。 如需詳細資訊，請參閱[Project Web App 配額](https://docs.microsoft.com/projectonline/tune-project-online-performance#project-web-app-quota)。 檢查[Project Online 中的時段報告資料匯總](https://docs.microsoft.com/ProjectOnline/configure-rollup-of-timephased-reporting-data-in-project-online)，以查看報告細微性可能會對配額使用量產生什麼影響。
3. 唯讀可能是在維護期間可能發生的暫時性情況。 我們的客戶甚至不會注意到大部分的維護，您也不會看到這種情況，但有時會有一些很短的唯讀時段。
