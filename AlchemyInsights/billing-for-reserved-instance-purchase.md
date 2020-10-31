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
# <a name="billing-for-reserved-instance-purchase"></a>保留執行個體的購買帳單

系統會依照您在購買時所選訂閱的付款條件，對保留執行個體之購買進行收費。 訂閱類型必須是企業合約 (優惠號碼： MS-AZR-0017P)、隨用隨付 (優惠號碼： MS-AZR-0003P)、Microsoft 客戶合約或 CSP。

- 如果是企業版訂閱，費用會從登記的金錢履約承諾餘額中扣減，或以超額進行收費
- 針對 [隨用隨付] 訂閱，會以信用卡或訂閱上的發票付款方式進行收費

**取消保留**

- **自助** ：您可以自己使用 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)取消或交換保留執行個體。 選取 [保留] 並按一下 [退款] 或 [交換]。 請注意，您必須有保留訂單的擁有者權限才能交換或退款。 僅存取保留將不允許您繼續退款或兌換。 要求保留訂單擁有者向您授予對保留訂單的存取權限
- **交換原則：** 您可以將一個保留與另一個相同類型的保留交換 – 保留交換 **沒有負面影響** 。 新保留的總承諾金額應大於兌換保留的退款金額和未來每月付款的總和 (如適用)
- **退款原則** ：在 12 個月的運行視窗內，退款和取消的未來付款總額不得超過 50000 美元。 我們 **目前不收取任何退款罰款** ，但可以在以後退款時收取

**例外：** 美國政府企業協定客戶不可用自助交換和取消功能

- **API / PS / CLI** 不支援取消和退款 [Azure 保留的自助兌換和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- 美國政府企業協定客戶不可用自助交換和取消功能。 支援其他美國政府訂閱類型，包括隨付隨用和 CSP

深入瞭解：[如何處理傳回和 exchange 交易](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)：深入瞭解： [exchange 及退款原則](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)其他問題：[就診保留實例](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)檔

**交換現有的保留執行個體 (自助)**

您可以將一個保留換成另一個相同類型的保留。 如果您不再需要保留，您還可以退款 (最高每年 50000 美元)。 美國政府企業協定客戶不可用自助交換和取消功能。 支援其他美國政府訂閱類型，包括隨付隨用和 CSP。 您必須具有保留訂單上的擁有者權限才能兌換或退款現有保留。

以下步驟將指導完成交易的過程

1. 登入 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。 選取您要退款的預約，然後按一下 [ **Exchange** 2]。選取您要購買的 VM 產品並輸入數量。 請確定新的購買合計超過返還的上限 [決定您購買之前的正確大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)。
3. 複查並完成交易

**保留執行個體退款**

若要退款保留，請移至 **[保留詳細資料]** 然後按一下 **[退款]**

**專業等級退款：**

**退款和 exchange 的 Pro-ration 和最低需求範例** 前期保留範例：

- 你在 1 月 1 日以 120 美元購買一年期的 RI
- 您想在 4 月 7 日退換這個保留嗎
- 由於保留已經進行 了97 天，您將獲得 (1-97/365)*120 美元。 (i.e. $88.1)。 目前退款沒有罰款
- 如果換貨，您的新購買金額應大於 88.1 美元
- 目前退款沒有罰款

**計費計畫保留範例：**

- 你以每月 10 美元的價格購買一年期定期 RI
- 您想在 4 月 7 日退換這個保留
- 由於最後一次付款在 7 天前，你將得到 (1-7/31)*10 美元。 (例如 $7.74)
- 取消的未來付款是 80 美元。 目前退款沒有罰款
- 這次取消將從您的 50000 美元退款限額中扣除 87.74 美元
- 如果交換，新購買的總價值應大於 87.74 美元

**無法查看最後一個計費期間的發票**

您可能不會看到發票的某些可能原因：

- 您的訂閱具有每月的信用金額，但您的訂閱並未超過，或者您有免費試用版。 只有當您欠付金額時才產生發票
- 從您訂閱 Azure 的當日起不到30天的時間
- 尚未產生發票。 等到帳單期限結束
- 如果您不是帳戶管理員，可能無法使用舊版發票

**從 Azure 入口網站下載您的發票 ( .pdf)**

- 從 Azure 入口網站的 [ [訂閱](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) ] 頁面中，選取您的訂閱，以 [供具有發票存取權的使用者使用](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- 選取 **發票**
- 按一下 [ **下載發票** ] 以查看您的 PDF 發票的副本。 如果 **無法使用** ，請參閱 [為什麼我看不到最後計費期間的發票？](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#noinvoice)

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

其他問題： [造訪保留執行個體文件](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**建議的文件**

- [計費基礎](https://docs.microsoft.com/partner-center/billing-basics/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [瞭解保留的實例折扣的套用方式](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [下載或查看您的 Azure 計費發票和每日使用狀況資料](https://docs.microsoft.com/azure/billing/billing-download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support)
- [瞭解保留的實例折扣的套用方式](https://docs.microsoft.com/azure/billing/billing-understand-vm-reservation-charges/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [瞭解隨付即用付費訂閱的保留實例用法](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [瞭解企業註冊的保留實例用法](https://docs.microsoft.com/azure/billing/billing-understand-reserved-instance-usage-ea/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [保留實例未包含的 Windows 軟體成本](https://docs.microsoft.com/azure/billing/billing-reserved-instance-windows-software-costs/?WT.mc_id=Portal-Microsoft_Azure_Support)
- [Partner Central Cloud Solution Provider 中的保留實例 (CSP) 程式](https://docs.microsoft.com/partner-center/azure-reservations/?WT.mc_id=Portal-Microsoft_Azure_Support)