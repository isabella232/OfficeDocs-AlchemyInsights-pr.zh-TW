---
title: 使用 TeamViewer 遠端管理 Intune 裝置
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798439"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>使用 TeamViewer 遠端管理 Intune 裝置

您可以使用 [TeamViewer](https://www.teamviewer.com/) 來遠端系統管理由 Intune 管理的裝置。

若要使用 TeamViewer 管理 Intune，請執行以下步驟： 

首先從 TeamViewer 獲取認證以在 Intune 上設定TeamViewer 連接器。 這允許管理員在裝置底下的 TeamViewer 連接器 UI 中輸入認證，這是在 Intune 和 TeamViewer 服務之間建立連結的一次性操作。

**第 1 部分：使用遠端裝置啟動工作階段**

1. 在 **[ 所有裝置 ]** 底下，選取您要啟動遠端工作階段的裝置。
2. 從 **…更多**，選取**新遠端協助工作階段**。
3. 選取 **[是]** 確認您要建立遠端工作階段。
    在 TeamViewer 服務確認 [啟動新遠端工作階段] 要求後，您將在裝置的 [概觀] (或 [基本資訊]) 窗格的詳細資訊下看到 **[啟動遠程協助] **的選項。 選取 **[查看更多]** 展開窗格，並顯示 [遠端協助] 狀態。
4. 選取 **[啟動遠端工作階段]**，在系統管理端啟動工作階段。
5. 選擇下載 TeamViewer 二進位 (Windows)，然後選取 **[執行]**。<br/>
    **附註** 您可以略過任何開啟到 TeamViewer 網站的網頁瀏覽器頁面。

6. 確認 TeamViewer 應用程式在裝置上進行變更的要求 (僅限 Windows)。
7. TeamViewer 應用程式啟動並包含工作階段代碼，以驗證與遠端裝置的連線。

**第 2 部分：遠程工作階段的目標裝置上**

1. 開啟 Intune 公司入口網站。
2. 尋找通知標識：「您的 IT 系統管理員正在請求遠端協助工作階段控制此裝置」，然後選取該通知。
3. 選擇下載 TeamViewer 應用程式，或確認從 App Store 下載 TeamViewer 應用程式，然後選取 **[執行]**。
    **附註** 您可以略過任何開啟到 TeamViewer 網站的網頁瀏覽器頁面。

4. 確認 TeamViewer 應用程式在裝置上進行變更的要求 (僅限 Windows)。
5. TeamViewer 應用程式啟動並包含工作階段代碼，以驗證與遠端裝置的連線。
6. 快顯詢問是否允許啟動工作階段。

**附註** TeamViewer 服務產生的工作階段代碼只能使用一次。 如果遺失連線，必須：

1. 關閉遠端裝置和系統管理員工作站上的 TeamViewer 應用程式執行個體。
2. 關閉遠端裝置上的公司入口網站。
3. 從系統管理員入口網站開始新的「新遠端協助工作階段」。
4. 重新開啟遠端裝置上的公司入口網站以接收新通知。
5. 像之前一樣，在遠端裝置和系統管理員工作站上的下載和開啟 TeamViewer 應用程式。