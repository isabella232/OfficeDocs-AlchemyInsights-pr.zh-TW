---
title: 通知 AAD Connect
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
- "9003245"
- "9326"
ms.openlocfilehash: 832c9dd587cb023b5b1d87e905acb123df34237f
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897721"
---
# <a name="notification-aad-connect"></a><span data-ttu-id="99090-102">通知 AAD Connect</span><span class="sxs-lookup"><span data-stu-id="99090-102">Notification AAD Connect</span></span>

- <span data-ttu-id="99090-103">確定您有權執行此作業。</span><span class="sxs-lookup"><span data-stu-id="99090-103">Ensure you are authorized to perform the operation.</span></span> <span data-ttu-id="99090-104">全域管理員預設可以存取。</span><span class="sxs-lookup"><span data-stu-id="99090-104">Global Admins have access by default.</span></span> <span data-ttu-id="99090-105">此外，您可以使用 [角色型存取控制](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) ，將註冊許可權委派給投稿者。</span><span class="sxs-lookup"><span data-stu-id="99090-105">Additionally, you can use [Role Based Access Control](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) to delegate registration permission to Contributor.</span></span>
- <span data-ttu-id="99090-106">確定所需端點已啟用，但由於防火牆而未封鎖。</span><span class="sxs-lookup"><span data-stu-id="99090-106">Ensure the required endpoints are enabled, and not blocked due to firewall.</span></span> <span data-ttu-id="99090-107">如需詳細資訊，請參閱 [需求](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)。</span><span class="sxs-lookup"><span data-stu-id="99090-107">For details, see [requirements](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).</span></span>
- <span data-ttu-id="99090-108">因為網路層對 SSL 檢查進行的輸出通訊，所以註冊可能會失敗。</span><span class="sxs-lookup"><span data-stu-id="99090-108">Registration can fail due to outbound communication being subjected to SSL inspection by the network layer.</span></span>
- <span data-ttu-id="99090-109">請確認您已驗證 Azure AD Connect Health 的通知設定，並複查您的設定。</span><span class="sxs-lookup"><span data-stu-id="99090-109">Make sure you have verified the notification settings for Azure AD Connect Health and review your setting.</span></span> <span data-ttu-id="99090-110">若要瞭解如何設定 Azure AD Connect Health 通知的通知設定，請參閱本 [指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations)。</span><span class="sxs-lookup"><span data-stu-id="99090-110">To understand how to configure the notification settings for Azure AD Connect Health notifications, see this [guide](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations).</span></span>
- <span data-ttu-id="99090-111">若要深入瞭解 AAD Connect Health sync 報表及如何下載它，請參閱 [物件層級同步處理報告](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)。</span><span class="sxs-lookup"><span data-stu-id="99090-111">To learn more about the AAD Connect Health sync report and how to download it, see [Object level synchronization report](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).</span></span>

<span data-ttu-id="99090-112">若要疑難排解 AAD Connect Health 警示，請遵循 [有關 Aad Connect health data freshness alerts 的疑難排解指南](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) 及常見問題的疑難排解，請參閱 [常見的 AAD connect Health 安裝問題](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)。</span><span class="sxs-lookup"><span data-stu-id="99090-112">To troubleshoot AAD Connect Health Alerts follow [the troubleshooting guide for AAD Connect Health data freshness alerts](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) and for commonly asked questions, see [Common AAD Connect Health installation questions](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq).</span></span>
