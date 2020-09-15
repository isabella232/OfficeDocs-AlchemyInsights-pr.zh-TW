---
title: 在 Yammer 中發布開啟的或下載的檔案
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6041"
- "9003112"
ms.openlocfilehash: de335e27624caf5a91bdc2913570eba92f627282
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695640"
---
# <a name="issue-opening-or-downloading-files-in-yammer"></a>在 Yammer 中發布開啟的或下載的檔案

傳統的 Yammer 支援多種上傳檔案到郵件和群組的選項。 根據網路設定，檔案預設為儲存在 SharePoint 中。

新版 Yammer 中的檔案選擇器尚未支援傳統 Yammer 中提供的所有選項。 未來的更新將新增其他功能。 如需詳細資訊，請參閱 [將檔案或影像附加至 Yammer 對話文章中](https://support.microsoft.com/office/attach-a-file-or-image-to-a-yammer-conversation-post-8d2d17f7-8f37-4535-961e-518d751be7e8)。

**無法開啟或下載檔案**  

檔案可能會上傳至 Yammer，但也會連結至 SharePoint Online 中的檔案。 若要進行疑難排解，您必須先決定檔案的位置。 如果檔案已下載到 Yammer，則會有 *.yammer.com 的URL。 確保要求的 URL 和 IP 位置未被封鎖。 如需詳細資訊，請參閱部落格文章 [不推薦在 Ymmer 上使用硬編碼 IP 位址](https://techcommunity.microsoft.com/t5/yammer-blog/using-hard-coded-ip-addresses-for-yammer-is-not-recommended/ba-p/276592)。

請查看是否也是全域系統管理人的使用者可以下載檔案。 如果檔案為私人檔案，您可能需要使用 [私人內容模式]。 如需詳細資訊，請參閱 [監視 Yammer 中的私人內容](https://docs.microsoft.com/yammer/manage-security-and-compliance/monitor-private-content)。  

**Yammer 網路層級來賓和 SharePoint Online 中的檔案**  

[Yammer 中的網路層級來賓](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#invite-guests) 不使用 Azure AD B2B 且為 Yammer 服務的內部使用者，因此他們無法存取儲存在 SharePoint 中的 Yammer 檔案。 建立可使用該身分識別在 SharePoint Online 中存取文件庫的外部 AAD B2B 使用者。 如需 Yammer 中未來 Azure AD B2B 來賓支援的相關資訊，請參閱 [在 Yammer 預覽中的企業對企業（B2B）來賓支援-客戶條款與常見問題](https://docs.microsoft.com/yammer/get-started-with-yammer/azure-ad-b2b-guests-yammer)。