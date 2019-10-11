---
title: 因為大型附件一直停留在寄件匣
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441297"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>修正卡在寄件匣中的郵件

我們建議您開始執行從[Microsoft 支援及修復小幫手](https://diagnostics.office.com/#/)工具的 [ [「 我所遇到問題傳送、 接收或找出電子郵件 」](https://aka.ms/SaRA-OutlookSendReceive)的案例。

當郵件卡住寄件匣中時，最可能的原因如下：
- 大型附件。
- 未啟用 [**連線時，立即傳送**] 選項。

若要移除大型附件： 

1. 在 Outlook 中，選取 [**傳送 / 接收** > **離線工作**。 
2. 在 [功能窗格中，選取 [**寄件匣**]。 從這裡開始，您可以： 
    - 刪除郵件 （選取它，然後選取 [**刪除**）。
    - 將郵件拖曳至 [草稿] 資料夾，連按兩下以開啟它，並移除附件選取它，然後選取 [**刪除**）。
3. 如果您收到錯誤，指出 Outlook 正嘗試傳送郵件時，關閉 Outlook。 可能需要一些時間才能結束。 如果 Outlook 不會關閉，請按 Ctrl + Alt + Delete 鍵，然後選取 [**啟動工作管理員]**。 在 [工作管理員] 中，選取 [**程序**] 索引標籤，捲動至 [outlook.exe，然後選取 [**結束處理程序**。
4. Outlook 關閉之後，重新啟動它，然後重複步驟 2 和 3。 
5. 移除附件之後，按一下 [**傳送 / 接收** > **離線工作**，繼續線上工作。 

郵件也不知道寄件匣中按一下 [**傳送**]，但您無法連線時。 按一下 [**傳送 / 接收**，然後查看 [**離線工作**] 按鈕。 如果顯示藍色，您要中斷連線。 選取連線 （白色的按鈕開啟），並按一下 **[全部傳送**它。
 
若要啟用**連線時，立即傳送**：
 
- 選取**檔案** > **選項** >  **進階**。
在**傳送及接收**] 區段中，選取 [**連線時，立即傳送**，然後再選擇 [**確定]**。
 
完整詳細資料，請參閱：
- [影片： 傳送] 或 [刪除的停滯的電子郵件](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [電子郵件會停留在 [寄件匣] 資料夾，直到您手動啟動 Outlook 傳送/接收作業](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
