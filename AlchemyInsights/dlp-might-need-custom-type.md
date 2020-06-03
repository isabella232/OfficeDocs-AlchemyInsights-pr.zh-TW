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
ms.openlocfilehash: 1ec8959a479f1a8f7bfcffb55f440e8c4ab435fb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507505"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="14c35-102">DLP 可能需要自訂類型</span><span class="sxs-lookup"><span data-stu-id="14c35-102">DLP might need a custom type</span></span>

<span data-ttu-id="14c35-103">**重要**：在這些前所未有的情況下，我們會採取下列步驟以確保 SharePoint Online 和 OneDrive 服務保持高度可用 – 請造訪 [SharePoint Online 暫時功能調整](https://aka.ms/ODSPAdjustments)以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="14c35-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="14c35-104">**DLP 可能需要自訂資訊類型**</span><span class="sxs-lookup"><span data-stu-id="14c35-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="14c35-105">使用資料遺失防護（DLP）原則，您可以識別及保護組織中的機密資料。</span><span class="sxs-lookup"><span data-stu-id="14c35-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="14c35-106">在某些情況下，您可能需要建立您自己的**自訂**敏感資訊類型，以保護組織的資料。</span><span class="sxs-lookup"><span data-stu-id="14c35-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="14c35-107">例如，您的組織可能需要識別及保護員工 IDs 或組織的某些特定格式的其他資料。如果是的話，請參閱下列文章以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="14c35-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="14c35-108">**自訂內建的敏感性資訊類型**</span><span class="sxs-lookup"><span data-stu-id="14c35-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="14c35-109">如果內建的機密資訊類型只會滿足您的需求，只需要進行一些調整，您就可以[自訂內建的敏感資訊類型](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="14c35-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="14c35-110">例如，您可以新增或移除關鍵字，也可以新增或移除支援的證據，例如日期或位址。</span><span class="sxs-lookup"><span data-stu-id="14c35-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="14c35-111">**建立自訂的敏感性資訊類型**</span><span class="sxs-lookup"><span data-stu-id="14c35-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="14c35-112">不過，如果您需要完全識別及保護不同類型的敏感資訊，您可以在安全性 & 合規性中心的 UI 中[建立自訂機密資訊類型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="14c35-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="14c35-113">**在安全性與合規性中心 PowerShell 中建立自訂敏感性資訊類型**</span><span class="sxs-lookup"><span data-stu-id="14c35-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="14c35-114">最後，如果使用者介面並未提供您所需的所有選項，您可以[在安全性 & 規範中心 PowerShell 中建立自訂機密資訊類型](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="14c35-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="14c35-115">從 XML 檔開始，您可以使用每個可用的選項。</span><span class="sxs-lookup"><span data-stu-id="14c35-115">By starting with an XML file, you can use every option available.</span></span>
