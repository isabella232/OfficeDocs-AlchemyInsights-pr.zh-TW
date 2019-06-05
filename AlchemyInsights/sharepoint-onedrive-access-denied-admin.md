---
title: 針對 「 拒絕存取 」 訊息進行疑難排解
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: ee154a60d80472639371d44faef464eea8734dc9
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716638"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a>疑難排解 Sharepoint/OneDrive 系統管理中心中的 「 拒絕存取 」 訊息

<p><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">如果您會收到拒絕存取訊息嘗試瀏覽至 Sharepoint/OneDrive 系統管理中心時，請確定該您<a href="https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One">指派授權給使用者</a>。如果使用者擁有授權，您也應該要確定他們已<a href="https://docs.microsoft.com/en-us/office365/admin/add-users/about-admin-roles?view=o365-worldwide">指派給系統管理員角色</a>可以存取系統管理中心。</span></p>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">當使用者是刪除並重新建立具有相同使用者主體名稱 (UPN)，也會發生這個問題。使用不同的 PUID （Passport 唯一識別碼） 值，會建立新的帳戶。當使用者嘗試存取網站集合或其 OneDrive 時，使用者會有不正確的 PUID。第二個案例牽涉到目錄同步處理與 Active Directory 組織單位 (OU)。如果使用者有已登入至 SharePoint]，然後會移至不同的 OU 和 resynced 與 SharePoint，否則可能會發生這個問題。</span></span></p>  <ul style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;" type="disc">  <li style="line-height: normal; ; font-size: 11pt; font-style: normal; font-weight: 400;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">若要解決此問題，您應還原原始的 UPN 與在文章中，<a href="https://docs.microsoft.com/en-us/office365/admin/add-users/restore-user?view=o365-worldwide">將還原的使用者在 Office 365 中</a>的步驟。</span></span></li>  </ul>  <p style="orphans: 2; -webkit-text-stroke-width: 0px; word-spacing: 0px;"><strong><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;">附註：</span></span></strong><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-fareast-font-family: 'Times New Roman'; mso-bidi-font-family: 'Times New Roman';"><span style="font-size: 10.5pt; font-family: '&amp;quot',serif;"><em style="mso-bidi-font-style: normal;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif;">&nbsp;</span></em><em><span style="font-family: '&amp;quot',serif;"><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;font-style: normal; mso-bidi-font-style: italic;">如果 OneDrive 或 SharePoint 系統管理中心不先前持有存取的多個使用者使用，可能會暫時的服務問題。&nbsp; </span></span></em><em><span style="font-size: 10.5pt; font-family: 'Verdana',sans-serif; mso-bidi-font-family: Calibri;"><a href="https://portal.office.com/adminportal/home#/servicehealth" target="_blank" rel="noopener"><span style="font-style: normal; mso-bidi-font-style: italic;">檢查的 service health dashboard</span></a>。</span></em></span></span></p>


