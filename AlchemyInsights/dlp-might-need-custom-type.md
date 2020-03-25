---
title: DLP 可能需要自訂類型
ms.author: pebaum
author: pebaum
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
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932649"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="e5c9c-102">DLP 可能需要自訂類型</span><span class="sxs-lookup"><span data-stu-id="e5c9c-102">DLP might need a custom type</span></span>

<span data-ttu-id="e5c9c-103">**重要**：許多 SharePoint 線上及 OneDrive 客戶對在後臺執行的服務執行業務關鍵型應用程式。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="e5c9c-104">包括內容遷移、資料遺失防護（DLP）及備份解決方案。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="e5c9c-105">在這些空前的時間內，我們採取的步驟，確定在遠端工作案例中，線上和 OneDrive 服務的 SharePoint，都為您的使用者提供高可用性和更可靠的服務。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="e5c9c-106">為了支援這專案標，我們已在星期幾的白天時段內，對背景應用程式（遷移、DLP 和備份解決方案）進行更為緊密的節流限制。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="e5c9c-107">您應該會認為，這些應用程式在這段時間內可達到非常有限的輸送量。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="e5c9c-108">不過，當地區的晚上和週末時，服務會準備好處理來自背景應用程式的大量要求。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="e5c9c-109">**DLP 可能需要自訂資訊類型**</span><span class="sxs-lookup"><span data-stu-id="e5c9c-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="e5c9c-110">使用資料遺失防護（DLP）原則，您可以識別及保護組織中的機密資料。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="e5c9c-111">在某些情況下，您可能需要建立您自己的**自訂**敏感資訊類型，以保護組織的資料。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="e5c9c-112">例如，您的組織可能需要識別及保護員工 IDs 或組織的某些特定格式的其他資料。如果是的話，請參閱下列文章以取得詳細資訊。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="e5c9c-113">**自訂內建的敏感性資訊類型**</span><span class="sxs-lookup"><span data-stu-id="e5c9c-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="e5c9c-114">如果內建的機密資訊類型只會滿足您的需求，只需要進行一些調整，您就可以[自訂內建的敏感資訊類型](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="e5c9c-115">例如，您可以新增或移除關鍵字，也可以新增或移除支援的證據，例如日期或位址。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="e5c9c-116">**建立自訂的敏感性資訊類型**</span><span class="sxs-lookup"><span data-stu-id="e5c9c-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="e5c9c-117">不過，如果您需要完全識別及保護不同類型的敏感資訊，您可以在安全性 & 合規性中心的 UI 中[建立自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type)。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="e5c9c-118">**在安全性與合規性中心 PowerShell 中建立自訂敏感性資訊類型**</span><span class="sxs-lookup"><span data-stu-id="e5c9c-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="e5c9c-119">最後，如果使用者介面並未提供您所需的所有選項，您可以[在安全性 & 規範中心 PowerShell 中建立自訂機密資訊類型](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell)。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="e5c9c-120">從 XML 檔開始，您可以使用每個可用的選項。</span><span class="sxs-lookup"><span data-stu-id="e5c9c-120">By starting with an XML file, you can use every option available.</span></span>
