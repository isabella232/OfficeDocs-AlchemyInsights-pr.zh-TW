---
title: 商務用 OneDriveWeb OneDrive 重新導向至 Delve
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1870"
- "900072"
ms.openlocfilehash: 295dea987cd14ea848d2bf802f57429642d554b9661dc4dbfc805a447b7d0ede
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53922978"
---
# <a name="redirected-to-delve-after-you-click-onedrive"></a>在您按一下 OneDrive 之後重新導向 Delve

請參閱我們的詳細 [疑難排解指南](https://docs.microsoft.com/sharepoint/support/sites/troubleshooting-guide-for-sites-stopped-at-provisioning)。

若要解決此問題，管理員必須授與使用者建立其「我的網站」網站的權利。 這是因為商務用 OneDrive 頁面是在「我的網站」上建立的。

若要授與此許可權，請遵循下列步驟：

1. 在 SharePoint 系統管理中心，按一下 [**使用者設定檔**]。

2. 在 [ **人員** ] 區段中，按一下 [ **管理使用者許可權**]。

3. 新增需要許可權才能建立「我的網站」網站的使用者。 根據預設，此設定會設定為 [ **外部使用者以外的所有人**]。

4. 在您新增使用者、使用者或群組之後，請確定已選取 [已新增使用者、使用者或群組]、[ **許可權** ] 區段，然後選取 [ **建立個人儲存區、新聞摘要] 及 [追蹤內容) 所需的個人網站 (**] 旁邊的核取方塊。

5. 按一下 **[確定]**，然後讓使用者流覽至 OneDrive 頁面以建立網站。
