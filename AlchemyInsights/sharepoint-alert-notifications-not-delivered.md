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
ms.openlocfilehash: 363f3c79a3b62f3017e6c873f1be3dd195cab883
ms.sourcegitcommit: 5296874062b16f945d9a7a7a9ab29ec53686310b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/21/2020
ms.locfileid: "44343073"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>未傳遞 SharePoint 警示通知

請檢查您電子郵件中的 [垃圾郵件] 資料夾，因為有時候提醒可能會到達這裡。

決定是否**未傳遞所有警示**，或是未傳遞特定檔案或文件庫中**的個別警示**。

- **未傳遞個別警示**：如果未傳遞特定檔案或文件庫中的個別警示，您可以嘗試刪除並重新建立。 請參閱[管理、查看或刪除 SharePoint 警示](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)，以重新建立警示。
- **未傳遞所有警示**：如果未傳遞所有來自多個檔案或文件庫的警示，請造訪[服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，檢查是否有任何 SharePoint 或 Exchange 可能發生的諮詢/事件。 問題可能是透過 Exchange 在電子郵件中 SharePoint 警示功能或延遲。 此外，請務必注意是否正在傳遞其他電子郵件，如果不是，則可能是 Exchange 延遲的問題。

警示上的常見問題：

- 無法將提醒傳送給通訊群組，只支援 Security 和 O365 群組。
- 您無法自訂警示電子郵件範本;您必須使用 Microsoft FLOW 或 SharePoint Designer 工作流程來達成這類工作流程。

## <a name="related-topics"></a>相關主題

想要在 SharePoint Online 中試用 Microsoft 流程嗎？

- [建立流程](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint 和流程](https://flow.microsoft.com//blog/sharepoint-and-flow/)
