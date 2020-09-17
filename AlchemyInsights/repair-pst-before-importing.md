---
title: 在匯入前修復 .pst 檔案
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1226"
- "1800027"
ms.assetid: ''
ms.openlocfilehash: 1ed37192a6b054b745fd48fbc01a6b00fa7074ed
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2020
ms.locfileid: "47799087"
---
# <a name="repair-pst-file-before-importing"></a><span data-ttu-id="64f6c-102">在匯入前修復 .pst 檔案</span><span class="sxs-lookup"><span data-stu-id="64f6c-102">Repair .pst file before importing</span></span>

<span data-ttu-id="64f6c-103">在 Outlook 中匯入 .pst 檔案之前，請先確認檔案未損毀，請修復檔案：</span><span class="sxs-lookup"><span data-stu-id="64f6c-103">Before you import a .pst file in Outlook, verify the file is not corrupted by repairing the file:</span></span>

1. <span data-ttu-id="64f6c-104">結束 Outlook。</span><span class="sxs-lookup"><span data-stu-id="64f6c-104">Exit Outlook.</span></span>

2. <span data-ttu-id="64f6c-105">`Scanpst.exe`在您的 Office 程式資料夾中尋找並執行 (C:\Program 檔案 (x86) \Microsoft Office\root\Office \<Version\> 或 C:\Program Files\Microsoft Office\root\Office \<Version\>) 。</span><span class="sxs-lookup"><span data-stu-id="64f6c-105">Find and run `Scanpst.exe` in your Office program folder (C:\Program Files (x86)\Microsoft Office\root\Office\<Version\> or C:\Program Files\Microsoft Office\root\Office\<Version\>).</span></span>

3. <span data-ttu-id="64f6c-106">在 **Microsoft Outlook 收件匣修復工具**中，按一下 **[流覽]** 以尋找 .pst 檔案 (例如，在 [C:\Users \\<username \> \AppData\Local\Microsoft\Outlook) ] 中。</span><span class="sxs-lookup"><span data-stu-id="64f6c-106">In the **Microsoft Outlook Inbox Repair tool**, click **Browse** to find the .pst file (for example, in C:\Users\\<username\>\AppData\Local\Microsoft\Outlook).</span></span> <span data-ttu-id="64f6c-107">選取 .pst 檔案，然後按一下 [ **開啟**]。</span><span class="sxs-lookup"><span data-stu-id="64f6c-107">Select the .pst file and then click **Open**.</span></span>

4. <span data-ttu-id="64f6c-108">按一下 [ **啟動** ] 開始掃描。</span><span class="sxs-lookup"><span data-stu-id="64f6c-108">Click **Start** to begin the scan.</span></span>

5. <span data-ttu-id="64f6c-109">如果在檔中找到錯誤，請按一下 [ **修復**]，然後在修復完成時按一下 **[確定]** 。</span><span class="sxs-lookup"><span data-stu-id="64f6c-109">If errors are found in the file, click **Repair**, and then click **OK** when the repair is complete.</span></span>

6. <span data-ttu-id="64f6c-110">嘗試重新匯入 Outlook 中的 .pst 檔案。</span><span class="sxs-lookup"><span data-stu-id="64f6c-110">Try to import the .pst file in Outlook again.</span></span>

<span data-ttu-id="64f6c-111">如需詳細資訊，請參閱 [修復 outlook 資料檔案](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) 並 [修正匯入 Outlook .pst](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e)檔案的問題。</span><span class="sxs-lookup"><span data-stu-id="64f6c-111">For more information, see [Repair Outlook data files](https://support.office.com/article/25663bc3-11ec-4412-86c4-60458afc5253) and [Fix problems importing an Outlook .pst file](https://support.office.com/article/2d2e50dc-5c36-4ab2-ab50-f1be733b3d6e).</span></span>
