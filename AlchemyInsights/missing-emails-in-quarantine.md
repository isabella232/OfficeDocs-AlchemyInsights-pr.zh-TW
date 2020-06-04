---
title: 隔離區中遺失的電子郵件
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "5668"
- "9002625"
ms.openlocfilehash: 61a926c363c62bc7acb5efefe42b834f33c78eb6
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/03/2020
ms.locfileid: "44542105"
---
# <a name="missing-emails-in-quarantine"></a><span data-ttu-id="2b6e4-102">隔離中遺失的電子郵件 "</span><span class="sxs-lookup"><span data-stu-id="2b6e4-102">Missing emails in quarantine"</span></span>

<span data-ttu-id="2b6e4-103">管理員可以[查看、發行或刪除這些郵件。](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span><span class="sxs-lookup"><span data-stu-id="2b6e4-103">Administrators can [view, release, or delete these messages.](https://docs.microsoft.com/microsoft-365/security/office-365-security/manage-quarantined-messages-and-files?view=o365-worldwide)</span></span>

<span data-ttu-id="2b6e4-104">若要開啟安全性 & 規範中心，請移至 [https://protection.office.com](https://protection.office.com/) 。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-104">To open the Security & Compliance Center, go to [https://protection.office.com](https://protection.office.com/).</span></span> <span data-ttu-id="2b6e4-105">若要直接開啟 [隔離] 頁面，請移至 [https://protection.office.com/quarantine](https://protection.office.com/quarantine) 。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-105">To open the Quarantine page directly, go to [https://protection.office.com/quarantine](https://protection.office.com/quarantine).</span></span>  

<span data-ttu-id="2b6e4-106">您可以依下列值進行搜尋：</span><span class="sxs-lookup"><span data-stu-id="2b6e4-106">You can search by the following values:</span></span>  

- <span data-ttu-id="2b6e4-107">**郵件識別碼**：郵件的全域唯一識別碼。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-107">**Message ID**: The globally unique identifier of the message.</span></span> <span data-ttu-id="2b6e4-108">如果您選取清單中的訊息，[**詳細資料**] 彈出窗格中隨即會顯示 [**郵件識別碼**] 值。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-108">If you select a message in the list, the  **Message ID**  value appears in the  **Details**  flyout pane that appears.</span></span> <span data-ttu-id="2b6e4-109">系統管理員可以使用 [郵件追蹤][](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) 來尋找郵件及其對應的郵件識別碼值。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-109">Admins can use [message trace](https://docs.microsoft.com/microsoft-365/security/office-365-security/message-trace-scc?view=o365-worldwide) to find messages and their corresponding Message ID values.</span></span>
- <span data-ttu-id="2b6e4-110">**寄件者電子郵件地址**：單一寄件者的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-110">**Sender email address**: A single sender's email address.</span></span>
- <span data-ttu-id="2b6e4-111">**收件者電子郵件地址**：單一收件者的電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-111">**Recipient email address**: A single recipient's email address.</span></span>
- <span data-ttu-id="2b6e4-112">**主旨**：使用郵件的完整主旨。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-112">**Subject**: Use the entire subject of the message.</span></span> <span data-ttu-id="2b6e4-113">搜尋時不會區分大小寫。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-113">The search is not case-sensitive.</span></span>

<span data-ttu-id="2b6e4-114">輸入搜尋準則之後，請按一下 [重新整理按鈕重新整理] ![ ](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide) **Refresh**以篩選結果。  </span><span class="sxs-lookup"><span data-stu-id="2b6e4-114">After you've entered the search criteria, click  ![Refresh button](https://docs.microsoft.com/microsoft-365/media/scc-quarantine-refresh.png?view=o365-worldwide)  **Refresh**  to filter the results.</span></span>

<span data-ttu-id="2b6e4-115">您用來在隔離區中查看及管理郵件和檔案的 Cmdlet 如下：</span><span class="sxs-lookup"><span data-stu-id="2b6e4-115">The cmdlets you use to view and manages messages and files in quarantine are:</span></span>
- [<span data-ttu-id="2b6e4-116">Delete-Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="2b6e4-116">Delete-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/delete-quarantinemessage)
- [<span data-ttu-id="2b6e4-117">Export-Get-quarantinemessage</span><span class="sxs-lookup"><span data-stu-id="2b6e4-117">Export-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/export-quarantinemessage)
- [<span data-ttu-id="2b6e4-118">Get-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="2b6e4-118">Get-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/get-quarantinemessage)
- <span data-ttu-id="2b6e4-119">[預覽-get-quarantinemessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage)：請注意，此 Cmdlet 只適用于 SharePoint Online、商務 OneDrive 或小組的 ATP 中的電子郵件，而非惡意程式碼檔案。</span><span class="sxs-lookup"><span data-stu-id="2b6e4-119">[Preview-QuarantineMessage](https://docs.microsoft.com/powershell/module/exchange/preview-quarantinemessage): Note that this cmdlet is only for messages, not malware files from ATP for SharePoint Online, OneDrive for Business, or Teams.</span></span>
- [<span data-ttu-id="2b6e4-120">Release-QuarantineMessage</span><span class="sxs-lookup"><span data-stu-id="2b6e4-120">Release-QuarantineMessage</span></span>](https://docs.microsoft.com/powershell/module/exchange/release-quarantinemessage)