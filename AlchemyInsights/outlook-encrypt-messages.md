---
title: Outlook 網頁版中的 S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: 33e94eac6a2982b8036e13d17bf60015f244f2cb
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 12/15/2019
ms.locfileid: "40053216"
---
# <a name="encrypt-email-messages-in-outlook"></a>在 Outlook 中的電子郵件加密

Office 365 郵件加密是內建於 Microsoft Azure 版權管理 (Azure RMS)，也就是 Azure 資訊保護的一部分。 如果您的訂閱包含 Azure 版權管理 」 或 「 Azure 資訊保護，**您不需要採取任何動作，以手動啟用或啟動**版權管理服務。

根據客戶意見反應，我們將不再讓 Exchange 郵件流程規則來自動加密預設包含特定類型的租用戶中的敏感資訊的外寄電子郵件。 相反地，我們會提供的詳細的指示上如何可以進行自己。 如需如何建立傳輸規則以加密敏感資訊的其他詳細資訊，請參閱[這篇文章](https://aka.ms/OmeEtr)。

- 如果使用 Outlook 網頁 (先前稱為**OWA**): 當您在撰寫電子郵件，只要按一下 [在 OWA 中的**保護**。 這將會套用 「 不要轉寄 」 權限。 按一下 [**變更權限**，然後選擇 [僅加密訊息**加密**。

- 如果使用**Outlook 用戶端**： 從來傳送加密的郵件 Outlook 2013 或 2016 或 Outlook 2016 for Mac 中，選取 [**選項** > **權限**，然後選取您需要的保護選項。

- 若要**自動加密所有電子郵件**傳送給特定收件者或外部夥伴組織，您需要在 Exchange 系統管理中心中建立郵件流程傳輸規則。 [支援本文](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)所提供的詳細的指示。

