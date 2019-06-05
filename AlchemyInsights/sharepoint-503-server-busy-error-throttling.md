---
title: SharePoint Online 節流
ms.author: kirks
author: Techwriter40
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 620a1094c1926b2c095c057a1791aaed8383afb3
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716918"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="2b106-102">SharePoint Online 節流</span><span class="sxs-lookup"><span data-stu-id="2b106-102">SharePoint Online Throttling</span></span>

<p><span data-ttu-id="2b106-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">使用者可能會收到 503 伺服器是忙碌錯誤，當您嘗試瀏覽至 Sharepoint 或 OneDrive 網站時。</span></span><span class="sxs-lookup"><span data-stu-id="2b106-103"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">Users may receive a 503 server is busy error when attempting to navigate to Sharepoint or OneDrive sites. </span></span></span></p> <p><span data-ttu-id="2b106-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">此錯誤可能被因內 Sharepoint 服務節流。SharePoint Online 使用節流以維持最佳的效能與可靠性的 SharePoint Online 服務。節流限制的使用者動作或並行數目 （來呼叫指令碼或程式碼） 以避免過度使用的資源。如果您不要取得節流，它是因為自訂程式碼的時間為 99%。</span></span><span class="sxs-lookup"><span data-stu-id="2b106-104"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">This error can be caused by throttling within the Sharepoint service. SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service. Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources. If you do get throttled, 99% of the time it is because of custom code.</span></span></span></p> <p><span data-ttu-id="2b106-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">如需有關節流設定，請參閱<a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">避免取得節流或封鎖 SharePoint Online 中</a>的詳細資訊。</span></span><span class="sxs-lookup"><span data-stu-id="2b106-105"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">For more information on throttling see, <a href="https://docs.microsoft.com/en-us/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online">Avoid getting throttled or blocked in SharePoint Online</a>.</span></span></span></p> <p><span data-ttu-id="2b106-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">如果您認為這項錯誤，若要節流與無關，您可以檢查是否有發生在您的租用戶上由瀏覽至<a href="https://portal.office.com/adminportal/home#/MessageCenter">訊息中心</a>的作用中維護。最後，請確定您造訪 [<a href="https://portal.office.com/adminportal/home#/servicehealth">服務健康情況</a>] 頁面上，若要檢查有可能會發生任何諮詢/事件。</span></span><span class="sxs-lookup"><span data-stu-id="2b106-106"><span style="mso-bidi-font-family: Calibri; mso-bidi-theme-font: minor-latin;">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the <a href="https://portal.office.com/adminportal/home#/MessageCenter">Message center</a>. Finally , ensure you visit the <a href="https://portal.office.com/adminportal/home#/servicehealth">Service Health</a> page to check for any advisories/incidents that may be occurring.</span></span></span></p> <p>&nbsp;</p>


