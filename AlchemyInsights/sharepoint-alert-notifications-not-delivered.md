---
title: 未傳遞 SharePoint 警示通知
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: a422805d11a128909e1be7bf5d08b24efc132e23
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43742038"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>未傳遞 SharePoint 警示通知

請檢查您電子郵件中的 [垃圾郵件] 資料夾，因為有時候提醒可能會到達這裡。

決定是否**未傳遞所有警示**，或是未傳遞特定檔案或文件庫中**的個別警示**。

- **未傳遞個別警示**：如果未傳遞特定檔案或文件庫中的個別警示，您可以嘗試刪除並重新建立。 請參閱[管理、查看或刪除 SharePoint 警示](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)，以重新建立警示。
- **未傳遞所有警示**：如果未傳遞所有來自多個檔案或文件庫的警示，請造訪[服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，檢查是否有任何 SharePoint 或 Exchange 可能發生的諮詢/事件。 問題可能是透過 Exchange 在電子郵件中 SharePoint 警示功能或延遲。 此外，請務必注意是否正在傳遞其他電子郵件，如果不是，則可能是 Exchange 延遲的問題。

警示上的常見問題：

- 無法將提醒傳送給通訊群組，只支援 Security 和 O365 群組。
- 您無法自訂警示電子郵件範本;您必須使用 Microsoft FLOW 或 SharePoint Designer 工作流程來達成這類工作流程。

詳細資訊：

- **警示設定**：如需有關設定警示的詳細資訊，請參閱[建立警示，以在 SharePoint 中的檔案或資料夾變更時取得通知](https://support.office.com/article/create-an-alert-to-get-notified-when-a-file-or-folder-changes-in-sharepoint-e5a79e7b-a146-46da-a9ef-d65409ba8918)。
- **警示疑難排解**：如需疑難排解提醒的詳細資訊，請參閱[使用者不會收到 SharePoint 線上警示通知](https://docs.microsoft.com/sharepoint/support/sites/no-alert-notifications)。
- **高級 O365 相容性警示原則**：如需設定這些警示的詳細資訊，請參閱[相容性警示原則](https://docs.microsoft.com/office365/securitycompliance/alert-policies)。
- **SharePoint 和 OneDrive 審核記錄**檔：如需如何取得這些事件的詳細資訊，請參閱[搜尋審核記錄](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log)檔。
- **由「高級威脅防護」所傳送的警示**：請參閱[SharePoint 和 OneDrive 的 ATP](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)。
- **資料遺失防護原則所傳送的警示**：請參閱[DLP 原則的電子郵件通知](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)。

## <a name="related-topics"></a>相關主題

想要在 SharePoint Online 中試用 Microsoft 流程嗎？

- [建立流程](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint 和流程](https://flow.microsoft.com//blog/sharepoint-and-flow/)
