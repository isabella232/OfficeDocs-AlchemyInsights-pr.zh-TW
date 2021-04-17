---
title: 取消保留
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 6b27344b43aa5c20d64d148ff164be805f3b5ef8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819683"
---
# <a name="cancelling-reservation"></a><span data-ttu-id="be959-102">取消保留</span><span class="sxs-lookup"><span data-stu-id="be959-102">Cancelling Reservation</span></span>

- <span data-ttu-id="be959-103">**自助**：您可以自己使用 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)取消或交換保留執行個體。</span><span class="sxs-lookup"><span data-stu-id="be959-103">**Self-service:** You can cancel or exchange a reserved instance yourself using [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="be959-104">選取 [保留] 並按一下 [退款] 或 [交換]。</span><span class="sxs-lookup"><span data-stu-id="be959-104">Select the reservation and click on refund or exchange.</span></span> <span data-ttu-id="be959-105">請注意，您必須有保留訂單的擁有者權限才能交換或退款。</span><span class="sxs-lookup"><span data-stu-id="be959-105">Note that you must have owner access on the Reservation Order to exchange or refund.</span></span> <span data-ttu-id="be959-106">僅存取保留將不允許您繼續退款或兌換。</span><span class="sxs-lookup"><span data-stu-id="be959-106">Access to only the Reservation will not let you proceed with refund or exchange.</span></span> <span data-ttu-id="be959-107">要求保留訂單擁有者向您授予對保留訂單的存取權限</span><span class="sxs-lookup"><span data-stu-id="be959-107">Ask the Reservation Order owner to give you owner access to the Reservation Order</span></span>
- <span data-ttu-id="be959-108">**交換原則：** 您可以將一個保留與另一個相同類型的保留交換 – 保留交換 **沒有負面影響**。</span><span class="sxs-lookup"><span data-stu-id="be959-108">**Exchange policy:** You can exchange a reservation for another reservation of the same type – there are **no penalties** on reservation exchange.</span></span> <span data-ttu-id="be959-109">新保留的總承諾金額應大於兌換保留的退款金額和未來每月付款的總和 (如適用)</span><span class="sxs-lookup"><span data-stu-id="be959-109">The total commitment with new reservation should be greater than the sum of exchanged reservation’s refund amount and the future monthly payments (if applicable)</span></span>
- <span data-ttu-id="be959-110">**退款原則**：在 12 個月的運行視窗內，退款和取消的未來付款總額不得超過 50000 美元。</span><span class="sxs-lookup"><span data-stu-id="be959-110">**Refund policy:** Sum of refund and the cancelled future payments cannot exceed $50,000 USD in a 12-month rolling window.</span></span> <span data-ttu-id="be959-111">我們 **目前不收取任何退款罰款**，但可以在以後退款時收取</span><span class="sxs-lookup"><span data-stu-id="be959-111">We are **currently not charging any penalty** on refunds but could charge it on future refunds</span></span>  
    <span data-ttu-id="be959-112">**例外：** 美國政府企業協定客戶不可用自助交換和取消功能</span><span class="sxs-lookup"><span data-stu-id="be959-112">**Exceptions:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers</span></span>
- <span data-ttu-id="be959-113">**API / PS / CLI** 不支援取消和退款 [Azure 保留的自助兌換和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="be959-113">**API / PS / CLI** support is not available for cancellation and refunds [Self-service exchanges and refunds for Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="be959-114">美國政府企業協定客戶不可用自助交換和取消功能。</span><span class="sxs-lookup"><span data-stu-id="be959-114">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="be959-115">支援其他美國政府訂閱類型，包括隨付隨用和 CSP</span><span class="sxs-lookup"><span data-stu-id="be959-115">Other US Government subscription types including Pay-As-You-Go and CSP are supported</span></span>

<span data-ttu-id="be959-116">深入了解：[如何處理退貨和換貨交易](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)</span><span class="sxs-lookup"><span data-stu-id="be959-116">Learn more : [How return and exchange transactions are processed](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)</span></span>  
<span data-ttu-id="be959-117">深入了解：[Exchange 和交換原則](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)</span><span class="sxs-lookup"><span data-stu-id="be959-117">Learn more : [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)</span></span>  
<span data-ttu-id="be959-118">其他問題： [造訪保留執行個體文件](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="be959-118">Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="be959-119">**交換現有的保留執行個體 (自助)**</span><span class="sxs-lookup"><span data-stu-id="be959-119">**Exchange an existing reserved instance (Self-service)**</span></span>

<span data-ttu-id="be959-120">您可以將一個保留換成另一個相同類型的保留。</span><span class="sxs-lookup"><span data-stu-id="be959-120">You can exchange a reservation for another reservation of the same type.</span></span> <span data-ttu-id="be959-121">如果您不再需要保留，您還可以退款 (最高每年 50000 美元)。</span><span class="sxs-lookup"><span data-stu-id="be959-121">You can also refund a reservation, up to $50,000 USD per year, if you no longer need it.</span></span> <span data-ttu-id="be959-122">美國政府企業協定客戶不可用自助交換和取消功能。</span><span class="sxs-lookup"><span data-stu-id="be959-122">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="be959-123">支援其他美國政府訂閱類型，包括隨付隨用和 CSP。</span><span class="sxs-lookup"><span data-stu-id="be959-123">Other US Government subscription types including Pay-As-You-Go and CSP are supported.</span></span> <span data-ttu-id="be959-124">您必須具有保留訂單上的擁有者權限才能兌換或退款現有保留。</span><span class="sxs-lookup"><span data-stu-id="be959-124">You must have owner access on the Reservation Order to exchange or refund an existing reservation.</span></span>

<span data-ttu-id="be959-125">以下步驟將指導完成交易的過程</span><span class="sxs-lookup"><span data-stu-id="be959-125">The following steps will guide on the procedure to complete the transaction</span></span>

1. <span data-ttu-id="be959-126">登入您的 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。</span><span class="sxs-lookup"><span data-stu-id="be959-126">Log in to your [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="be959-127">選取您要退款的保留，然後按一下 **[交換]**</span><span class="sxs-lookup"><span data-stu-id="be959-127">Select the reservations that you want to refund and click **Exchange**</span></span>
2. <span data-ttu-id="be959-128">選擇要購買的 VM 產品並輸入數量。</span><span class="sxs-lookup"><span data-stu-id="be959-128">Select the VM product that you want to purchase and type a quantity.</span></span> <span data-ttu-id="be959-129">確保新的購買總額大於退貨總額[在購買之前確定正確的大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)</span><span class="sxs-lookup"><span data-stu-id="be959-129">Make sure that the new purchase total is more than the return total [Determine the right size before you purchase](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)</span></span>
3. <span data-ttu-id="be959-130">檢閱 並完成交易</span><span class="sxs-lookup"><span data-stu-id="be959-130">Review and complete the transaction</span></span>

<span data-ttu-id="be959-131">**保留執行個體退款**</span><span class="sxs-lookup"><span data-stu-id="be959-131">**Refund for a reserved instance**</span></span>

<span data-ttu-id="be959-132">若要退款保留，請移至 **[保留詳細資料]** 然後按一下 **[退款]**</span><span class="sxs-lookup"><span data-stu-id="be959-132">To refund a reservation, go to **Reservation Details** and click **Refund**</span></span>

<span data-ttu-id="be959-133">**專業等級退款：**</span><span class="sxs-lookup"><span data-stu-id="be959-133">**Pro-rated refund:**</span></span>

<span data-ttu-id="be959-134">**退款和兌換的專業比例和最低要求範例**</span><span class="sxs-lookup"><span data-stu-id="be959-134">**Pro-ration and minimum requirement examples for refund and exchange**</span></span>  
<span data-ttu-id="be959-135">預先保留範例：</span><span class="sxs-lookup"><span data-stu-id="be959-135">Upfront reservation example:</span></span>

- <span data-ttu-id="be959-136">你在 1 月 1 日以 120 美元購買一年期的 RI</span><span class="sxs-lookup"><span data-stu-id="be959-136">You purchase a one-year term RI for $120 on January 1</span></span>
- <span data-ttu-id="be959-137">您想在 4 月 7 日退換這個保留嗎</span><span class="sxs-lookup"><span data-stu-id="be959-137">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="be959-138">由於保留已經進行 了97 天，您將獲得 (1-97/365)\*120 美元。</span><span class="sxs-lookup"><span data-stu-id="be959-138">Since the reservation has been live for 97 days, you will get (1-97/365) \* $120 back.</span></span> <span data-ttu-id="be959-139">(i.e. $88.1)。</span><span class="sxs-lookup"><span data-stu-id="be959-139">(i.e. $88.1).</span></span> <span data-ttu-id="be959-140">目前退款沒有罰款</span><span class="sxs-lookup"><span data-stu-id="be959-140">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="be959-141">如果換貨，您的新購買金額應大於 88.1 美元</span><span class="sxs-lookup"><span data-stu-id="be959-141">If exchanging, your new purchase should be greater than $88.1</span></span>
- <span data-ttu-id="be959-142">目前退款沒有罰款</span><span class="sxs-lookup"><span data-stu-id="be959-142">There is no penalty on refunds currently</span></span>

<span data-ttu-id="be959-143">**計費計畫保留範例：**</span><span class="sxs-lookup"><span data-stu-id="be959-143">**Billing plan reservation example:**</span></span>

- <span data-ttu-id="be959-144">你以每月 10 美元的價格購買一年期定期 RI</span><span class="sxs-lookup"><span data-stu-id="be959-144">You purchase a one-year term RI for $10 per month</span></span>
- <span data-ttu-id="be959-145">您想在 4 月 7 日退換這個保留</span><span class="sxs-lookup"><span data-stu-id="be959-145">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="be959-146">由於最後一次付款在 7 天前，你將得到 (1-7/31)\*10 美元。</span><span class="sxs-lookup"><span data-stu-id="be959-146">Since the last payment happened 7 days, you will get (1-7/31) \* $10 back.</span></span> <span data-ttu-id="be959-147">(例如 $7.74)</span><span class="sxs-lookup"><span data-stu-id="be959-147">(i.e. $7.74)</span></span>
- <span data-ttu-id="be959-148">取消的未來付款是 80 美元。</span><span class="sxs-lookup"><span data-stu-id="be959-148">The future payments cancelled are $ 80.</span></span> <span data-ttu-id="be959-149">目前退款沒有罰款</span><span class="sxs-lookup"><span data-stu-id="be959-149">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="be959-150">這次取消將從您的 50000 美元退款限額中扣除 87.74 美元</span><span class="sxs-lookup"><span data-stu-id="be959-150">This cancellation will deduct $87.74 from you’re the $50,000 refund limit</span></span>
- <span data-ttu-id="be959-151">如果交換，新購買的總價值應大於 87.74 美元</span><span class="sxs-lookup"><span data-stu-id="be959-151">If exchanging, the total value of new purchase should be greater than $87.74</span></span>

<span data-ttu-id="be959-152">**建議的文件**</span><span class="sxs-lookup"><span data-stu-id="be959-152">**Recommended Documents**</span></span>

- [<span data-ttu-id="be959-153">如何處理退貨和換貨交易</span><span class="sxs-lookup"><span data-stu-id="be959-153">How return and exchange transactions are processed</span></span>](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [<span data-ttu-id="be959-154">交換和退款原則</span><span class="sxs-lookup"><span data-stu-id="be959-154">Exchange and Refund policies</span></span>](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)