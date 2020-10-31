---
title: 保留執行個體的購買帳單
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 6cdcb5af27a475cc838eb434ff025eb18356360c
ms.sourcegitcommit: 1ac3474897abb7c4969e222f934294e05f468536
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/30/2020
ms.locfileid: "48815979"
---
# <a name="billing-for-reserved-instance-purchase"></a><span data-ttu-id="43d66-102">保留執行個體的購買帳單</span><span class="sxs-lookup"><span data-stu-id="43d66-102">Billing for Reserved Instance purchase</span></span>

<span data-ttu-id="43d66-103">系統會依照您在購買時所選訂閱的付款條件，對保留執行個體之購買進行收費。</span><span class="sxs-lookup"><span data-stu-id="43d66-103">The reserved instance purchase is charged to the payment method tied to the subscription that you select at the time of purchase.</span></span> <span data-ttu-id="43d66-104">訂閱類型必須是企業合約 (優惠號碼： MS-AZR-0017P)、隨用隨付 (優惠號碼： MS-AZR-0003P)、Microsoft 客戶合約或 CSP。</span><span class="sxs-lookup"><span data-stu-id="43d66-104">The subscription type must be an enterprise agreement (offer number: MS-AZR-0017P), Pay-As-You-Go (offer number: MS-AZR-0003P), Microsoft Customer Agreement or CSP.</span></span>

- <span data-ttu-id="43d66-105">如果是企業版訂閱，費用會從登記的金錢履約承諾餘額中扣減，或以超額進行收費</span><span class="sxs-lookup"><span data-stu-id="43d66-105">For an enterprise subscription, the charges are deducted from the enrollment's monetary commitment balance or charged as overage</span></span>
- <span data-ttu-id="43d66-106">針對 [隨用隨付] 訂閱，會以信用卡或訂閱上的發票付款方式進行收費</span><span class="sxs-lookup"><span data-stu-id="43d66-106">For Pay-As-You-Go subscription, the charges are billed to the credit card or invoice payment method on the subscription</span></span>

<span data-ttu-id="43d66-107">**取消保留**</span><span class="sxs-lookup"><span data-stu-id="43d66-107">**Cancelling Reservation**</span></span>

- <span data-ttu-id="43d66-108">**自助** ：您可以自己使用 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)取消或交換保留執行個體。</span><span class="sxs-lookup"><span data-stu-id="43d66-108">**Self-service:** You can cancel or exchange a reserved instance yourself using [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="43d66-109">選取 [保留] 並按一下 [退款] 或 [交換]。</span><span class="sxs-lookup"><span data-stu-id="43d66-109">Select the reservation and click on refund or exchange.</span></span> <span data-ttu-id="43d66-110">請注意，您必須有保留訂單的擁有者權限才能交換或退款。</span><span class="sxs-lookup"><span data-stu-id="43d66-110">Note that you must have owner access on the Reservation Order to exchange or refund.</span></span> <span data-ttu-id="43d66-111">僅存取保留將不允許您繼續退款或兌換。</span><span class="sxs-lookup"><span data-stu-id="43d66-111">Access to only the Reservation will not let you proceed with refund or exchange.</span></span> <span data-ttu-id="43d66-112">要求保留訂單擁有者向您授予對保留訂單的存取權限</span><span class="sxs-lookup"><span data-stu-id="43d66-112">Ask the Reservation Order owner to give you owner access to the Reservation Order</span></span>
- <span data-ttu-id="43d66-113">**交換原則：** 您可以將一個保留與另一個相同類型的保留交換 – 保留交換 **沒有負面影響** 。</span><span class="sxs-lookup"><span data-stu-id="43d66-113">**Exchange policy:** You can exchange a reservation for another reservation of the same type – there are **no penalties** on reservation exchange.</span></span> <span data-ttu-id="43d66-114">新保留的總承諾金額應大於兌換保留的退款金額和未來每月付款的總和 (如適用)</span><span class="sxs-lookup"><span data-stu-id="43d66-114">The total commitment with new reservation should be greater than the sum of exchanged reservation’s refund amount and the future monthly payments (if applicable)</span></span>
- <span data-ttu-id="43d66-115">**退款原則** ：在 12 個月的運行視窗內，退款和取消的未來付款總額不得超過 50000 美元。</span><span class="sxs-lookup"><span data-stu-id="43d66-115">**Refund policy:** Sum of refund and the cancelled future payments cannot exceed $50,000 USD in a 12-month rolling window.</span></span> <span data-ttu-id="43d66-116">我們 **目前不收取任何退款罰款** ，但可以在以後退款時收取</span><span class="sxs-lookup"><span data-stu-id="43d66-116">We are **currently not charging any penalty** on refunds but could charge it on future refunds</span></span>

<span data-ttu-id="43d66-117">**例外：** 美國政府企業協定客戶不可用自助交換和取消功能</span><span class="sxs-lookup"><span data-stu-id="43d66-117">**Exceptions:** Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers</span></span>

- <span data-ttu-id="43d66-118">**API / PS / CLI** 不支援取消和退款 [Azure 保留的自助兌換和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="43d66-118">**API / PS / CLI** support is not available for cancellation and refunds [Self-service exchanges and refunds for Azure Reservations](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="43d66-119">美國政府企業協定客戶不可用自助交換和取消功能。</span><span class="sxs-lookup"><span data-stu-id="43d66-119">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="43d66-120">支援其他美國政府訂閱類型，包括隨付隨用和 CSP</span><span class="sxs-lookup"><span data-stu-id="43d66-120">Other US Government subscription types including Pay-As-You-Go and CSP are supported</span></span>

<span data-ttu-id="43d66-121">深入瞭解：[如何處理傳回和 exchange 交易](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)：深入瞭解： [exchange 及退款原則](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)其他問題：[就診保留實例](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)檔</span><span class="sxs-lookup"><span data-stu-id="43d66-121">Learn more : [How return and exchange transactions are processed](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed) Learn more : [Exchange and Refund policies](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies) Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="43d66-122">**交換現有的保留執行個體 (自助)**</span><span class="sxs-lookup"><span data-stu-id="43d66-122">**Exchange an existing reserved instance (Self-service)**</span></span>

<span data-ttu-id="43d66-123">您可以將一個保留換成另一個相同類型的保留。</span><span class="sxs-lookup"><span data-stu-id="43d66-123">You can exchange a reservation for another reservation of the same type.</span></span> <span data-ttu-id="43d66-124">如果您不再需要保留，您還可以退款 (最高每年 50000 美元)。</span><span class="sxs-lookup"><span data-stu-id="43d66-124">You can also refund a reservation, up to $50,000 USD per year, if you no longer need it.</span></span> <span data-ttu-id="43d66-125">美國政府企業協定客戶不可用自助交換和取消功能。</span><span class="sxs-lookup"><span data-stu-id="43d66-125">Self-service exchange and cancel capability isn't available for US Government Enterprise Agreement customers.</span></span> <span data-ttu-id="43d66-126">支援其他美國政府訂閱類型，包括隨付隨用和 CSP。</span><span class="sxs-lookup"><span data-stu-id="43d66-126">Other US Government subscription types including Pay-As-You-Go and CSP are supported.</span></span> <span data-ttu-id="43d66-127">您必須具有保留訂單上的擁有者權限才能兌換或退款現有保留。</span><span class="sxs-lookup"><span data-stu-id="43d66-127">You must have owner access on the Reservation Order to exchange or refund an existing reservation.</span></span>

<span data-ttu-id="43d66-128">以下步驟將指導完成交易的過程</span><span class="sxs-lookup"><span data-stu-id="43d66-128">The following steps will guide on the procedure to complete the transaction</span></span>

<span data-ttu-id="43d66-129">1. 登入 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。</span><span class="sxs-lookup"><span data-stu-id="43d66-129">1.Log in to your [Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade).</span></span> <span data-ttu-id="43d66-130">選取您要退款的預約，然後按一下 [ **Exchange** 2]。選取您要購買的 VM 產品並輸入數量。</span><span class="sxs-lookup"><span data-stu-id="43d66-130">Select the reservations that you want to refund and click **Exchange** 2.Select the VM product that you want to purchase and type a quantity.</span></span> <span data-ttu-id="43d66-131">請確定新的購買合計超過返還的上限 [決定您購買之前的正確大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)。</span><span class="sxs-lookup"><span data-stu-id="43d66-131">Make sure that the new purchase total is more than the return total [Determine the right size before you purchase](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy).</span></span>
<span data-ttu-id="43d66-132">3. 複查並完成交易</span><span class="sxs-lookup"><span data-stu-id="43d66-132">3.Review and complete the transaction</span></span>

<span data-ttu-id="43d66-133">**保留執行個體退款**</span><span class="sxs-lookup"><span data-stu-id="43d66-133">**Refund for a reserved instance**</span></span>

<span data-ttu-id="43d66-134">若要退款保留，請移至 **[保留詳細資料]** 然後按一下 **[退款]**</span><span class="sxs-lookup"><span data-stu-id="43d66-134">To refund a reservation, go to **Reservation Details** and click **Refund**</span></span>

<span data-ttu-id="43d66-135">**專業等級退款：**</span><span class="sxs-lookup"><span data-stu-id="43d66-135">**Pro-rated refund:**</span></span>

<span data-ttu-id="43d66-136">**退款和 exchange 的 Pro-ration 和最低需求範例** 前期保留範例：</span><span class="sxs-lookup"><span data-stu-id="43d66-136">**Pro-ration and minimum requirement examples for refund and exchange** Upfront reservation example:</span></span>

- <span data-ttu-id="43d66-137">你在 1 月 1 日以 120 美元購買一年期的 RI</span><span class="sxs-lookup"><span data-stu-id="43d66-137">You purchase a one-year term RI for $120 on January 1</span></span>
- <span data-ttu-id="43d66-138">您想在 4 月 7 日退換這個保留嗎</span><span class="sxs-lookup"><span data-stu-id="43d66-138">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="43d66-139">由於保留已經進行 了97 天，您將獲得 (1-97/365)\*120 美元。</span><span class="sxs-lookup"><span data-stu-id="43d66-139">Since the reservation has been live for 97 days, you will get (1-97/365) \* $120 back.</span></span> <span data-ttu-id="43d66-140">(i.e. $88.1)。</span><span class="sxs-lookup"><span data-stu-id="43d66-140">(i.e. $88.1).</span></span> <span data-ttu-id="43d66-141">目前退款沒有罰款</span><span class="sxs-lookup"><span data-stu-id="43d66-141">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="43d66-142">如果換貨，您的新購買金額應大於 88.1 美元</span><span class="sxs-lookup"><span data-stu-id="43d66-142">If exchanging, your new purchase should be greater than $88.1</span></span>
- <span data-ttu-id="43d66-143">目前退款沒有罰款</span><span class="sxs-lookup"><span data-stu-id="43d66-143">There is no penalty on refunds currently</span></span>

<span data-ttu-id="43d66-144">**計費計畫保留範例：**</span><span class="sxs-lookup"><span data-stu-id="43d66-144">**Billing plan reservation example:**</span></span>

- <span data-ttu-id="43d66-145">你以每月 10 美元的價格購買一年期定期 RI</span><span class="sxs-lookup"><span data-stu-id="43d66-145">You purchase a one-year term RI for $10 per month</span></span>
- <span data-ttu-id="43d66-146">您想在 4 月 7 日退換這個保留</span><span class="sxs-lookup"><span data-stu-id="43d66-146">On April 7th you want to refund or exchange this reservation</span></span>
- <span data-ttu-id="43d66-147">由於最後一次付款在 7 天前，你將得到 (1-7/31)\*10 美元。</span><span class="sxs-lookup"><span data-stu-id="43d66-147">Since the last payment happened 7 days, you will get (1-7/31) \* $10 back.</span></span> <span data-ttu-id="43d66-148">(例如 $7.74)</span><span class="sxs-lookup"><span data-stu-id="43d66-148">(i.e. $7.74)</span></span>
- <span data-ttu-id="43d66-149">取消的未來付款是 80 美元。</span><span class="sxs-lookup"><span data-stu-id="43d66-149">The future payments cancelled are $ 80.</span></span> <span data-ttu-id="43d66-150">目前退款沒有罰款</span><span class="sxs-lookup"><span data-stu-id="43d66-150">There is currently no penalty on refunds</span></span>
- <span data-ttu-id="43d66-151">這次取消將從您的 50000 美元退款限額中扣除 87.74 美元</span><span class="sxs-lookup"><span data-stu-id="43d66-151">This cancellation will deduct $87.74 from you’re the $50,000 refund limit</span></span>
- <span data-ttu-id="43d66-152">如果交換，新購買的總價值應大於 87.74 美元</span><span class="sxs-lookup"><span data-stu-id="43d66-152">If exchanging, the total value of new purchase should be greater than $87.74</span></span>

<span data-ttu-id="43d66-153">**無法查看最後一個計費期間的發票**</span><span class="sxs-lookup"><span data-stu-id="43d66-153">**Unable to see invoice for the last billing period**</span></span>

<span data-ttu-id="43d66-154">您可能不會看到發票的某些可能原因：</span><span class="sxs-lookup"><span data-stu-id="43d66-154">Some possible reasons you might not see an invoice:</span></span>

- <span data-ttu-id="43d66-155">您的訂閱具有每月的信用金額，但您的訂閱並未超過，或者您有免費試用版。</span><span class="sxs-lookup"><span data-stu-id="43d66-155">You have a monthly credit amount with your subscription that you didn't exceed or you have a Free Trial.</span></span> <span data-ttu-id="43d66-156">只有當您欠付金額時才產生發票</span><span class="sxs-lookup"><span data-stu-id="43d66-156">An invoice is only generated when you owe money</span></span>
- <span data-ttu-id="43d66-157">從您訂閱 Azure 的當日起不到30天的時間</span><span class="sxs-lookup"><span data-stu-id="43d66-157">It's less than 30 days from the day you subscribed to Azure</span></span>
- <span data-ttu-id="43d66-158">尚未產生發票。</span><span class="sxs-lookup"><span data-stu-id="43d66-158">The invoice isn't generated yet.</span></span> <span data-ttu-id="43d66-159">等到帳單期限結束</span><span class="sxs-lookup"><span data-stu-id="43d66-159">Wait until the end of the billing period</span></span>
- <span data-ttu-id="43d66-160">如果您不是帳戶管理員，可能無法使用舊版發票</span><span class="sxs-lookup"><span data-stu-id="43d66-160">If you're not the Account Administrator, older invoices may not be available to you</span></span>

<span data-ttu-id="43d66-161">**從 Azure 入口網站下載您的發票 ( .pdf)**</span><span class="sxs-lookup"><span data-stu-id="43d66-161">**Download your invoice from Azure portal (.pdf)**</span></span>

- <span data-ttu-id="43d66-162">從 Azure 入口網站的 [ [訂閱](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ] 頁面中，選取您的訂閱，以 [供具有發票存取權的使用者使用](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="43d66-162">Select your subscription from the [Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) page in Azure portal as [a user with access to invoices](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>
- <span data-ttu-id="43d66-163">選取 **發票**</span><span class="sxs-lookup"><span data-stu-id="43d66-163">Select **Invoices**</span></span>
- <span data-ttu-id="43d66-164">按一下 [ **下載發票** ] 以查看您的 PDF 發票的副本。</span><span class="sxs-lookup"><span data-stu-id="43d66-164">Click **Download Invoice** to view a copy of your PDF invoice.</span></span> <span data-ttu-id="43d66-165">如果 **無法使用** ，請參閱 [為什麼我看不到最後計費期間的發票？](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span><span class="sxs-lookup"><span data-stu-id="43d66-165">If it says **Not available** , see [Why don't I see an invoice for the last billing period?](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)</span></span>

<span data-ttu-id="43d66-166">**透過電子郵件 ( .pdf) 接收您的發票**</span><span class="sxs-lookup"><span data-stu-id="43d66-166">**Receive your invoice in email (.pdf)**</span></span>

- <span data-ttu-id="43d66-167">從 [ [訂閱](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ] 頁面中選取您的訂閱。</span><span class="sxs-lookup"><span data-stu-id="43d66-167">Select your subscription from the [Subscriptions](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) page.</span></span> <span data-ttu-id="43d66-168">按一下 [ **發票** ]，然後以電子郵件傳送發票</span><span class="sxs-lookup"><span data-stu-id="43d66-168">Click **Invoices** then Email my invoice</span></span>
- <span data-ttu-id="43d66-169">按一下 [ **加入** ] 並接受這些條款。</span><span class="sxs-lookup"><span data-stu-id="43d66-169">Click **opt in** and accept the terms.</span></span> <span data-ttu-id="43d66-170">您必須加入宣告您擁有的每一個訂閱</span><span class="sxs-lookup"><span data-stu-id="43d66-170">You will have to opt in for each subscription you own</span></span>

<span data-ttu-id="43d66-171">附注：如果您在遵循這些步驟之後未收到電子郵件，請確定您的電子郵件地址在[您的設定檔的通訊喜好](https://account.windowsazure.com/profile)設定中是正確的</span><span class="sxs-lookup"><span data-stu-id="43d66-171">Note: If you don't get an email after following the steps, make sure your email address is correct in the [communication preferences on your profile](https://account.windowsazure.com/profile)</span></span>

<span data-ttu-id="43d66-172">**從 Azure 入口網站下載使用狀況資料**</span><span class="sxs-lookup"><span data-stu-id="43d66-172">**Download your usage data from the Azure portal**</span></span>

- <span data-ttu-id="43d66-173">以[帳戶管理員](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)身分登入[Azure 帳戶中心](https://account.windowsazure.com/Subscriptions)</span><span class="sxs-lookup"><span data-stu-id="43d66-173">Sign into the [Azure Account Center](https://account.windowsazure.com/Subscriptions) as the [Account Admin](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)</span></span>
- <span data-ttu-id="43d66-174">選取您要取得發票和使用狀況資訊的訂閱</span><span class="sxs-lookup"><span data-stu-id="43d66-174">Select the subscription for which you want the invoice and usage information</span></span>
- <span data-ttu-id="43d66-175">選取 **帳單記錄**</span><span class="sxs-lookup"><span data-stu-id="43d66-175">Select **Billing History**</span></span>
- <span data-ttu-id="43d66-176">選取 [ **View Current 語句** ]，以查看預估產生時的費用估計值</span><span class="sxs-lookup"><span data-stu-id="43d66-176">Select **View Current Statement** to see an estimate of your charges at the time the estimate was generated</span></span>
- <span data-ttu-id="43d66-177">選取 [ **下載使用** ]，將每日使用狀況資料下載成 CSV 檔案。</span><span class="sxs-lookup"><span data-stu-id="43d66-177">Select **Download Usage** to download the daily usage data as a CSV file.</span></span> <span data-ttu-id="43d66-178">如果您看到兩個可用的版本，請下載第2版。</span><span class="sxs-lookup"><span data-stu-id="43d66-178">If you see two versions available, download version 2</span></span>

<span data-ttu-id="43d66-179">其他問題： [造訪保留執行個體文件](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="43d66-179">Other questions: [Visit reserved instance docs](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="43d66-180">**建議的文件**</span><span class="sxs-lookup"><span data-stu-id="43d66-180">**Recommended Documents**</span></span>

- [<span data-ttu-id="43d66-181">計費基礎</span><span class="sxs-lookup"><span data-stu-id="43d66-181">Billing basics</span></span>](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d66-182">瞭解保留的實例折扣的套用方式</span><span class="sxs-lookup"><span data-stu-id="43d66-182">Understand how the Reserved Instance discount is applied</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d66-183">下載或查看您的 Azure 計費發票和每日使用狀況資料</span><span class="sxs-lookup"><span data-stu-id="43d66-183">Download or view your Azure billing invoice and daily usage data</span></span>](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d66-184">瞭解保留的實例折扣的套用方式</span><span class="sxs-lookup"><span data-stu-id="43d66-184">Understand how the Reserved Instance discount is applied</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d66-185">瞭解隨付即用付費訂閱的保留實例用法</span><span class="sxs-lookup"><span data-stu-id="43d66-185">Understand Reserved Instance usage for your Pay-As-You-Go subscription</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d66-186">瞭解企業註冊的保留實例用法</span><span class="sxs-lookup"><span data-stu-id="43d66-186">Understand Reserved Instance usage for your Enterprise enrollment</span></span>](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d66-187">保留實例未包含的 Windows 軟體成本</span><span class="sxs-lookup"><span data-stu-id="43d66-187">Windows software costs not included with Reserved instances</span></span>](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="43d66-188">Partner Central Cloud Solution Provider 中的保留實例 (CSP) 程式</span><span class="sxs-lookup"><span data-stu-id="43d66-188">Reserved Instances in Partner Central Cloud Solution Provider (CSP) program</span></span>](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)