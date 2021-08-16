---
title: Outlook 網頁版中的 S/MIME
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 9000329
ms.openlocfilehash: bef87baafdbaf9346f99f1ff54aaa83bc9173c70f1412ea00afb717c15a8014c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54010715"
---
# <a name="encrypt-email-messages-in-outlook"></a>加密 Outlook 中的電子郵件

Microsoft 365郵件加密是以 Microsoft Azure Rights Management (azure RMS) 為基礎，這是 azure 資訊保護的一部分。 如果您的訂閱包含 Azure 版權管理或 Azure 資訊保護， **您不需要採取任何動作手動啟用或啟用** Rights Management 服務。

根據客戶的意見反應，我們將不再啟用 Exchange 郵件流程規則，在您的租使用者中，預設會自動將包含特定類型敏感資訊的輸出電子郵件加密。 相反地，我們會提供如何進行此作業的詳細指示。 如需如何建立傳輸規則以加密機密資訊的其他詳細資料，請參閱 [本文](https://aka.ms/OmeEtr)。

- 如果使用網頁上的 Outlook (以前的 **OWA**) ：撰寫電子郵件時，只要按一下 owa 中的 [**保護**] 即可。 這將會套用「不要轉寄」許可權。 按一下 [ **變更許可權** ]，然後選擇 [ **加密** ] 以只加密郵件。

- 若使用 **Outlook 用戶端**：若要從 Outlook 2013 或2016傳送加密的郵件，或 Mac 版 Outlook 2016，請選取 [**選項**  >  **許可權**]，然後選取所需的保護選項。

- 若要 **自動加密所有** 傳送給特定收件者或外部夥伴組織的電子郵件，您必須在 Exchange 系統管理中心建立郵件流程傳輸規則。 [此支援文章](https://docs.microsoft.com/microsoft-365/compliance/define-mail-flow-rules-to-encrypt-email#create-mail-flow-rules-to-encrypt-email-messages-with-the-new-ome-capabilities)中提供詳細指示。

