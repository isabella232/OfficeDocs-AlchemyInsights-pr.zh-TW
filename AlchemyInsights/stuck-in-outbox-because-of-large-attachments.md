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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241243"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a>修正寄件匣中停滯的郵件

我們建議您從[Microsoft 支援及修復](https://diagnostics.office.com/#/)小幫手工具中執行「[我遇到傳送、接收或尋找電子郵件訊息時出現問題](https://aka.ms/SaRA-OutlookSendReceive)」案例的狀態。

當郵件在您的 [寄件匣] 中停滯時，最可能的原因是大型附件或「連線時立即傳送」選項未啟用。

**移除大型附件**

1. 在 Outlook 中，選取 [**傳送/接收** > **離線工作**]。 
2. 在功能窗格中，選取 [**寄件匣**]。 在這裡，您可以： 
    - 刪除郵件（選取它，然後選取 [**刪除**]）。
    - 將郵件拖曳至 [草稿] 資料夾，按兩下以開啟它，然後移除附件，然後選取 [**刪除**]。
3. 如果您收到錯誤，指出 Outlook 嘗試傳輸郵件，請關閉 Outlook。 可能需要幾分鐘的時間才能結束。 若 Outlook 未關閉，請按 Ctrl + Alt + Delete，然後選取 [**開始任務管理員**]。 在 **[任務**管理器] 中，選取 [程式] 索引標籤，向下滾動至 [excel.exe]，然後選取 [**結束**程式]。
4. Outlook 關閉後，請重新開機，並重複步驟2和3。 
5. 移除附件後，請按一下 [**傳送/接收** > **離線工作**] 以繼續線上工作。 

當您按一下 [**傳送**]，但未連接時，郵件也會在 [寄件匣] 中停滯。 按一下 [**傳送/接收**]，然後查看 [**工作離線工作**] 按鈕。 如果是藍色，表示您已中斷連線。 按一下以進行連線（按鈕變成白色），然後按一下 [**全部傳送**]。
 
**啟用連線時立即傳送**
 
1. 在 [檔案] 索引標籤上，按一下 [選項]。****

2. 按一下 [Outlook 選項] 對話方塊中的 [進階]。****

3. 在 [傳送及接收] 區段中，按一下以啟用**連線時立即傳送**。 按一下 [確定]****。
 
如需完整的詳細資訊，請參閱：
- [影片：傳送或刪除卡住的電子郵件](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [除非您在 Outlook 中手動啟動傳送/接收作業，否則電子郵件會保留在 [寄件匣] 資料夾中。](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
