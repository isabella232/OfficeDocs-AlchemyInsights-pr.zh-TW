---
title: Intune Exchange 內部部署連接器
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/28/2020
ms.locfileid: "48791422"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="04af1-102">Intune Exchange 內部部署連接器</span><span class="sxs-lookup"><span data-stu-id="04af1-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="04af1-103">如需設定在 Intune 和 Exchange （主控內部部署）之間的連接器的詳細資訊，請參閱下列檔：</span><span class="sxs-lookup"><span data-stu-id="04af1-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="04af1-104">在 Microsoft Intune Azure 中設定 Intune 內部部署 Exchange connector</span><span class="sxs-lookup"><span data-stu-id="04af1-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="04af1-105">**FAQ:：**</span><span class="sxs-lookup"><span data-stu-id="04af1-105">**FAQ:**</span></span>

<span data-ttu-id="04af1-106">問：當您嘗試設定 Exchange connector 時，看到錯誤，例如「不支援 Exchange Connector 版本」。</span><span class="sxs-lookup"><span data-stu-id="04af1-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="04af1-107">原因為何？</span><span class="sxs-lookup"><span data-stu-id="04af1-107">What could be the cause?</span></span>

<span data-ttu-id="04af1-108">A：您所使用的帳戶有適當的授權-必須具有 active Intune 授權</span><span class="sxs-lookup"><span data-stu-id="04af1-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="04af1-109">問：是否可以有多個 Exchange 連接器？</span><span class="sxs-lookup"><span data-stu-id="04af1-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="04af1-110">A：您只能為每個 Exchange 組織的每個 Intune 租使用者設定一個 Exchange connector。</span><span class="sxs-lookup"><span data-stu-id="04af1-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="04af1-111">連接器只可安裝在多部伺服器 exchange 組織中的一部伺服器上。</span><span class="sxs-lookup"><span data-stu-id="04af1-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="04af1-112">此外，您無法在同一個承租人中設定 Exchange 內部部署和 Exchange Online 的連接器。</span><span class="sxs-lookup"><span data-stu-id="04af1-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="04af1-113">Q：連接器是否可以使用 CAS 陣列作為其與 Exchange 的連線？</span><span class="sxs-lookup"><span data-stu-id="04af1-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="04af1-114">A：在連接器設定中指定的 CAS 陣列不是支援的設定。</span><span class="sxs-lookup"><span data-stu-id="04af1-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="04af1-115">只應該指定一部伺服器，而且應該是在連接器設定檔中找到的硬編碼，可在</span><span class="sxs-lookup"><span data-stu-id="04af1-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="04af1-116">program data\microsoft\microsoft Intune on Exchange connector \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="04af1-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="04af1-117">找到下列專案 ```<ExchangeWebServiceURL />``` ，並將 URL 取代為 exchange server。</span><span class="sxs-lookup"><span data-stu-id="04af1-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="04af1-118">**例子：**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="04af1-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="04af1-119">請參閱下列檔，以取得其他疑難排解： [疑難排解 Intune 內部部署 Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="04af1-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="04af1-120">**啟用 Exchange connector 的詳細記錄**</span><span class="sxs-lookup"><span data-stu-id="04af1-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="04af1-121">開啟 Exchange Connector 追蹤設定檔進行編輯。</span><span class="sxs-lookup"><span data-stu-id="04af1-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="04af1-122">檔案位於：%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="04af1-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="04af1-123">**例子：**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="04af1-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="04af1-124">使用下列機碼找到 TraceSourceLine： OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="04af1-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="04af1-125">將預設)  (的 [資訊] ActivityTracing 中的 SourceLevel 節點值變更為 Verbose ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="04af1-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="04af1-126">**範例：**</span><span class="sxs-lookup"><span data-stu-id="04af1-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="04af1-127">重新開機 Microsoft Intune Exchange 服務</span><span class="sxs-lookup"><span data-stu-id="04af1-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="04af1-128">在 Intune Portal 中執行完整同步處理，直到完成，然後將 XML 變更回「資訊 ActivityTracing」，並重新啟動 Microsoft Intune Exchange 服務。</span><span class="sxs-lookup"><span data-stu-id="04af1-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="04af1-129">記錄的位置如下： `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="04af1-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>