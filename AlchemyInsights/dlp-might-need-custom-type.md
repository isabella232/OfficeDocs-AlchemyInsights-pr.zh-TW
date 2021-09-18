---
title: DLP 可能需要自訂類型
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446682"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP 可能需要自訂類型

**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。

**DLP 可能需要自訂資訊類型**

透過資料遺失防護 (DLP) 原則，您可以識別及保護組織中的機密資料。 在某些情況下，您可能需要建立您自己的自訂敏感資訊類型，以保護組織的資料。 如需詳細資訊，請參閱 [瞭解敏感資訊類型](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) 和 [機密資訊類型實體定義](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)。

如需如何建立自訂機密資訊類型和原則的詳細資訊，請參閱： 

**自訂內建的敏感性資訊類型**

如果內建的機密資訊類型只會滿足您的需求，只需要進行一些調整，請參閱 [自訂內建的敏感資訊類型](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。 例如，您可以新增或移除關鍵字，也可以新增或移除支援的證據，例如日期或位址。

**建立自訂的敏感性資訊類型**

不過，如果您需要完全識別及保護不同類型的敏感資訊，您可以在 Microsoft 365 合規性中心中建立自訂機密資訊類型。 如需詳細資訊，請參閱 [開始使用自訂機密資訊類型](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。

**在安全性與合規性中心 PowerShell 中建立自訂敏感性資訊類型**

最後，如果使用者介面並未提供您所需的所有選項，您可以在安全性 & 規範中心 PowerShell 中建立自訂機密資訊類型。 從 XML 檔開始，您可以使用每個可用的選項。 如需詳細資訊，請參閱 [使用 PowerShell 建立自訂機密資訊類型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)。

若要先在測試模式中測試原則，請參閱 [在測試模式中實施原則](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) ，以及 [建立、測試及調整 DLP 原則](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy)。 