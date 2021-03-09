---
title: 為 SharePoint Online、OneDrive 和 Microsoft 團隊啟用 Microsoft Defender for Office 365
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/08/2021
ms.locfileid: "50552327"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="b692b-102">為 SharePoint Online、OneDrive 和 Microsoft 團隊啟用 Microsoft Defender for Office 365</span><span class="sxs-lookup"><span data-stu-id="b692b-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="b692b-103">使用您的全域系統管理員或安全性系統管理員認證，登入 [Office 365 安全性與合規性中心](https://protection.office.com/)。</span><span class="sxs-lookup"><span data-stu-id="b692b-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="b692b-104">在左窗格中選取 [**威脅管理**]，然後選取 [**原則**  >  [安全附件](https://protection.office.com/safeattachment)]。</span><span class="sxs-lookup"><span data-stu-id="b692b-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="b692b-105">**針對 SharePoint、OneDrive 和 Microsoft 團隊選取 [開啟 Microsoft Defender For Office 365**]，然後選取 [**儲存**]。</span><span class="sxs-lookup"><span data-stu-id="b692b-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="b692b-106">以全域管理員或 SharePoint Online 管理員身分執行下列 PowerShell Cmdlet，並將 **DisallowInfectedFileDownload** 參數設定為 *true*： [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="b692b-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="b692b-107">為偵測到的檔案設定警示</span><span class="sxs-lookup"><span data-stu-id="b692b-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="b692b-108">如需詳細資訊，請參閱 [適用于 SharePoint、OneDrive 和 Microsoft 小組的 Microsoft Defender For Office 365](https://go.microsoft.com/fwlink/?linkid=2092041)。</span><span class="sxs-lookup"><span data-stu-id="b692b-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
