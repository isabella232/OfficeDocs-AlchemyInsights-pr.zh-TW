---
title: 執行網站探索
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50529193"
---
# <a name="do-site-discovery"></a>執行網站探索

如果組織仍使用舊版 Web 應用程式並計劃來使用 Internet Explorer 模式 (大部分客戶會這麼做)，則您應該執行一些額外的網站探索。

**您已部署舊版 Microsoft Edge**

如果您已經將企業網站清單設定為可對舊版 Microsoft Edge 運作，則您的網站探索幾乎已完成。 您可能需要做的一件事是新增中性網站。

中性網站通常是提供單一登入 (SSO) 的網站。 如果您從 Microsoft Edge 前往中性網站，則您會想要保持在 Microsoft Edge 中以進行驗證。 如果您以 Internet Explorer 模式前往中性網站，則您會想要保持 Internet Explorer 模式中以進行驗證。

識別您使用的任何 SSO 或其他中性網站，並將其新增到您的企業網站清單。

**Internet Explorer 是您的預設瀏覽器**

如果您現在僅使用 Internet Explorer，可能不知道哪些網站已升級至新式 Web 標準，以及哪些網站仍需要 Internet Explorer。 您將需要尋找並將這些網站新增到企業網站清單，以便可以只針對這些網站使用 Internet Explorer 模式。

> [!NOTE]
> [企業網站探索](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery)會探索可能需要 Internet Explorer 模式的網站。 它可以在 Windows 10、Windows 8.1 或 Windows 7 上從執行 Internet Explorer 8 到 Internet Explorer 11 的電腦上收集資料。

**分析資料**

收集網站資料之後，建議您執行下列的四個步驟程序來分析資料：
1. 依網域然後依 URL 排序資料。
2. 定義要針對 Internet Explorer 模式設定的應用程式界限。 您想要包含定義應用程式的所有網站和 Web 控制項，但不想包含額外的網站和控制項。 有些網站可能簡單的如 *https://contoso.com/app1* 一般，而其他網站可能需要您定義多個網站和頁面。
3. 測試應用程式以確認它無法原生地運作。 許多網站在偵測新式瀏覽器時會提供新式內容，並且會在偵測到 Internet Explorer 時僅提供舊版內容。
4. 如果應用程式無法通過測試，請將其新增到企業網站清單。

> [!NOTE]
> 最佳做法是將組成應用程式的所有網站分組。 如此一來，當您升級應用程式時，要從 Internet Explorer 模式移除整個網站，並開始對該應用程式使用新式瀏覽器會比較容易。

完成網站探索並分析資料之後，就可以開始查看您的通道策略。

