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
ms.openlocfilehash: 3bc8b2e751395b8a099fb5079ad40c5c93222e0e
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529178"
---
# <a name="troubleshoot-saml-signing-certificate-issues"></a><span data-ttu-id="7c5be-102">疑難排解 SAML 簽署憑證問題</span><span class="sxs-lookup"><span data-stu-id="7c5be-102">Troubleshoot SAML Signing certificate issues</span></span>

<span data-ttu-id="7c5be-103">若要解決 SAML 簽署憑證問題，請執行下列建議步驟：</span><span class="sxs-lookup"><span data-stu-id="7c5be-103">To resolve SAML Signing certificate issue, perform the following recommended steps:</span></span>

1. <span data-ttu-id="7c5be-104">當您新增支援 SSO 的企業應用程式時，Azure 會產生名為 [SAML 簽署憑證](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications) 的憑證。</span><span class="sxs-lookup"><span data-stu-id="7c5be-104">When you add an enterprise application which supports SSO, Azure will generate a certificate which is called the [SAML Signing certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#auto-generated-certificate-for-gallery-and-non-gallery-applications).</span></span> <span data-ttu-id="7c5be-105">此憑證的到期日為 3 年。</span><span class="sxs-lookup"><span data-stu-id="7c5be-105">This certificate has an expiration date of 3 years.</span></span> <span data-ttu-id="7c5be-106">若要變更您的憑證的到期日，請參閱 [自訂您的同盟憑證的到期日，並轉用至新的憑證](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate)。</span><span class="sxs-lookup"><span data-stu-id="7c5be-106">To change the expiration date of your certificate, see [Customize the expiration date for your federation certificate and roll it over to a new certificate](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#customize-the-expiration-date-for-your-federation-certificate-and-roll-it-over-to-a-new-certificate).</span></span>
2. <span data-ttu-id="7c5be-107">Azure 會使用此憑證簽署應用程式所要求的 SAML 權杖，並將之傳送至應用程式，以取得成功的 SSO。</span><span class="sxs-lookup"><span data-stu-id="7c5be-107">Azure will use this certificate to sign the SAML tokens requested by the application and send it over to the application for a successful SSO.</span></span> <span data-ttu-id="7c5be-108">若要完成此程序，請從 Azure 入口網站下載憑證，並將之傳送至應用程式廠商以完成 SSO 程序。</span><span class="sxs-lookup"><span data-stu-id="7c5be-108">In order for this to complete, download the certificate from the Azure portal and send it to the application vendor to complete the SSO process.</span></span>

<span data-ttu-id="7c5be-109">完成此程序之後，您的應用程式將會信任此憑證，且應用程式將接受此憑證所簽署的所有 SAML 權杖。</span><span class="sxs-lookup"><span data-stu-id="7c5be-109">After this process completes your application will trust this certificate and all the SAML tokens signed by this certificate will be accepted by the application.</span></span>

3. <span data-ttu-id="7c5be-110">如果此憑證過期，請建立新憑證，將之更新至應用程式廠商，然後在 Azure 端啟動該憑證。</span><span class="sxs-lookup"><span data-stu-id="7c5be-110">If this certificate expires, create a new certificate, update it to the application vendor and then make it active on the Azure side.</span></span> <span data-ttu-id="7c5be-111">如需詳細資訊，請參閱 [更新即將到期的憑證](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire)。</span><span class="sxs-lookup"><span data-stu-id="7c5be-111">For more information, see [Renew a certificate that will soon expire](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#renew-a-certificate-that-will-soon-expire).</span></span>

> [!NOTE]
> <span data-ttu-id="7c5be-112">如果憑證過期，並不會封鎖使用者。</span><span class="sxs-lookup"><span data-stu-id="7c5be-112">If the certificate expires, the user will not be blocked.</span></span>

4. <span data-ttu-id="7c5be-113">[新增收取通知的電子郵件地址](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) 以在目前憑證到期前接收通知。</span><span class="sxs-lookup"><span data-stu-id="7c5be-113">[Add an email address for notifications](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-certificates-for-federated-single-sign-on#add-email-notification-addresses-for-certificate-expiration) to be received before the current certificate expires.</span></span>

> [!NOTE]
> <span data-ttu-id="7c5be-114">步驟 4 是選擇性步驟。</span><span class="sxs-lookup"><span data-stu-id="7c5be-114">Step-4 is an optional one.</span></span>

5. <span data-ttu-id="7c5be-115">變更應用程式的 SAML 憑證簽署選項和憑證簽署演算法。</span><span class="sxs-lookup"><span data-stu-id="7c5be-115">Change an application's SAML certificate signing options and the certificate signing algorithm.</span></span> <span data-ttu-id="7c5be-116">如需詳細資訊，請參閱 [變更憑證簽署選項和簽署演算法](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options)。</span><span class="sxs-lookup"><span data-stu-id="7c5be-116">For more information, see [Change certificate signing options and signing algorithm](https://docs.microsoft.com/azure/active-directory/manage-apps/certificate-signing-options).</span></span>

