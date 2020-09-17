---
title: 未開始工作流程
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794758"
---
# <a name="workflow-is-not-starting"></a>未開始工作流程

- SharePoint 2010 和 SharePoint 2013 工作流程無法啟動。

    - 如果您的工作流程未開始，可能是暫時性的服務問題，使用者可能會遇到工作流程進度的延遲延遲。 請檢查 [服務健康情況儀表板](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) ，以查看您的組織是否受到影響。

    - 如果從您第一次看到此問題起已經過去超過24小時，請記錄支援票證。 多數情況下，我們已經著手研究解決方案。 請至少為我們提供24小時的時間來完成解決方案。

- SharePoint 2010 工作流程在開始時延遲。

    - 如果工作流程以大量批次觸發，便會發生這種情況。  (例如，一次新增多個專案) 。

    - 工作流程並非設計為即時執行，所以延遲是設計行為。

   -  如果工作流程是複雜且可擴展的物件標記語言 (XMOL) ，編譯可能會很慢。 請[參閱本文。](https://support.microsoft.com//kb/3043697)

    - 您應該簡化工作流程，或使用 Microsoft SharePoint 2013 工作流程平臺類型進行重新設計。

    - 如果您的工作流程歷程記錄已增加，您可能想要清除專案或建立新的歷程記錄清單。

        詳細資訊： [清除工作流程歷程記錄](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)


## <a name="related-topics"></a>相關主題
想要在 SharePoint Online 中試用 Microsoft 流程嗎？
- [建立流程](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流程](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


