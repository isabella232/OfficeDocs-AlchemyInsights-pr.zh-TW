---
title: 取消保留
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003552"
- "6817"
ms.openlocfilehash: 04875e33f07c6d0a4306b3579ef81f2d28c7f506
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791398"
---
# <a name="cancelling-reservation"></a>取消保留

- **自助** ：您可以自己使用 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)取消或交換保留執行個體。 選取 [保留] 並按一下 [退款] 或 [交換]。 請注意，您必須有保留訂單的擁有者權限才能交換或退款。 僅存取保留將不允許您繼續退款或兌換。 要求保留訂單擁有者向您授予對保留訂單的存取權限
- **交換原則：** 您可以將一個保留與另一個相同類型的保留交換 – 保留交換 **沒有負面影響** 。 新保留的總承諾金額應大於兌換保留的退款金額和未來每月付款的總和 (如適用)
- **退款原則** ：在 12 個月的運行視窗內，退款和取消的未來付款總額不得超過 50000 美元。 我們 **目前不收取任何退款罰款** ，但可以在以後退款時收取  
    **例外：** 美國政府企業協定客戶不可用自助交換和取消功能
- **API / PS / CLI** 不支援取消和退款 [Azure 保留的自助兌換和退款](https://docs.microsoft.com/azure/cost-management-billing/reservations/exchange-and-refund-azure-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)
- 美國政府企業協定客戶不可用自助交換和取消功能。 支援其他美國政府訂閱類型，包括隨付隨用和 CSP

深入了解：[如何處理退貨和換貨交易](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)  
深入了解：[Exchange 和交換原則](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)  
其他問題： [造訪保留執行個體文件](https://docs.microsoft.com/azure/billing/billing-save-compute-costs-reservations?WT.mc_id=Portal-Microsoft_Azure_Support)

**交換現有的保留執行個體 (自助)**

您可以將一個保留換成另一個相同類型的保留。 如果您不再需要保留，您還可以退款 (最高每年 50000 美元)。 美國政府企業協定客戶不可用自助交換和取消功能。 支援其他美國政府訂閱類型，包括隨付隨用和 CSP。 您必須具有保留訂單上的擁有者權限才能兌換或退款現有保留。

以下步驟將指導完成交易的過程

1. 登入您的 [Azure 入口網站](https://portal.azure.com/#blade/Microsoft_Azure_Reservations/ReservationsBrowseBlade)。 選取您要退款的保留，然後按一下 **[交換]**
2. 選擇要購買的 VM 產品並輸入數量。 確保新的購買總額大於退貨總額[在購買之前確定正確的大小](https://docs.microsoft.com/azure/virtual-machines/windows/prepay-reserved-vm-instances?WT.mc_id=Portal-Microsoft_Azure_Support#determine-the-right-vm-size-before-you-buy)
3. 檢閱 並完成交易

**保留執行個體退款**

若要退款保留，請移至 **[保留詳細資料]** 然後按一下 **[退款]**

**專業等級退款：**

**退款和兌換的專業比例和最低要求範例**  
預先保留範例：

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

**建議的文件**

- [如何處理退貨和換貨交易](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#how-return-and-exchange-transactions-are-processed)
- [交換和退款原則](https://docs.microsoft.com/azure/billing/billing-azure-reservations-self-service-exchange-and-refund?WT.mc_id=Portal-Microsoft_Azure_Support#exchange-policies)