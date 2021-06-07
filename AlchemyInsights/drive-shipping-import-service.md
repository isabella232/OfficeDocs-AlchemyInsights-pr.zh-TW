---
title: Microsoft 365 匯入服務中的磁碟機寄送
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2021
ms.locfileid: "52721675"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="a7e76-102">Microsoft 365 匯入服務中的磁碟機寄送</span><span class="sxs-lookup"><span data-stu-id="a7e76-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="a7e76-103">使用磁碟機寄送的方式是透過複製 PST 至硬碟，然後運送硬碟至 Microsoft。</span><span class="sxs-lookup"><span data-stu-id="a7e76-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="a7e76-104">若要啟動此工具：</span><span class="sxs-lookup"><span data-stu-id="a7e76-104">To start the job:</span></span>

1. <span data-ttu-id="a7e76-105">在 [Microsoft 365 合規性中心] 的 **[資訊控管]** 底下，選取 **[匯入]**。</span><span class="sxs-lookup"><span data-stu-id="a7e76-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="a7e76-106">選取 **選擇匯入工作類型**，然後選取 **下一步**。</span><span class="sxs-lookup"><span data-stu-id="a7e76-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="a7e76-107">若要查看此匯入選項的步驟，請選取 **將硬碟寄送到我們的其中一個實體位置**。</span><span class="sxs-lookup"><span data-stu-id="a7e76-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="a7e76-108">以下是一些要記住的事項：</span><span class="sxs-lookup"><span data-stu-id="a7e76-108">Here are some things to remember:</span></span>

- <span data-ttu-id="a7e76-109">您必須在 Exchange Online 中獲派信箱匯入匯出角色，才能將 PST 檔案匯入 Microsoft 365 信箱。</span><span class="sxs-lookup"><span data-stu-id="a7e76-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="a7e76-110">如果 PST 大於 20GB，效能可能會受到影響。</span><span class="sxs-lookup"><span data-stu-id="a7e76-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="a7e76-111">只支援 2.5 吋固態硬碟 (SSD)，或是 2.5 吋或 3.5 吋 SATA II/III 內接式硬碟。</span><span class="sxs-lookup"><span data-stu-id="a7e76-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="a7e76-112">包含 PST 檔案的硬碟必須使用 BitLocker 進行加密。</span><span class="sxs-lookup"><span data-stu-id="a7e76-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="a7e76-113">使用磁碟機寄送以將 PST 檔案匯入到 Microsoft 365 信箱的成本，是每 GB 的資料 $2 USD。</span><span class="sxs-lookup"><span data-stu-id="a7e76-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="a7e76-114">如需使用磁碟機寄送方式匯入 PST 的其他資訊，請參閱 [使用磁碟機寄送以匯入貴組織的 PST 檔案](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)。</span><span class="sxs-lookup"><span data-stu-id="a7e76-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>