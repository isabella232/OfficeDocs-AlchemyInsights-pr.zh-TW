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
ms.openlocfilehash: 7184ffd68f56639a8bcb87e9c6cab88388868103
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764863"
---
# <a name="encrypt-email-messages-in-outlook"></a>加密 Outlook 中的電子郵件

Microsoft 365 郵件加密是以 Microsoft Azure Rights Management （Azure RMS）為基礎，這是 Azure 資訊保護的一部分。 如果您的訂閱包含 Azure 版權管理或 Azure 資訊保護，**您不需要採取任何動作手動啟用或啟用**Rights Management 服務。

根據客戶的意見反應，我們將不再啟用 Exchange 郵件流程規則，以預設會在您的租使用者中自動加密包含特定類型敏感資訊的輸出電子郵件。 相反地，我們會提供如何進行此作業的詳細指示。 如需如何建立傳輸規則以加密機密資訊的其他詳細資料，請參閱[本文](https://aka.ms/OmeEtr)。

- 如果使用網頁上的 Outlook （以前稱為**OWA**）：撰寫電子郵件時，只要按一下 OWA 中的 [**保護**] 即可。 這將會套用「不要轉寄」許可權。 按一下 [**變更許可權**]，然後選擇 [**加密**] 以只加密郵件。

- 若使用**outlook 用戶端**：若要從 outlook 2013 或2016（或 outlook 2016 Mac）傳送加密的郵件，請選取 [**選項** > **許可權**]，然後選取所需的保護選項。

- 若要**自動加密所有**傳送給特定收件者或外部夥伴組織的電子郵件，您必須在 Exchange 系統管理中心中建立郵件流程傳輸規則。 [此支援文章](https://docs.microsoft.com/office365/securitycompliance/define-mail-flow-rules-to-encrypt-email#create-a-mail-flow-rule-to-encrypt-email-messages-with-the-new-ome-capabilities)中提供詳細指示。

