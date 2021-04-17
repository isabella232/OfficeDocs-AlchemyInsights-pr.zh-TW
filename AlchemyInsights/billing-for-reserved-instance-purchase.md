---
title: 購買保留實例的計費
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6814"
- "9003552"
ms.openlocfilehash: 9d71554d2089a6d9e5d4850149d113959f3d43c0
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51820313"
---
# <a name="billing-for-reserved-instance-purchase"></a>購買保留實例的計費

購買的保留的實例會計費到與您在購買時所選取之訂閱相關的支付方式。 訂閱類型必須是企業合約 (提供者編號： AZR-0017P) 、隨付費 (提供號碼： AZR-0003P) 、Microsoft 客戶合約或 CSP。

- 針對企業訂閱，費用會從登記的貨幣承諾餘額中扣減，或是因超額而收費。
- 若為隨送即用訂閱，訂閱上的信用卡或發票支付方式會收費。

**取消保留**

- **自助服務：** 您可以使用 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)自行取消或交換保留實例。 選取 [預約]，然後按一下 [退款] 或 [exchange]。 請注意，您必須將保留順序的擁有者存取權設為 [exchange] 或「退款」。 只有保留權可供您進行退款或 exchange 的存取。 要求預約訂單擁有人讓您擁有權存取預留訂單
- **Exchange 原則：** 您可以為相同類型的其他預約交換保留–保留 exchange **沒有處罰** 。 新的預約承諾總數應該大於更換的預約退款金額與未來每月付款 (（如果適用的話）的總和。) 
- **退款原則：** 退款總額和取消的未來付款金額在12個月的滾動視窗中不得超過 $50000 USD。 我們 **目前未收費退款的任何處罰** ，但可于未來退款時收費

**例外狀況：** 自助服務 exchange 和取消功能不適用於美國政府企業合約合約客戶

- **API/PS/CLI** 支援不適用於取消和退款 [Azure 保留的自助服務交換和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)功能
- 自助服務 exchange 和取消功能不適用於美國政府企業合約合約客戶。 支援其他美國政府訂閱類型（包括隨需付費和 CSP）

深入瞭解：[如何處理傳回和 exchange 交易](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)：深入瞭解： [exchange 及退款原則](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)其他問題：[就診保留實例](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)檔

**Exchange 現有的保留實例 (自助服務)**

您可以為相同類型的其他預訂，交換保留。 您也可以退款保留，每年 $50000 USD （如果您不再需要）。 自助服務 exchange 和取消功能不適用於美國政府企業合約合約客戶。 支援其他美國政府訂閱類型（包括隨付即用和 CSP）。 您必須具有保留訂單上的擁有者存取權，才可交換或退款現有的預約。

下列步驟會引導您完成交易的步驟。

1. 登入 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。 選取您要退款的預約，然後按一下 [ **Exchange** 2]。選取您要購買的 VM 產品並輸入數量。 請確定新的購買合計超過返還的上限 [決定您購買之前的正確大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)。
3. 複查並完成交易

**用於保留實例的退款**

若要退款預約，請移至 [**預約詳細資料**]，然後按一下 [**退款**]

**專業等級退款：**

**退款和 exchange 的 Pro-ration 和最低需求範例** 前期保留範例：

- 您于1月1日為 $120 購買一年期 RI
- 您想要退款或交換此保留的4月7日
- 因為保留已在97天內活，您會收到 (1-97/365) * $120 回來。  (（例如 $88.1) ）。 目前沒有退款的處罰
- 如果進行交換，您的新購買應該大於 $88。1
- 目前沒有退款的處罰

**計費計畫保留範例：**

- 每月購買一年 $10 的條款 RI
- 您想要退款或交換此保留的4月7日
- 自從最後一次付款發生7天之後，您會收到 (1-7/31) * $10 回來。  (，例如 $7.74) 
- 未來的付款已取消為 $80。 目前沒有退款的處罰
- 這種取消會從您的 $50000 退款限制中扣減 $87.74。
- 如果進行交換，新購買的總價值應大於 $87.74

**無法查看最後一個計費期間的發票**

您可能不會看到發票的某些可能原因：

- 您的訂閱具有每月的信用金額，但您的訂閱並未超過，或者您有免費試用版。 只有當您欠付金額時才產生發票
- 從您訂閱 Azure 的當日起不到30天的時間
- 尚未產生發票。 等到帳單期限結束
- 如果您不是帳戶管理員，可能無法使用舊版發票

**從 Azure 入口網站下載您的發票 ( .pdf)**

- 從 Azure 入口網站的 [ [訂閱](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ] 頁面中，選取您的訂閱，以 [供具有發票存取權的使用者使用](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- 選取 **發票**
- 按一下 **[下載發票]** 以查看您的 PDF 發票複本。 如果 **無法使用**，請參閱 [為什麼我看不到最後計費期間的發票？](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

**透過電子郵件 ( .pdf) 接收您的發票**

- 從 [ [訂閱](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ] 頁面中選取您的訂閱。 按一下 [ **發票** ]，然後以電子郵件傳送發票
- 按一下 [ **加入** ] 並接受這些條款。 您必須加入宣告您擁有的每一個訂閱

附注：如果您在遵循這些步驟之後未收到電子郵件，請確定您的電子郵件地址在[您的設定檔的通訊喜好](https://account.windowsazure.com/profile)設定中是正確的

**從 Azure 入口網站下載使用狀況資料**

- 以[帳戶管理員](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#whoisaa)身分登入[Azure 帳戶中心](https://account.windowsazure.com/Subscriptions)
- 選取您要取得發票和使用狀況資訊的訂閱
- 選取 **帳單記錄**
- 選取 [ **View Current 語句** ]，以查看預估產生時的費用估計值
- 選取 [ **下載使用** ]，將每日使用狀況資料下載成 CSV 檔案。 如果您看到兩個可用的版本，請下載第2版。

其他問題：[請造訪保留實例](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)檔

**建議的文件**

- [計費基礎](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [瞭解保留的實例折扣的套用方式](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [下載或查看您的 Azure 計費發票和每日使用狀況資料](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [瞭解保留的實例折扣的套用方式](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [瞭解隨付即用付費訂閱的保留實例用法](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [瞭解企業註冊的保留實例用法](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [保留實例未包含的 Windows 軟體成本](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Partner Central Cloud Solution Provider 中的保留實例 (CSP) 程式](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)