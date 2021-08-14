---
title: ADFS 同盟憑證逾期失效
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "645"
- "1300012"
ms.assetid: 26a7eebb-1424-4ddc-a123-af1cc94bc40f
ms.openlocfilehash: 48d4ccbbc0ed3dc54cbcd17ae7b9040bfd9ecc426897c06b653bf40bc7d5e9b2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952960"
---
# <a name="adfs-federation-certificate-expiring"></a>ADFS 同盟憑證逾期失效

若要解決此問題，請遵循下列步驟：
  
1. 若尚未安裝模組，請在電腦上安裝 Windows PowerShell 的 Microsoft Azure Active Directory 模組 () 。 若要這麼做，請移至[使用 Windows PowerShell 管理 AZURE AD](https://aka.ms/aadposh)。

2. 請遵循「案例1： ad fs token 簽署憑證已過期」一節中的「案例」[當同盟使用者登入 Microsoft 365、Azure 或 Intune 時，[存取網站時發生問題] 錯誤](https://support.microsoft.com/help/2713898/there-was-a-problem-accessing-the-site-error-from-ad-fs-when-a-federat)。

3. 依照 [更新或修復 Microsoft、Azure 或 Intune 中](https://docs.microsoft.com/office365/troubleshoot/security/update-federated-domain-office-365)的同盟網域的設定中的步驟進行。

    若要深入瞭解如何更新同盟憑證，請參閱[更新 Microsoft 365 和 Azure Active Directory 的同盟憑證](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-o365-certs)。
