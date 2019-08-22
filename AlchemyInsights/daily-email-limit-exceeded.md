---
title: 已超過每日的電子郵件限制。 暫止工作流程。
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 7/25/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: e3fbcd5bfc279847cfb39140c3689f5433b61509
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36514433"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>超過限制每日的電子郵件。 暫止工作流程。

在下列案例中可能會收到此錯誤：

- 您可以讓工作流程在 SharePoint Online 中使用 SharePoint 2010 或 SharePoint 2013 工作流程平台類型。
- 工作流程已設定為傳送自訂電子郵件訊息給 200 位以上的使用者在時間、 10000 個以上的收件者每日或每分鐘 30 個以上的郵件。
- 當您執行的工作流程時，不會傳送電子郵件訊息，並請注意下列行為：
    - 使用 [SharePoint 2013 平台類型為工作流程，您瀏覽至 [**工作流程狀態**] 頁面上。 在 [工作流程狀態] 頁面**內部的狀態**設定為 [**已啟動**，並資訊註解方塊會顯示**無法傳送給收件者**。

若要解決此問題，設定您的工作流程不超過[Exchange Online 寄件者限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)傳送電子郵件訊息。 例如，使用工作流程中的暫停、 傳送電子郵件給 Office 365 群組、 通訊群組或擁有郵件功能的安全性群組，或將郵件傳送至 200 個收件者，一次。


如需詳細資訊，請參閱下列[文章](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)。

## <a name="related-topics"></a>相關主題
- [建立流程](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流程](https://flow.microsoft.com/blog/sharepoint-and-flow/) 