---
title: 疑難排解登入 OneDrive
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8283"
- "9004614"
ms.openlocfilehash: 2c9a390f38ecbba94698a352348e2e533a50ee17
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/24/2021
ms.locfileid: "52626104"
---
# <a name="troubleshoot-signing-in-to-onedrive"></a>疑難排解登入 OneDrive

本文說明下列案例：

- 針對關於登入 OneDrive 同步處理用戶端的問題進行疑難排解
- 針對關於登入商務用 OneDrive 網站的問題進行疑難排解

**針對關於登入 OneDrive 同步處理用戶端的問題進行疑難排解**

- 有關解决錯誤代碼 0x004de40 的步驟，請參閱[登入至 OneDrive 時的錯誤碼 0x8004de40](/sharepoint/troubleshoot/administration/error-0x8004de40-in-onedrive)。
- 造訪網站以登入 OneDrive 或 SharePoint 網站，然後按一下網站功能表列頂端的 [同步] 按鈕。
- 確保您正在登入商務用 OneDrive，而不是 OneDrive.com。 如果您造訪的 URL 開頭為 onedrive.live.com，則該 URL 不是您商務用 OneDrive 的位置。 要確保您登入的是商務用 OneDrive 的一個簡單方法是透過此連結：https://portal.office.com/onedrive，然後使用您的公司或學校帳戶登入。
- 如果您仍無法解決問題，請考慮[重設 OneDrive](https://support.microsoft.com/office/reset-onedrive-34701e00-bf7b-42db-b960-84905399050c)。
- [將您的帳戶與 OneDrive 取消連結](https://support.microsoft.com/office/how-to-remove-an-account-in-onedrive-72699268-9e64-45bd-b723-9a19f4512fd1)，登入 OneDrive 或 SharePoint 網站，然後按一下網站功能表列頂端的 [同步] 按鈕。

**針對關於登入商務用 OneDrive 網站的問題進行疑難排解**

- 確保您正在登入商務用 OneDrive，而不是 OneDrive.com。 如果您造訪的 URL 開頭為 onedrive.live.com，則該 URL 不是您商務用 OneDrive 的位置。 要確保您登入的是商務用 OneDrive 的一個簡單方法是透過此連結：https://portal.office.com/onedrive，然後使用您的公司或學校帳戶登入。
- 如果已將您重新導向您的 Delve 個人檔案頁面，Microsoft 365 系統管理員將需要[授與使用者建立自己的商務用 OneDrive 網站的權限](https://support.microsoft.com/office/you-re-redirected-to-your-delve-profile-page-after-you-click-onedrive-on-the-microsoft-365-app-launcher-2af26640-9ddf-46c3-8912-6af30efcc7b0)。
- 使用 [Microsoft Edge 中的 InPrivate 瀏覽](https://support.microsoft.com/microsoft-edge/browse-inprivate-in-microsoft-edge-e6f47704-340c-7d4f-b00d-d0cf35aa1fcc) (或另一個瀏覽器中的類似功能) 來測試您是否可以造訪 OneDrive 網站。
    - 如果 InPrivate 瀏覽可正常運作，則您可能需要[在 Microsoft Edge 中清除您的瀏覽資料](https://support.microsoft.com/microsoft-edge/view-and-delete-browser-history-in-microsoft-edge-00cf7943-a9e1-975a-a33d-ac10ce454ca4) (或另一個瀏覽器中的類似功能)。

**疑難排解登入 Office 以與 OneDrive 同步的問題**

如果您收到說明 **已封鎖上傳**、**登入以儲存此檔案** 或 **儲存複本** 的錯誤訊息，您可能需要 [從 Office 已連線的服務移除並重新連線 OneDrive](https://support.microsoft.com/office/how-to-resolve-upload-blocked-sign-into-save-this-file-or-save-a-copy-error-messages-32c7340c-f5fb-4ca0-a829-65d8120f81f8)。

**其他疑難排解提示**

如果您是全域、授權或使用者系統管理員，請[將正確的授權指派給受影響的使用者](/microsoft-365/admin/manage/assign-licenses-to-users)。

