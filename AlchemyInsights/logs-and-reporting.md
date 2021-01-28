---
title: 記錄與報告
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/27/2021
ms.locfileid: "50031495"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="2d4f4-102">記錄與報告</span><span class="sxs-lookup"><span data-stu-id="2d4f4-102">Logs and Reporting</span></span>

<span data-ttu-id="2d4f4-103">[Azure Active directory 報告常見問題](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) 解答有關 Azure Active Directory (azure AD) 報告常見問題的常見問題。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="2d4f4-104">如需詳細資訊，請參閱 [Azure Active Directory 報告](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="2d4f4-105">**對審計問題進行疑難排解**</span><span class="sxs-lookup"><span data-stu-id="2d4f4-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="2d4f4-106">如果您在查看某些審核活動時發生問題，但在此 [清單](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)中找不到活動，請將支援票證檔。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="2d4f4-107">如果您在租使用者中查看任何審計記錄檔時遇到問題，請提供支援憑證。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="2d4f4-108">如果您的審計活動不會立即顯示在 Azure 入口網站中，請查看延遲 [資訊](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) 和檔案 a 支援票證（如果延遲超過所記錄的延遲）。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="2d4f4-109">Azure AD 活動記錄保留</span><span class="sxs-lookup"><span data-stu-id="2d4f4-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="2d4f4-110">如果您沒有看到您所選取之日期範圍的所有審計，您可以下載最多250K 列 (從 Azure 入口網站的最近) 登入排序。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="2d4f4-111">如需詳細資訊，請參閱 [審核活動下載](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="2d4f4-112">**疑難排解登錄問題**</span><span class="sxs-lookup"><span data-stu-id="2d4f4-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="2d4f4-113">如果您有租使用者的 Azure AD Premium (P1 或 P2) 授權，您只會看到過去的30天的資料。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="2d4f4-114">登入只適用于 Azure AD Premium 承租人。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="2d4f4-115">無法使用免費或基本授權承租人。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="2d4f4-116">如果您的承租人具有「高級 P1」授權，而且您無法看到登入，請查看我們的 [延遲資訊](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) ，如果延遲超過所述的延遲，請查看支援票證。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="2d4f4-117">如果您沒有看到您所選取之日期範圍的所有登入，請注意，您最多可以下載250K 列 (從 Azure 入口網站的最近) 登入排序。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="2d4f4-118">如需詳細資訊，請參閱登 [入活動下載](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities)。</span><span class="sxs-lookup"><span data-stu-id="2d4f4-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="2d4f4-119">**疑難排解安全報告 (已標記為危險的使用者 Sign-In)**</span><span class="sxs-lookup"><span data-stu-id="2d4f4-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="2d4f4-120">已標記風險安全性報告的使用者</span><span class="sxs-lookup"><span data-stu-id="2d4f4-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="2d4f4-121">Azure Active Directory 入口網站中的危險登入報告</span><span class="sxs-lookup"><span data-stu-id="2d4f4-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="2d4f4-122">Azure Active Directory 風險事件</span><span class="sxs-lookup"><span data-stu-id="2d4f4-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
