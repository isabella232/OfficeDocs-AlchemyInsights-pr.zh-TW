---
title: 如何停用外部群組
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "966"
- "6000006"
ms.assetid: 4e429507-039b-410e-a994-54b443d4e91e
ms.openlocfilehash: 9c513da49dc953b4ae76bb06854e33232ec40e11151f11ade33c3080092aa598
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54015611"
---
# <a name="how-to-disable-external-groups"></a>如何停用外部群組

Yammer 外部郵件會套用 Exchange 傳輸規則 (ETRs) ，這是一組主動控制措施，可防止公司資訊共用。 為了限制使用者建立外部群組，您必須 (ETR) 設定 Exchange 傳輸規則，然後設定 Yammer，以使用 Exchange 傳輸規則來封鎖外部郵件。
  
在 Exchange Online 系統管理中心建立規則之後，請遵循下列步驟，將 ETR 設定為套用於 Yammer 中：
  
- 以已驗證的系統管理員身分登入 Yammer，然後在 **Yammer 系統管理中心**，移至 C **內容及安全性 \> 安全性設定。**

- 在 [**外部郵件**] 底下，選取 [**強制您的 Exchange Online Exchange 傳輸規則 (ETRs) in Yammer。**

- 選擇 **[儲存]**。

如需詳細資訊，請參閱[停用 Yammer 網路中的外部郵件](https://docs.microsoft.com/yammer/work-with-external-users/disable-external-messaging)。
  