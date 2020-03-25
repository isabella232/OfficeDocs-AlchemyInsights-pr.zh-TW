---
title: DLP 原則提示無法運作
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932577"
---
# <a name="dlp-policy-tip-issues"></a>DLP 原則提示問題

**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。 包括內容遷移、資料遺失防護（DLP）及備份解決方案。 在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。

為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。 您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。 不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。

**DLP 原則秘訣**

使用**DLP 原則**時，使用者可能會收到與**原則提示**違規的原則提示。 系統管理員可以設定在測試其 DLP 原則時或當原則處於完全強制執行模式時所顯示的原則提示。
  
若要在完整執行模式中的 [安全性與合規性中心] 中設定 DLP 原則上的原則提示，請執行下列操作：
  
- 使用[這裡](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)的步驟，確定已**啟用**DLP 規則上的原則提示。

- 確定您的**內容符合**觸發本文所述規則**所需**[的專案。](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)

- 原則提示會顯示在 OWA 和 Outlook 中。 不過，使用**Outlook 2013 或更新版本**時，原則秘訣只會顯示在某些情況下。 這些條件如下所示： [Outlook 2013 或更新版本支援的條件，以顯示原則提示](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)

如需有關 DLP 原則提示的詳細資訊，請參閱：[顯示 dlp 原則的原則提示](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)
  