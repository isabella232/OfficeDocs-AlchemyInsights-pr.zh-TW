---
title: 疑難排解 SAML 簽署憑證問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9406"
- "9004341"
ms.openlocfilehash: fb043122edf5f99325f0403810eb0dc119d254e0
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314411"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a>疑難排解 SAML 簽署憑證問題

若要解決 SAML 簽署憑證問題，請執行下列建議步驟：

1. 當您新增支援 SSO 的企業應用程式時，Azure 會產生名為 [SAML 簽署憑證](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) 的憑證。 此憑證的到期日為 3 年。 若要變更您的憑證的到期日，請參閱 [自訂您的同盟憑證的到期日，並轉用至新的憑證](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)。
2. Azure 會使用此憑證簽署應用程式所要求的 SAML 權杖，並將之傳送至應用程式，以取得成功的 SSO。 若要完成此程序，請從 Azure 入口網站下載憑證，並將之傳送至應用程式廠商以完成 SSO 程序。

完成此程序之後，您的應用程式將會信任此憑證，且應用程式將接受此憑證所簽署的所有 SAML 權杖。

3. 如果此憑證過期，請建立新憑證，將之更新至應用程式廠商，然後在 Azure 端啟動該憑證。 如需詳細資訊，請參閱 [更新即將到期的憑證](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)。

**注意**：如果憑證過期，並不會封鎖使用者。

4. [新增收取通知的電子郵件地址](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) 以在目前憑證到期前接收通知。

**注意**：步驟 4 是選擇性步驟。

5. 變更應用程式的 SAML 憑證簽署選項和憑證簽署演算法。 如需詳細資訊，請參閱 [變更憑證簽署選項和簽署演算法](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)。

