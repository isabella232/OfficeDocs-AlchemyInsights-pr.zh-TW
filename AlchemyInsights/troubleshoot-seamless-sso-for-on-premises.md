---
title: 針對內部部署無縫單一登入 (SSO) 進行疑難排解
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9370"
- "9004357"
ms.openlocfilehash: a8d14b12bfb3b02da0468eee70af26344465a2a2
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/12/2021
ms.locfileid: "50753393"
---
# <a name="troubleshoot-seamless-single-sign-on-sso-for-on-premises"></a><span data-ttu-id="ea1c7-102">針對內部部署無縫單一登入 (SSO) 進行疑難排解</span><span class="sxs-lookup"><span data-stu-id="ea1c7-102">Troubleshoot Seamless Single Sign-on (SSO) for on-premises</span></span>

<span data-ttu-id="ea1c7-103">如需解決無縫單一登入 (SSO) 問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="ea1c7-103">To resolve Seamless Single Sign-on (SSO) issues, perform the following steps:</span></span>

<span data-ttu-id="ea1c7-104">**如何換用 AZUREADSSO 電腦帳戶的 Kerberos 解密金鑰？**</span><span class="sxs-lookup"><span data-stu-id="ea1c7-104">**How can I roll over the Kerberos decryption key of the AZUREADSSO computer account?**</span></span>

<span data-ttu-id="ea1c7-105">強烈建議您至少每 30 天換用一次 Kerberos 解密金鑰。</span><span class="sxs-lookup"><span data-stu-id="ea1c7-105">We highly recommend that you roll over the Kerberos decryption key at least every 30 days.</span></span> <span data-ttu-id="ea1c7-106">如需手動執行這項操作，請參閱[如何換用 Kerberos 解密金鑰](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#)。</span><span class="sxs-lookup"><span data-stu-id="ea1c7-106">To do this manually, see [How to roll over Kerberos decryption keys](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq#).</span></span>

<span data-ttu-id="ea1c7-107">**設定無縫 SSO**</span><span class="sxs-lookup"><span data-stu-id="ea1c7-107">**Configure Seamless SSO**</span></span>

<span data-ttu-id="ea1c7-108">如需部署無縫 SSO，請遵循 [Azure Active Directory 無縫單一登入：快速入門](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys)的步驟。</span><span class="sxs-lookup"><span data-stu-id="ea1c7-108">To deploy Seamless SSO, follow the steps in [Azure Active Directory Seamless Single Sign-On: Quickstart](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-quick-start#step-5-roll-over-keys).</span></span>

<span data-ttu-id="ea1c7-109">**公告**</span><span class="sxs-lookup"><span data-stu-id="ea1c7-109">**Advisory**</span></span>

- <span data-ttu-id="ea1c7-110">[Azure Active Directory 無縫單一登入：常見問題](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - 本文說明有關 Azure Active Directory 無縫單一登入 (無縫 SSO) 的常見問題。</span><span class="sxs-lookup"><span data-stu-id="ea1c7-110">[Azure Active Directory Seamless Single Sign-On: Frequently asked questions](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso-faq) - In this article, we address frequently asked questions about Azure Active Directory Seamless Single Sign-On (Seamless SSO).</span></span> <span data-ttu-id="ea1c7-111">繼續檢查新的內容。</span><span class="sxs-lookup"><span data-stu-id="ea1c7-111">Keep checking back for new content.</span></span>
- <span data-ttu-id="ea1c7-112">[Microsoft 問與答](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - 本文提供如何提出功能要求或詢問有關無縫 SSO 技術問題的資訊。</span><span class="sxs-lookup"><span data-stu-id="ea1c7-112">[Microsoft Q&A](https://docs.microsoft.com/answers/topics/azure-ad-single-sign-on.html) - This article provides information on how to make feature requests or ask technical questions about Seamless SSO.</span></span>

<span data-ttu-id="ea1c7-113">**疑難排解**</span><span class="sxs-lookup"><span data-stu-id="ea1c7-113">**Troubleshoot**</span></span>

<span data-ttu-id="ea1c7-114">[Azure Active Directory 無縫單一登入](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) 疑難排解 - 本文可協助尋找有關 Azure Active Directory (Azure AD) 無縫單一登入 (無縫 SSO) 常見問題的疑難排解資訊。</span><span class="sxs-lookup"><span data-stu-id="ea1c7-114">[Troubleshoot Azure Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-sso) - This article helps you find troubleshooting information about common problems regarding Azure Active Directory (Azure AD) Seamless Single Sign-On (Seamless SSO).</span></span>







