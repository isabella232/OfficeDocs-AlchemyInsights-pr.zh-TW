---
title: 適用於 Office 365 的 Microsoft Defender，適用於 SharePoint、OneDrive 和 Microsoft Teams
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1037
ms.assetid: ''
ms.openlocfilehash: 7d2ed7bc4c7d99cd01dadc12e38762903d6d8ab3
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52543568"
---
# <a name="microsoft-defender-for-office-365-for-sharepoint-onedrive-and-microsoft-teams"></a><span data-ttu-id="b52cb-102">適用於 Office 365 的 Microsoft Defender，適用於 SharePoint、OneDrive 和 Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="b52cb-102">Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams</span></span>

<span data-ttu-id="b52cb-103">請遵循下列步驟，為 Office 365 啟用 Microsoft Defender：</span><span class="sxs-lookup"><span data-stu-id="b52cb-103">Follow these steps to enable Microsoft Defender for Office 365:</span></span>

1. <span data-ttu-id="b52cb-104">移至 [https://protection.office.com](https://protection.office.com) 並以全域管理員或安全性管理員帳戶登入。</span><span class="sxs-lookup"><span data-stu-id="b52cb-104">Go to [https://protection.office.com](https://protection.office.com) and sign in with a global administrator or security administrator account.</span></span>

2. <span data-ttu-id="b52cb-105">在 [ **威脅管理**] 底下的左側流覽窗格中，選擇 [ **原則** \> **安全附件**]。</span><span class="sxs-lookup"><span data-stu-id="b52cb-105">In the left navigation pane under **Threat management**, choose **Policy** \> **Safe Attachments**.</span></span>

3. <span data-ttu-id="b52cb-106">**針對 SharePoint、OneDrive 及 Microsoft Teams，選取 [為 Office 365 開啟 Defender**]。</span><span class="sxs-lookup"><span data-stu-id="b52cb-106">Select **Turn on Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**.</span></span>

4. <span data-ttu-id="b52cb-107">[建立活動警示原則](/microsoft-365/compliance/create-activity-alerts) ，以在我們偵測到惡意檔時收到通知。</span><span class="sxs-lookup"><span data-stu-id="b52cb-107">[Create an activity alert policy](/microsoft-365/compliance/create-activity-alerts) to receive notifications when we detect malicious files.</span></span>

<span data-ttu-id="b52cb-108">如需完整的指示，請參閱[開啟 SharePoint、OneDrive 和 Microsoft Teams 的安全附件](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="b52cb-108">For complete instructions, see this [Turn on Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams).</span></span>

<span data-ttu-id="b52cb-109">**附注**：依設計，Microsoft Defender for Office 365 不會掃描 SharePoint Online、商務用 OneDrive 或 Microsoft Teams 中的每一個檔案。</span><span class="sxs-lookup"><span data-stu-id="b52cb-109">**Note**: By design, Microsoft Defender for Office 365 doesn't scan every single file in SharePoint Online, OneDrive for Business, or Microsoft Teams.</span></span> <span data-ttu-id="b52cb-110">使用共用活動、訪客活動及威脅信號來識別惡意檔案的處理常式會以非同步方式掃描檔案。</span><span class="sxs-lookup"><span data-stu-id="b52cb-110">Files are scanned asynchronously by a process that uses sharing activity, guest activity, and threat signals to identify malicious files.</span></span> <span data-ttu-id="b52cb-111">如需詳細資訊，請參閱[SharePoint、OneDrive 及 Microsoft Teams 的安全附件](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams)。</span><span class="sxs-lookup"><span data-stu-id="b52cb-111">For more information, see [Safe Attachments for SharePoint, OneDrive, and Microsoft Teams](/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>
