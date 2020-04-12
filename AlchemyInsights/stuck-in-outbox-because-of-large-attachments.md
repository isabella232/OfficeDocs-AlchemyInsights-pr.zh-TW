---
title: 因大附件而滯留于寄件匣
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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232621"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>修正寄件匣中停滯的郵件

我們建議您從受影響電腦上的[Microsoft 支援及修復](https://diagnostics.office.com/#/)小幫手工具中，執行「[我已有問題傳送、接收或尋找電子郵件訊息](https://aka.ms/SaRA-OutlookSendReceive)」案例。

當郵件在您的 [寄件匣] 中停滯時，最可能的原因是大型附件或「連線時立即傳送」選項未啟用。

**移除大型附件**

1. 按一下 [**傳送/接收** > **離線工作**]。 
2. 在功能窗格中，按一下 [**寄件匣**]。 在這裡，您可以： 
    - 刪除郵件。 只需選取它，然後按一下 [**刪除**]。
    - 將郵件拖曳至 [**草稿] 資料夾**，按兩下以開啟郵件，然後刪除附件（按一下該附件，然後按一下 [**刪除**]）。
3. 如果錯誤告訴您 Outlook 嘗試傳輸郵件，請關閉 Outlook。 可能需要幾分鐘的時間才能結束。 若 Outlook 未關閉，請按**Ctrl + Alt + Delete** ，然後按一下 [**開始任務管理員**]。 在 **[任務**管理器] 中，選取 [程式] 索引標籤，向下滾動至 [excel.exe]，然後按一下 [**結束**程式]。
4. Outlook 關閉後，請重新開機 Outlook，然後重複步驟2-3。 
5. 移除附件後，請按一下 [**傳送/接收** > **離線工作**] 以取消選取按鈕，並繼續線上工作。 

當您按一下 [**傳送**]，但未連接時，郵件也會在 [寄件匣] 中停滯。 按一下 [**傳送/接收**]，然後查看 [**工作離線工作**] 按鈕。 如果是藍色，表示您已中斷連線。 按一下以進行連線（按鈕變成白色），然後按一下 [**全部傳送**]。
 
**啟用連線時立即傳送**
 
1. 在 [檔案] 索引標籤上，按一下 [選項]。****

2. 按一下 [Outlook 選項] 對話方塊中的 [進階]。****

3. 在 [傳送及接收] 區段中，按一下以啟用**連線時立即傳送**。 按一下 [確定]****。
 
如需完整的詳細資訊，請參閱：
- [影片：傳送或刪除卡住的電子郵件](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [除非您在 Outlook 中手動啟動傳送/接收作業，否則電子郵件會保留在 [寄件匣] 資料夾中。](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
