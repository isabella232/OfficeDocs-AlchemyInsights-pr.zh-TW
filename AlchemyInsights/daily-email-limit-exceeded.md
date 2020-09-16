---
title: 超過每日電子郵件限制。 工作流程已暫停。
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5200020"
- "1227"
ms.openlocfilehash: dfb42b24f1c2b4b05cb067a82505a6a8b63f277e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731554"
---
# <a name="daily-email-limit-exceeded-workflow-is-suspended"></a>超過每日電子郵件限制。 工作流程已暫停。

在下列案例中，您可能會收到此錯誤：

- 您在使用 SharePoint 2010 或 SharePoint 2013 工作流程平臺類型的 SharePoint Online 中有工作流程。
- 工作流程設定為一次傳送自訂的電子郵件訊息給超過200位使用者、每天超過10000個收件者，或每分鐘超過30封郵件。
- 當您執行工作流程時，未傳送電子郵件訊息，您會注意到下列行為：
    - 針對使用 SharePoint 2013 平臺類型的工作流程，請流覽至 [ **工作流程狀態** ] 頁面。 在 [工作流程狀態] 頁面上， **內部狀態** 會設定為 [ **已啟動**]，而 [資訊] 氣球會顯示 **無法傳送給收件**者。

若要解決此問題，請設定工作流程以傳送電子郵件，但不超過 [Exchange Online 寄件者限制](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#recipientlimits)。 例如，在工作流程中使用 pause，將電子郵件傳送至 Microsoft 365 群組、通訊群組或啟用郵件功能的安全性群組，或一次傳送郵件給超過200個收件者。


如需詳細資訊，請參閱下列 [文章](https://support.microsoft.com/help/3150442/daily-email-limit-has-exceeded-and-your-workflow-has-been-suspended-or)。

## <a name="related-topics"></a>相關主題
- [建立流程](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [SharePoint 和流程](https://flow.microsoft.com/blog/sharepoint-and-flow/) 