---
title: 嘗試使用 SharePoint 或 OneDrive 時進行維護訊息的 Read-Only
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
- "127"
- "128"
ms.assetid: de7b6877-f3f9-4402-8072-c73783aaccaa
ms.openlocfilehash: a3d313816beefcefa4d93528d3ad9a684e60390e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670823"
---
# <a name="read-only-for-maintenance-message-when-attempting-to-use-sharepoint-or-onedrive"></a>嘗試使用 SharePoint 或 OneDrive 時進行維護訊息的 Read-Only

當下列其中一種案例嘗試使用 SharePoint 或 OneDrive 時，使用者可能會收到 **Read-Only 以進行維護** 訊息。 

-   已計畫或主動維護活動。  流覽至 [訊息中心](https://portal.office.com/adminportal/home#/messagecenter)以檢查是否有這些檔案。
-   可能發生的高優先順序主動服務事件。 流覽至 [服務健康情況](https://portal.office.com/adminportal/home#/servicehealth)，以檢查是否有任何建議/事件。
-   一種次要的自動修復復原案例，因為伺服器上可能有超過30分鐘以上的任何未預期事件，可能會發生這種情況。 
    
    這些次要復原沒有任何訊息中心或服務健康情況文章，但您應該可以立即恢復正常。

在極少數的情況下，我們看到上述三個案例中的其中一種是導致原因，而服務已還原，但使用者瀏覽器快取尚未清除。

請先嘗試清除瀏覽器快取，然後再流覽至網站。

1. 在您的 Microsoft Edge browser 中，選取 [ **設定**]，然後選取 [ **隱私權與安全性**]。
2. 在 [ **清除流覽**] 底下，選取 **[選擇要清除**的專案]。
3. 選取 [ **cookie] 和 [儲存的網站資料**]，然後選取 [ **清除**]。

>[!Note] 
> 當您使用其他瀏覽器（例如 Mozilla Firefox 或 Google Chrome）時，可能會有不同的步驟。

>[!Note] 
> 另一個選項是在新的 InPrivate 視窗中開啟 SharePoint 網站或 OneDrive。