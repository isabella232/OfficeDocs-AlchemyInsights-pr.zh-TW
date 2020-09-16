---
title: 錯誤：無法上傳或下載您的變更，因為您的快取憑證已過期
ms.author: v-miegge
author: v-miegge
manager: v-cojank
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: ''
ms.custom:
- "3534"
- "9001489"
ms.openlocfilehash: 8105fa7b311bc932f95c8bff4d6b58ed9aabe74a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47734470"
---
# <a name="error-we-cant-upload-or-download-your-changes-because-your-cached-credentials-have-expired"></a><span data-ttu-id="21c27-102">錯誤：無法上傳或下載您的變更，因為您的快取憑證已過期</span><span class="sxs-lookup"><span data-stu-id="21c27-102">Error: We can't upload or download your changes because your cached credentials have expired</span></span>

<span data-ttu-id="21c27-103">將檔案儲存至 OneDrive 應用程式時，如果您收到的錯誤包含 **"您的快取認證已到期"** 字樣，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="21c27-103">When saving files to the OneDrive app, if you receive an error that contains the phrase **"your cached credentials have expired"**, perform the following steps:</span></span>

1. <span data-ttu-id="21c27-104">關閉所有 Office 應用程式。</span><span class="sxs-lookup"><span data-stu-id="21c27-104">Close all Office applications.</span></span>
1. <span data-ttu-id="21c27-105">開啟 [認證管理員]，並在工作列上的搜尋方塊中輸入 [ **認證管理員** ]，然後選取 [ **認證管理員控制台**]。</span><span class="sxs-lookup"><span data-stu-id="21c27-105">Open Credential Manager, and type **credential manager** in the search box on the taskbar, then select **Credential Manager Control panel**.</span></span>
1. <span data-ttu-id="21c27-106">選取 [ **Windows 認證**]。</span><span class="sxs-lookup"><span data-stu-id="21c27-106">Select **Windows Credentials**.</span></span>
1. <span data-ttu-id="21c27-107">尋找任何以 word **OneDrive**開頭的專案。</span><span class="sxs-lookup"><span data-stu-id="21c27-107">Find any entry that starts with the word **OneDrive**.</span></span>
1. <span data-ttu-id="21c27-108">選取專案，然後按 [ **移除**]。</span><span class="sxs-lookup"><span data-stu-id="21c27-108">Select the entry, then press **Remove**.</span></span>
1. <span data-ttu-id="21c27-109">關閉 [認證管理員]，然後在您的工作列中以滑鼠右鍵按一下藍色雲端，然後選取 [ **關閉] OneDrive**。</span><span class="sxs-lookup"><span data-stu-id="21c27-109">Close Credential Manager, then right click on the blue cloud in your systray, and select **Close OneDrive**.</span></span>
1. <span data-ttu-id="21c27-110">在工作列上的搜尋方塊中輸入 **OneDrive** ，然後選取 [OneDrive 要啟動的 **應用程式** OneDrive]。</span><span class="sxs-lookup"><span data-stu-id="21c27-110">Type **OneDrive** into the search box on the taskbar and select **OneDrive App** to launch OneDrive.</span></span>
1. <span data-ttu-id="21c27-111">登入 OneDrive，然後嘗試將檔儲存至 OneDrive。</span><span class="sxs-lookup"><span data-stu-id="21c27-111">Sign into OneDrive, then try to save the file to OneDrive.</span></span>
