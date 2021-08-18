---
title: 啟用保管庫 SharePoint 線上、OneDrive 和 Microsoft Teams 的附件
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
ms.openlocfilehash: 61372075ac8ccf04606a8003b4ec29f89fc048e5
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332370"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>啟用保管庫 SharePoint 線上、OneDrive 和 Microsoft Teams 的附件

1. 使用您的全域系統管理員或安全性系統管理員認證，開啟 Microsoft 365 Defender 入口網站 <https://security.microsoft.com> ，然後移至原則 **& 規則** \> **威脅** 原則 \> **保管庫附件** 的原則區段

   若要直接移至 [**保管庫附件**] 頁面，請使用 <https://security.microsoft.com/safeattachmentv2> 。

2. 在 [**保管庫附件**] 頁面上，按一下 [**通用設定**]。
3. 在出現的浮出控制項上，選取 [針對 **SharePoint、OneDrive 及 Microsoft Teams 開啟 Microsoft Defender Office 365**]，然後選取 [**儲存**]。

    **秘訣**：執行下列步驟，以加強 SharePoint、OneDrive 和 Microsoft Teams 的保管庫附件保護：
    - 若要防止使用者下載惡意檔案，請 `$true` 在 SharePoint 線上 PowerShell 的 **[Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** Cmdlet 上，使用 *DisallowInfectedFileDownload* 參數的值。 如需詳細資訊，請參閱[使用 SharePoint 線上 PowerShell 以避免使用者下載惡意](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)檔案。
    - [建立偵測到的檔案的警示原則](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

如需詳細資訊，請參閱[保管庫 Office 365 的附件供 SharePoint、OneDrive 及 Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041)。
