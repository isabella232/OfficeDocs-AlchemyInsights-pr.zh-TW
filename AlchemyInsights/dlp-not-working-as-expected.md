---
title: DLP 未如期運作
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
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932613"
---
# <a name="dlp-not-working-as-expected"></a>DLP 未如期運作

**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。 包括內容遷移、資料遺失防護（DLP）及備份解決方案。 在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。

為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。 您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。 不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。

 **設定 DLP**

Office 365 中的**資料遺失防護（DLP）** 未如期運作時，是否發生問題？ 如果是的話，請確定已正確設定**dlp 原則**，且您的資料包含**dlp 原則**在評估時所要尋找的專案。
  
DLP 原則可讓您識別及保護組織中的機密資訊。 若要設定 DLP 原則，請在[這裡](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)使用資訊。
  
 **DLP 原則的查找範圍**
  
在 Office 365 安全性與合規性中心使用內**建的敏感資訊類型**時，當偵測到這些敏感類型時，DLP 原則會尋找特定的模式和元素。
  
- **內建的敏感資訊類型**

    如需有關內建機密類型和 DLP 原則在偵測敏感類型時所尋找的資訊，請參閱：[敏感資訊類型的外觀](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)。

- **自訂敏感資訊類型**

    如果您嘗試建立自訂的機密資訊類型，請使用下列文章，以取得如何建立自訂機密資訊類型的詳細資訊：[建立自訂的機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。

**測試 DLP 原則**

若要使用內建或自訂的機密資訊類型來測試資料，請使用 [**分類** > **機密資訊類型**] 底下的 [**測試類型**] 選項。 如需詳細資訊，請參閱[測試自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center)。

 **報告**
  
- 使用[DLP 報告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)取得敏感性資料洞察力。

- 請參閱事件的特定詳細資料與[附隨報告](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)。
