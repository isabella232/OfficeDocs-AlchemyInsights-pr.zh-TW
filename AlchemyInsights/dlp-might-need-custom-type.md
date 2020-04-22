---
title: DLP 可能需要自訂類型
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704480"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP 可能需要自訂類型

**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。

**DLP 可能需要自訂資訊類型**

使用資料遺失防護（DLP）原則，您可以識別及保護組織中的機密資料。 在某些情況下，您可能需要建立您自己的**自訂**敏感資訊類型，以保護組織的資料。

例如，您的組織可能需要識別及保護員工 IDs 或組織的某些特定格式的其他資料。如果是的話，請參閱下列文章以取得詳細資訊。
  
 **自訂內建的敏感性資訊類型**
  
如果內建的機密資訊類型只會滿足您的需求，只需要進行一些調整，您就可以[自訂內建的敏感資訊類型](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)。 例如，您可以新增或移除關鍵字，也可以新增或移除支援的證據，例如日期或位址。
  
 **建立自訂的敏感性資訊類型**
  
不過，如果您需要完全識別及保護不同類型的敏感資訊，您可以在安全性 & 合規性中心的 UI 中[建立自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。
  
**在安全性與合規性中心 PowerShell 中建立自訂敏感性資訊類型**

最後，如果使用者介面並未提供您所需的所有選項，您可以[在安全性 & 規範中心 PowerShell 中建立自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)。 從 XML 檔開始，您可以使用每個可用的選項。
