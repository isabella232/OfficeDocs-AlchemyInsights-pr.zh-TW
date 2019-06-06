---
title: SharePoint 或 OneDrive 效能問題
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719508"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint 或 OneDrive 變慢、無法存取或無法多名使用者使用

如果以前具有存取權限的多名使用者現在無法使用 OneDrive 或 SharePoint 網站，則可能有暫時服務的問題。 [請查看服務健康情況儀表板](https://portal.office.com/adminportal/home#/servicehealth)。

## <a name="add-and-license-the-user"></a>新增及授權使用者

確定[在商務用 Office 365 中指派授權給使用者](https://docs.microsoft.com/zh-TW/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One)。


## <a name="assign-permissions"></a>指派權限

如果已指派使用者 Sharepoint 授權，但還是收到拒絕存取的訊息，請確定有[指派使用者適當層級](https://docs.microsoft.com/zh-TW/sharepoint/understanding-permission-levels)的權限。

## <a name="consider-using-the-access-request-feature"></a>請考慮使用存取要求功能


  [存取 ](https://support.office.com/zh-TW/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3)要求功能可讓使用者要求存取他們目前無權查看的內容。

## <a name="allow-custom-script-may-cause-access-denied-issues"></a>允許自訂指令碼可能會造成拒絕存取的問題

某些情況下，*允許自訂指令碼*功能可能會顯示拒絕存取。 如需受影響功能清單、安全性考量，以及停用此功能的能力。 請參閱[允許或防止自訂指令碼 (機器翻譯)](https://docs.microsoft.com/zh-TW/sharepoint/allow-or-prevent-custom-script)。

