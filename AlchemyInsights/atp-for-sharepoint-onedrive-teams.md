---
title: 適用於 SharePoint、OneDrive 及 Microsoft Teams 的 ATP
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: b304f6c7d9959e49a8152c03f11c6c864a154ea5
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34764882"
---
# <a name="atp-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="db0b5-102">適用於 SharePoint、OneDrive 及 Microsoft Teams 的 ATP</span><span class="sxs-lookup"><span data-stu-id="db0b5-102">ATP for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="db0b5-103">請遵循下列步驟來啟用進階威脅防護：</span><span class="sxs-lookup"><span data-stu-id="db0b5-103">Follow these steps to enable Advanced Threat Protection:</span></span>

1. <span data-ttu-id="db0b5-104">移至 [[https://protection.office.com](https://protection.office.com)並以全域管理員或安全性系統管理員帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="db0b5-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="db0b5-105">在左側的導覽窗格中**威脅管理**] 下，選擇 [**原則** \> **安全附件**。</span><span class="sxs-lookup"><span data-stu-id="db0b5-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="db0b5-106">選取 [**開啟 ATP SharePoint、 OneDrive 及 Microsoft Teams**。</span><span class="sxs-lookup"><span data-stu-id="db0b5-106">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="db0b5-107">[建立活動警示原則](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts)到我們會偵測到的惡意檔案時收到通知。</span><span class="sxs-lookup"><span data-stu-id="db0b5-107">[Create an activity alert policy](https://docs.microsoft.com/office365/securitycompliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="db0b5-108">完整的指示，請參閱本[主題](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="db0b5-108">For complete instructions, see this [topic](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="db0b5-109">**附註**： 根據設計，ATP 不會掃描每一個檔案中 SharePoint Online、 OneDrive 商務或 Microsoft Teams。</span><span class="sxs-lookup"><span data-stu-id="db0b5-109">**Note**: By design, ATP doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="db0b5-110">使用共用活動，來賓活動，程序會以非同步方式掃描檔案，並威脅發出來識別惡意的檔案。</span><span class="sxs-lookup"><span data-stu-id="db0b5-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="db0b5-111">如需詳細資訊，請參閱本[主題](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="db0b5-111">For more information, see this [topic](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>
