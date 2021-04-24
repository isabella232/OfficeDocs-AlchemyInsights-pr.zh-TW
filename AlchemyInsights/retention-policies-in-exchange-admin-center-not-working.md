---
title: Exchange Admin Center 中的保留原則無法運作
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "308"
- "3100007"
ms.assetid: a48fd5fd-4af7-4d5f-b617-b0f9334ccaa7
ms.openlocfilehash: bb2ce7ce2405be575dfdb79d304fef690e863a4e
ms.sourcegitcommit: e9206b7bb1bf2efd2471edbf4c60c00c3607bc41
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2021
ms.locfileid: "51952219"
---
# <a name="retention-policies-in-exchange-admin-center"></a><span data-ttu-id="da14d-102">Exchange 系統管理中心中的保留原則</span><span class="sxs-lookup"><span data-stu-id="da14d-102">Retention Policies in Exchange Admin Center</span></span>

<span data-ttu-id="da14d-103">如果您想讓我們為下列所述的設定執行自動檢查，請選取此頁面頂端的 [上一步] 按鈕 <--然後輸入具有保留原則問題的使用者電子郵件地址。</span><span class="sxs-lookup"><span data-stu-id="da14d-103">If you want us to run automated checks for the settings mentioned below, select the back button <-- at the top of this page, and then enter the email address of the user who has problems with retention policies.</span></span>

<span data-ttu-id="da14d-104">如果您在 Exchange 系統管理中心中的保留原則發生問題，但未套用到信箱或專案不會移至封存信箱，請檢查下列事項：</span><span class="sxs-lookup"><span data-stu-id="da14d-104">If you have problems with retention policies in the Exchange Admin Center not applying to mailboxes or items not moving to the archive mailbox, check the following:</span></span>

<span data-ttu-id="da14d-105">**根源：**</span><span class="sxs-lookup"><span data-stu-id="da14d-105">**Root Causes:**</span></span>

- <span data-ttu-id="da14d-106">**受管理的資料夾助理** 尚未處理使用者的信箱。</span><span class="sxs-lookup"><span data-stu-id="da14d-106">**Managed Folder Assistant** has not processed the user's mailbox.</span></span> <span data-ttu-id="da14d-107">受管理的資料夾助理每隔7天會嘗試處理雲端架構組織中的每個信箱。</span><span class="sxs-lookup"><span data-stu-id="da14d-107">The Managed Folder Assistant tries to process every mailbox in your cloud-based organization once every seven days.</span></span>

  <span data-ttu-id="da14d-108">**解決方案：** 執行受管理的資料夾助理。</span><span class="sxs-lookup"><span data-stu-id="da14d-108">**Solution:** Run the Managed Folder Assistant.</span></span>

- <span data-ttu-id="da14d-109">信箱上已 **啟用** **RetentionHold** 。</span><span class="sxs-lookup"><span data-stu-id="da14d-109">**RetentionHold** has been **enabled** on the mailbox.</span></span> <span data-ttu-id="da14d-110">如果信箱已放在 RetentionHold 中，信箱的保留原則在該時段內將不會被處理。</span><span class="sxs-lookup"><span data-stu-id="da14d-110">If the mailbox has been placed on a RetentionHold, the retention policy on the mailbox will not be processed during that time.</span></span>

  <span data-ttu-id="da14d-111">**解決方案：** 檢查 [保留暫止] 設定的狀態，並視需要更新。</span><span class="sxs-lookup"><span data-stu-id="da14d-111">**Solution:** Check status of Retention Hold setting and update as needed.</span></span> <span data-ttu-id="da14d-112">如需詳細資訊，請參閱 [信箱保留](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold)功能。</span><span class="sxs-lookup"><span data-stu-id="da14d-112">For details, see [Mailbox Retention Hold](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/mailbox-retention-hold).</span></span>
 
<span data-ttu-id="da14d-113">**附注：** 如果信箱小於 10 MB，受管理的資料夾助理將不會自動處理信箱。</span><span class="sxs-lookup"><span data-stu-id="da14d-113">**Note:** If a mailbox is smaller than 10 MB, the Managed Folder Assistant will not automatically process the mailbox.</span></span>
 
<span data-ttu-id="da14d-114">如需 Exchange 系統管理中心內保留原則的詳細資訊，請參閱：</span><span class="sxs-lookup"><span data-stu-id="da14d-114">For more info on retention policies in the Exchange Admin Center, see:</span></span>

- [<span data-ttu-id="da14d-115">保留標記和保留原則</span><span class="sxs-lookup"><span data-stu-id="da14d-115">Retention tags and retention policies</span></span>](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/retention-tags-and-policies)

- <span data-ttu-id="da14d-116">[將保留原則套用至信箱，](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) 或 [新增或移除保留標記](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span><span class="sxs-lookup"><span data-stu-id="da14d-116">[Apply a retention policy to mailboxes](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy) or [Add or remove retention tags](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/add-or-remove-retention-tags)</span></span>

- [<span data-ttu-id="da14d-117">如何找出位於信箱的保留類型</span><span class="sxs-lookup"><span data-stu-id="da14d-117">How to identify the type of hold placed on a mailbox</span></span>](https://docs.microsoft.com/microsoft-365/compliance/identify-a-hold-on-an-exchange-online-mailbox)
