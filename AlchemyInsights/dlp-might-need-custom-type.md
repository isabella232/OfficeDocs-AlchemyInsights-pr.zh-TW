---
title: DLP 可能需要自訂類型
ms.author: stephow
author: stephow-MSFT
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 8b49afcf50e5eb53f517bbdbd002fb80dddb6f9b
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35389676"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="17a63-102">DLP 可能需要自訂類型</span><span class="sxs-lookup"><span data-stu-id="17a63-102">DLP might need a custom type</span></span>

<span data-ttu-id="17a63-103">使用資料遺失防護 (DLP) 原則, 您可以識別和保護組織中的敏感性資料。</span><span class="sxs-lookup"><span data-stu-id="17a63-103">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="17a63-104">在某些情況下, 您可能需要建立自己的**自訂**機密資訊類型, 以保護貴組織的資料。</span><span class="sxs-lookup"><span data-stu-id="17a63-104">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="17a63-105">例如, 您的組織可能需要以某種特定格式來識別及保護員工識別碼或其他資料。若是如此, 請參閱下列文章以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="17a63-105">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="17a63-106">**自訂內建的敏感性資訊類型**</span><span class="sxs-lookup"><span data-stu-id="17a63-106">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="17a63-107">如果內建的敏感資訊類型只符合您的需求, 您可以[自訂內建的敏感資訊類型](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="17a63-107">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="17a63-108">例如, 您可以新增或移除關鍵字, 或新增或移除支援的證據, 例如日期或位址。</span><span class="sxs-lookup"><span data-stu-id="17a63-108">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="17a63-109">**建立自訂的敏感性資訊類型**</span><span class="sxs-lookup"><span data-stu-id="17a63-109">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="17a63-110">但是, 如果您需要完全識別及保護不同類型的敏感資訊, 您可以在安全性 & 規範中心的 UI 中[建立自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="17a63-110">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="17a63-111">**在安全性 & 合規性中心 PowerShell 中建立自訂機密資訊類型**</span><span class="sxs-lookup"><span data-stu-id="17a63-111">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="17a63-112">最後, 如果 UI 不提供您需要的所有選項, 您可以[在安全性 & 規範中心 PowerShell 中建立自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="17a63-112">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="17a63-113">從 XML 檔案開始, 您可以使用每個可用的選項。</span><span class="sxs-lookup"><span data-stu-id="17a63-113">By starting with an XML file, you can use every option available.</span></span>
