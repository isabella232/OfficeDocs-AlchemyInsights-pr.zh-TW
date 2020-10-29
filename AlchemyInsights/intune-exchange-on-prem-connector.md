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
# <a name="intune-exchange-on-premise-connector"></a>Intune Exchange 內部部署連接器

如需設定在 Intune 和 Exchange （主控內部部署）之間的連接器的詳細資訊，請參閱下列檔：

[在 Microsoft Intune Azure 中設定 Intune 內部部署 Exchange connector](https://docs.microsoft.com/intune/exchange-connector-install)

**FAQ:：**

問：當您嘗試設定 Exchange connector 時，看到錯誤，例如「不支援 Exchange Connector 版本」。 原因為何？

A：您所使用的帳戶有適當的授權-必須具有 active Intune 授權

問：是否可以有多個 Exchange 連接器？

A：您只能為每個 Exchange 組織的每個 Intune 租使用者設定一個 Exchange connector。 連接器只可安裝在多部伺服器 exchange 組織中的一部伺服器上。

此外，您無法在同一個承租人中設定 Exchange 內部部署和 Exchange Online 的連接器。

Q：連接器是否可以使用 CAS 陣列作為其與 Exchange 的連線？

A：在連接器設定中指定的 CAS 陣列不是支援的設定。 只應該指定一部伺服器，而且應該是在連接器設定檔中找到的硬編碼，可在

program data\microsoft\microsoft Intune on Exchange connector \ OnpremiseExchangeConnectorServiceConfiguration.xml

找到下列專案 ```<ExchangeWebServiceURL />``` ，並將 URL 取代為 exchange server。

**例子：**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

請參閱下列檔，以取得其他疑難排解： [疑難排解 Intune 內部部署 Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**啟用 Exchange connector 的詳細記錄**

1. 開啟 Exchange Connector 追蹤設定檔進行編輯。  
檔案位於：%ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml  

**例子：**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. 使用下列機碼找到 TraceSourceLine： OnPremisesExchangeConnectorService  
  
3. 將預設)  (的 [資訊] ActivityTracing 中的 SourceLevel 節點值變更為 Verbose ActivityTracing  

**範例：**
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
4. 重新開機 Microsoft Intune Exchange 服務  
5. 在 Intune Portal 中執行完整同步處理，直到完成，然後將 XML 變更回「資訊 ActivityTracing」，並重新啟動 Microsoft Intune Exchange 服務。  
6. 記錄的位置如下： `%ProgramData%\Microsoft\Windows Intune Exchange Connector`