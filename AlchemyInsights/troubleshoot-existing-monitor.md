---
title: 疑難排解現有監視器
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690702"
---
# <a name="troubleshoot-an-existing-monitor"></a>疑難排解現有監視器

請嘗試這些解決方案來疑難排解監視器。 

**重新整理監視器的顯示：**

同步選取下列機碼： Windows 鍵 + Ctrl + Shift + B。這將會重新整理與您的圖形驅動程式的通訊。 您的監視器會稍閃閃爍，並在幾秒鐘後傳回回來。

**監視硬體疑難排解：**

1. 拔下將電腦連接至監視器的電纜，然後再將它插入。
2. 中斷電腦 (的任何非必要裝置，例如配接器或塢站) 。

**如果您最近在您的電腦上安裝更新，您可以復原您的顯示驅動程式：**

1. 選取 [ **開始**]，輸入 [ **裝置管理員**]，然後從 [結果] 中選取 [ **裝置管理員** ]。
2. 展開 [ **顯示配接器** ] 區段中，以滑鼠右鍵按一下您的顯示配接器，and 選取 [ **屬性**]。
3. 流覽至 [ **驅動程式** ] 索引標籤，然後選取 [ **還原驅動程式**]。 <br>
附注：如果這不是可用或變暗，請從下列選項中選取 [ **否** ]，以移至下一個步驟。
4. 您可能需要先重新開機電腦，這些變更才會生效。

**卸載並重新安裝您的顯示驅動程式：**

1. 選取 [ **開始**]，輸入 [ **裝置管理員**]，然後從 [結果] 中選取 [ **裝置管理員** ]。
2. 展開 [ **顯示配接器** ] 區段中，以滑鼠右鍵按一下您的顯示配接器，and 選取 [ **卸載裝置**]。 
3. 選取 [ **刪除此裝置的驅動程式軟體** ] 旁邊的方塊，然後選取 [ **卸載**]。<br>
附注：您可能會在此階段要求您重新開機電腦。 重新開機之前，請務必記下來餘下的指示。
4. 再次開啟 [裝置管理員]。
5. 展開 [ **顯示配接器** ] 區段，以滑鼠右鍵按一下您的顯示配接器，然後選取 [ **更新驅動程式**]。
6. 選取 [ **自動搜尋更新驅動程式軟體** ]，並遵循安裝指示。