---
title: DLP 未如預期運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: 3d8316502b4e51a101197a908cf691f0ab7f845a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389604"
---
# <a name="dlp-not-working-as-expected"></a>DLP 未如預期運作

您是否遇到 Office 365 中**資料遺失防護 (DLP)** 的問題無法如預期般運作？ 如果是的話, 請確定您的**DLP 原則**設定正確, 且您的資料包含了**dlp 原則**在評估時所要尋找的內容。
  
 **設定 DLP:**
  
DLP 原則可讓您識別和保護組織中的敏感資訊。 若要設定 DLP 原則, 請使用[此處](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)的資訊。
  
 **DLP 原則尋找的內容:**
  
在 Office 365 安全性與合規性中心使用**內建的機密資訊類型**時, DLP 原則會在偵測這些敏感類型時, 尋找特定模式和元素。
  
- **內建的機密資訊類型:**

    如需內建敏感類型以及偵測敏感類型時 DLP 原則所尋找的詳細資訊, 請參閱:[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。

- **自訂機密資訊類型:**

    如果您嘗試建立自訂的機密資訊類型, 請使用下列文章, 以取得如何建立自訂機密資訊類型的資訊:[建立自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。

 **下屬**
  
- 使用[DLP 報告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)取得敏感性資料洞察力。

- 請參閱事件的特定詳細資料與[附隨報告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)。
