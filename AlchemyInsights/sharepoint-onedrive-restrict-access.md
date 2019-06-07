---
title: 限制存取 SharePoint 或 OneDrive 中
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 3227f10270148c0e515b687c48058affa4d2be70
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/07/2019
ms.locfileid: "34759072"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>限制存取 SharePoint 或 OneDrive 中

有許多方式可以限制存取 SharePoint Online/OneDrive 服務。 這些不同的存取限制方法概述如下。 

權限限制

在 SharePoint Online 和商務用 OneDrive，我們要限制存取網站、 檔案及資料夾等項目只授與存取這些群組/個人應該具有存取權。

[自訂 SharePoint 清單或文件庫的權限](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

[自訂 SharePoint 網站的權限](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions) (機器翻譯)

[變更子資料夾的權限](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

[從未受控裝置中控制存取權](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

為 SharePoint 或 Office 365 全域系統管理員，您可以封鎖或限制存取 SharePoint 和 OneDrive 內容來自未受管理的裝置 (這些混合式 AD 加入或相容 Intune 中)。

網路位置限制

身為 IT 系統管理員，您可以控制存取 SharePoint 和 OneDrive 的資源，根據您信任的已定義的網路位置。 這也稱為是位置為基礎的原則。 如需詳細資訊，請參閱[SharePoint Online 和 OneDrive 資料是根據網路位置控制存取](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)

網站鎖定限制 

在 SharePoint Online 中，您必須鎖定網站集合，因此沒有人有權存取的能力。 這是透過 PowerShell 和[SharePoint Online 管理命令介面](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)使用[Set-sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState 屬性設定。

限制使用者只能建立網站或子網站

為 SharePoint 系統管理員或 Office 365 全域系統管理員，您可以讓您的使用者建立及管理自己的 SharePoint 網站，請決定何種網站他們可以建立，並指定網站的位置。 如需詳細資訊，請參閱[在 SharePoint Online 中的管理網站架設](https://docs.microsoft.com/sharepoint/manage-site-creation)

