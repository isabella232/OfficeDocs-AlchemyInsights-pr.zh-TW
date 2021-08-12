---
title: 應用程式與 Microsoft Surface Pro X 的相容性
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/14/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7009"
- "9003951"
ms.openlocfilehash: 8f353d1337415183db1df168406b33594fb5fdb0aac3f13d0afe3e682fa6e3f3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932016"
---
# <a name="app-compatibility-with-microsoft-surface-pro-x"></a>應用程式與 Microsoft Surface Pro X 的相容性

應用程式在 Surface Pro X 等裝置上執行方式不同。大多數應用程式都是相容的，但也有一些限制。 以下是執行應用程式時可能遇到的問題清單： 

**驅動程式。** 如果驅動程式的設計對象是 Windows 10 ARM 型電腦，則其將運作。 如果驅動程式不運作，它所依賴的應用程式或硬體也不會運作。 有關裝置的其他支援，請參閱[Windows 10 ARM 型電腦常見問題集](https://support.microsoft.com/windows/windows-10-arm-based-pcs-faq-477f51df-2e3b-f68f-31b0-06f5e4f8ebb5)或諮詢硬體製造商。

**64-bit (x64) 應用程式。** 64 位元 (x64) 的應用程式無法運行。 您將需要64 位元 (ARM64) 應用程式、32 位元 (ARM32) 應用程式或 32 位元 (x86) 應用程式。 您通常可以找到 32 位元 (x86) 版本的應用程式，但有些應用程式開發人員只提供 64 位元 (x64) 應用程式。

**自訂應用程式。** 自訂 Windows 體驗的應用程式，如輔助技術或雲端儲存體應用程式可能會出現問題。 若要深入了解，請連絡應用程式製造商。

**協力廠商防毒軟體。** 無法安裝某些協力廠商防毒軟體。 Windows 安全性有助於在 Windows 10 裝置受支援的生命週期內確保裝置安全。

**Windows 傳真和掃描。** Windows 傳真和掃描在 Windows 10 ARM 型電腦上不可用。

如果您發現在安裝、解除安裝或重新安裝應用程式時遇到問題，請參閱[應用程式疑難排解詳細資料​​](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-app-install#app-troubleshooting-details)。

除極少數情况外，所有關鍵字都應該是「或」而不是「和」。