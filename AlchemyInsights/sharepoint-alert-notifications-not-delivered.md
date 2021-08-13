---
title: 未傳遞 SharePoint 警示通知
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "1655"
ms.openlocfilehash: 05bd913098372a57d3061e8c516a6a6b4f0a9bdafde02acc930062d6281d06dd
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53957892"
---
# <a name="sharepoint-alert-notifications-not-delivered"></a>未傳遞 SharePoint 警示通知

請檢查您電子郵件中的 [垃圾郵件] 資料夾，因為有時候提醒可能會到達這裡。

決定是否 **未傳遞所有警示** ，或是未傳遞特定檔案或文件庫中 **的個別警示** 。

- **未傳遞個別警示**：如果未傳遞特定檔案或文件庫中的個別警示，您可以嘗試刪除並重新建立。 請參閱[管理、查看或刪除 SharePoint 警示](https://support.office.com/article/manage-view-or-delete-sharepoint-alerts-99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2)，以重新建立警示。
- **未傳遞所有警示**：如果未傳遞所有來自多個檔案或文件庫的警示，請造訪 [服務健康情況儀表板](https://admin.microsoft.com/AdminPortal/Home#/servicehealth)，檢查是否有任何 SharePoint 或 Exchange 發生的諮詢/事件。 問題可能是透過 Exchange 的電子郵件中 SharePoint 警示功能或延遲。 此外，請務必注意是否正在傳遞其他電子郵件，如果不是，則可能是 Exchange 延遲的問題。

警示上的常見問題：

- 無法將提醒傳送給通訊群組，只支援 Security 和 O365 群組。
- 您無法自訂警示電子郵件範本;您必須使用 Microsoft FLOW 或 SharePoint Designer 工作流程來達成這類工作流程。

## <a name="related-topics"></a>相關主題

想要在 SharePoint 線上中嘗試 Microsoft Flow 嗎？

- [建立 Flow](https://support.office.com/article/a9c3e03b-0654-46af-a254-20252e580d01)

- [SharePoint 和 Flow](https://flow.microsoft.com//blog/sharepoint-and-flow/)
