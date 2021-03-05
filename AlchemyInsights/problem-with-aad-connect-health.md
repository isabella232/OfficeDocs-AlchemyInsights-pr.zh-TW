---
title: AAD Connect Health 的問題
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50453289"
---
# <a name="problem-with-aad-connect-health"></a><span data-ttu-id="38b64-102">AAD Connect Health 的問題</span><span class="sxs-lookup"><span data-stu-id="38b64-102">Problem with AAD Connect Health</span></span>

- <span data-ttu-id="38b64-103">確定您有權執行此作業。</span><span class="sxs-lookup"><span data-stu-id="38b64-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="38b64-104">全域管理員預設可以存取。</span><span class="sxs-lookup"><span data-stu-id="38b64-104">Global Admins have access by default.</span></span> <span data-ttu-id="38b64-105">此外，您可以使用 [角色型存取控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) ，將註冊許可權委派給投稿者。</span><span class="sxs-lookup"><span data-stu-id="38b64-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="38b64-106">確定所需端點已啟用，但由於防火牆而未封鎖。</span><span class="sxs-lookup"><span data-stu-id="38b64-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="38b64-107">如需詳細資訊，請參閱 [需求](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。</span><span class="sxs-lookup"><span data-stu-id="38b64-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="38b64-108">因為網路層對 SSL 檢查進行的輸出通訊，所以註冊可能會失敗。</span><span class="sxs-lookup"><span data-stu-id="38b64-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="38b64-109">請確認您已驗證 Azure AD Connect Health 的通知設定。</span><span class="sxs-lookup"><span data-stu-id="38b64-109">Make sure you have verified the notification settings for Azure AD Connect Health.</span></span> <span data-ttu-id="38b64-110">請複查您的設定。</span><span class="sxs-lookup"><span data-stu-id="38b64-110">Please review your setting.</span></span> <span data-ttu-id="38b64-111">本 [指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) 可協助您瞭解如何設定 Azure AD Connect health 通知的通知設定。</span><span class="sxs-lookup"><span data-stu-id="38b64-111">This [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) can help you understand how to configure the notification settings for Azure AD Connect health notifications.</span></span>
- <span data-ttu-id="38b64-112">若要深入瞭解 AAD Connect Health sync 報表及如何下載它，請參閱 [物件層級同步處理報告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。</span><span class="sxs-lookup"><span data-stu-id="38b64-112">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="38b64-113">若要疑難排解 AAD Connect 狀況警示，請遵循 [Aad Connect health 資料新鮮度警示的疑難排解指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 及常見問題的疑難排解，請參閱 [常見的 AAD connect Health 安裝問題](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。</span><span class="sxs-lookup"><span data-stu-id="38b64-113">To troubleshoot AAD Connect Health alerts, follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
