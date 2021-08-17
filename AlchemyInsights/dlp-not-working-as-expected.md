---
title: DLP 未如期運作
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079693"
---
# <a name="dlp-not-working-as-expected"></a>DLP 未如期運作

**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。

 **設定 DLP**

是否有 **資料遺失防護 (DLP)** Office 365 未如期運作的問題？ 如果是的話，請確定已正確設定 **dlp 原則** ，且您的資料包含 **dlp 原則** 在評估時所要尋找的專案。
  
DLP 原則可讓您識別及保護組織中的機密資訊。 若要設定 DLP 原則，請在 [這裡](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)使用資訊。
  
 **DLP 原則的查找範圍**
  
在安全性與合規性中心使用內 **建的敏感資訊類型** 時，當偵測到這些敏感類型時，DLP 原則會尋找特定的模式和元素。
  
- **內建的敏感資訊類型**

    如需有關內建機密類型和 DLP 原則在偵測敏感類型時所尋找的資訊，請參閱： [敏感資訊類型的外觀](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。

- **自訂敏感資訊類型**

    如果您嘗試建立自訂的機密資訊類型，請使用下列文章，以取得如何建立自訂機密資訊類型的詳細資訊： [建立自訂的機密資訊類型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)。

**測試 DLP 原則**

若要使用內建或自訂的機密資訊類型來測試資料，請使用 [**分類**   >  **機密資訊類型**] 底下的 [測試類型] 選項。 如需詳細資訊，請參閱 [測試自訂機密資訊類型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)。

 **報告**
  
- 使用[DLP 報告](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)取得敏感性資料洞察力。

- 請參閱事件的特定詳細資料與 [附隨報告](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports)。
