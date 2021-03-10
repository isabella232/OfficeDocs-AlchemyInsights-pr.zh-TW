---
title: 密碼記錄檔
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
- "9361"
- "9003259"
ms.openlocfilehash: ed151b436fa2043c610931deeb74a202af88fcf4
ms.sourcegitcommit: 226fe97678b6be215eda0c278399f8be9be525c1
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50523081"
---
# <a name="password-logs"></a><span data-ttu-id="f626b-102">密碼記錄檔</span><span class="sxs-lookup"><span data-stu-id="f626b-102">Password logs</span></span>

<span data-ttu-id="f626b-103">**我在存取密碼重設稽核記錄檔時發生問題**</span><span class="sxs-lookup"><span data-stu-id="f626b-103">**I'm having problems accessing password reset audit logs**</span></span>

<span data-ttu-id="f626b-104">若要疑難排解存取密碼重設稽核記錄檔的問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="f626b-104">To troubleshoot issues regarding access to password reset audit logs, perform the following step:</span></span>

<span data-ttu-id="f626b-105">確保您獲得授權檢視稽核記錄檔。</span><span class="sxs-lookup"><span data-stu-id="f626b-105">Ensure you are authorized to view audit logs.</span></span> 

<span data-ttu-id="f626b-106">只有下列角色獲得授權：</span><span class="sxs-lookup"><span data-stu-id="f626b-106">Only the following roles are authorized:</span></span>
 - <span data-ttu-id="f626b-107">全域管理員</span><span class="sxs-lookup"><span data-stu-id="f626b-107">Global administrator</span></span>
 - <span data-ttu-id="f626b-108">安全性系統管理員</span><span class="sxs-lookup"><span data-stu-id="f626b-108">Security administrator</span></span>
 - <span data-ttu-id="f626b-109">安全性讀取者</span><span class="sxs-lookup"><span data-stu-id="f626b-109">Security reader</span></span>

<span data-ttu-id="f626b-110">**我想要查看從最初部署開始的所有密碼重設稽核事件**</span><span class="sxs-lookup"><span data-stu-id="f626b-110">**I want to see all password reset audit events from the time I initially deployed**</span></span>

<span data-ttu-id="f626b-111">過去 30 天的報告最多會儲存 120,000 個密碼重設/註冊事件。</span><span class="sxs-lookup"><span data-stu-id="f626b-111">Up to 120,000 password reset/registration events are stored in the reports of the last 30 days.</span></span> <span data-ttu-id="f626b-112">下載 CSV 時，此上限會套用至 UI。</span><span class="sxs-lookup"><span data-stu-id="f626b-112">This maximum limit applies to the UI when downloading the CSV.</span></span> <span data-ttu-id="f626b-113">可透過 PowerShell 使用 1 百萬個事件。</span><span class="sxs-lookup"><span data-stu-id="f626b-113">1 million events are available through PowerShell.</span></span>
<span data-ttu-id="f626b-114">如需詳細資訊，請參閱以下連結：</span><span class="sxs-lookup"><span data-stu-id="f626b-114">For more information, see the links below:</span></span>

- [<span data-ttu-id="f626b-115">來自 Azure AD 報告和事件 API 的自助密碼重設事件</span><span class="sxs-lookup"><span data-stu-id="f626b-115">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="f626b-116">如何使用 PowerShell 快速下載密碼重設註冊事件</span><span class="sxs-lookup"><span data-stu-id="f626b-116">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)

<span data-ttu-id="f626b-117">**我想要深入瞭解有關密碼重設報告功能**</span><span class="sxs-lookup"><span data-stu-id="f626b-117">**I want to understand more about password reset reporting capabilities**</span></span>

<span data-ttu-id="f626b-118">在 **使用者和群組** 下方，檢查誰在 Microsoft Azure 入口網站使用 Azure AD 密碼重設稽核記錄檔進行註冊或重設密碼。</span><span class="sxs-lookup"><span data-stu-id="f626b-118">Check who is registering for or resetting passwords with Azure AD password reset audit logs in the Azure portal under **Users and groups**.</span></span>
<span data-ttu-id="f626b-119">如需詳細資訊，請參閱下列連結：</span><span class="sxs-lookup"><span data-stu-id="f626b-119">For more information, see the following links:</span></span>

- [<span data-ttu-id="f626b-120">密碼重設報告概觀</span><span class="sxs-lookup"><span data-stu-id="f626b-120">Password reset reports overview</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="f626b-121">如何在 Microsoft Azure 入口網站中檢視密碼重設報告</span><span class="sxs-lookup"><span data-stu-id="f626b-121">How to view password reset reports in the Azure portal</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="f626b-122">來自 Azure AD 報告和事件 API 的自助密碼重設事件</span><span class="sxs-lookup"><span data-stu-id="f626b-122">Self-service password reset events from the Azure AD Reports and Events API</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)
- [<span data-ttu-id="f626b-123">如何使用 PowerShell 快速下載密碼重設註冊事件</span><span class="sxs-lookup"><span data-stu-id="f626b-123">How to download password reset registration events quickly with PowerShell</span></span>](https://docs.microsoft.com/azure/active-directory/authentication/howto-sspr-reporting)


