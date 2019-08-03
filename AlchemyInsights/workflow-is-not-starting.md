---
title: 無法啟動工作流程
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171765"
---
# <a name="workflow-is-not-starting"></a>無法啟動工作流程

- 無法啟動 SharePoint 2010 和 SharePoint 2013 工作流程。

    如果無法啟動您的工作流程，可能有的暫時的服務問題： 使用者可能會遇到間歇性延遲與工作流程進度。 檢查[服務健康狀況儀表板](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth)若要查看您的組織會受到影響。

    如果您第一次看到此問題以來超過 24 小時，請登支援票證。 在許多情況下，我們已使用的方案。 請讓我們至少 24 小時才能完成解決方案。

- SharePoint 2010 工作流程延遲開始。

    如果在大型的批次中觸發工作流程時，發生此情況。 （例如，當多個項目會新增一次）。

    工作流程是並非特別設計用來執行即時，因此延遲是所設計的行為。

    如果工作流程是複雜的 「 可延伸物件標記語言 」 (XMOL)，編譯可能會很慢。 請檢查[這](https://support.microsoft.com/en-us/kb/3043697)篇文章。

    您應該簡化工作流程或重新設計使用 Microsoft SharePoint 2013 工作流程平台類型。

    此外，如果您的工作流程歷程記錄有變大，可能會想要清除項目或建立新的歷程記錄清單。

    [清除工作流程歷程記錄](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)的詳細資訊：


## <a name="related-topics"></a>相關主題
想要在 SharePoint Online 中的 Micrsoft 流程？
- [建立流程](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流程](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


