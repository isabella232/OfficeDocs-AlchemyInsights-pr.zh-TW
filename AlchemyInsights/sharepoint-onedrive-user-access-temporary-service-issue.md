---
title: 效能問題-SharePoint 或 OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771235"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>多個使用者的 SharePoint 或 OneDrive 變慢、無法存取或無法使用

如果有 OneDrive 或 SharePoint 網站無法供先前具有存取權的使用者使用，則可能會發生暫時的服務問題。 [檢查服務健康情況儀表板](https://portal.office.com/adminportal/home#/servicehealth)。

**新增及授權使用者**

確定您 [將授權指派給 Microsoft 365 for business 中的使用者](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users)。


**指派許可權**

若使用者已獲指派 Sharepoint 授權，但仍收到「拒絕存取」訊息，請確定已指派適當的 [許可權等級](https://docs.microsoft.com/sharepoint/understanding-permission-levels) 。

**考慮使用存取要求功能**

「 [存取要求」功能](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) 可讓使用者要求存取其目前未具有查看許可權的內容。

**允許自訂腳本可能會造成存取權拒絕問題**

在某些情況下， *允許自訂腳本* 的功能可能會遭到拒絕存取。 如需受影響的功能清單，安全性考慮和停用功能的功能。 請造訪 [Allow 或預防自訂腳本](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script)。

