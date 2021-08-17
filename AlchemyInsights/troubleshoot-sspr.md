---
title: 疑難排解 SSPR
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.topic: article
ms.audience: Admin
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003259"
- "6128"
ms.openlocfilehash: 9d8184efdc60befd359059c62ea3eb1a14ad7d2a20dade921d4a71e424f52033
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54038949"
---
# <a name="troubleshoot-sspr"></a>疑難排解 SSPR

**設定密碼重設時有問題**

- 如果您是系統管理員，並尋找如何啟用自助密碼重設，請參閱 [教學課程啟用 SSPR](https://docs.microsoft.com/azure/active-directory/authentication/tutorial-enable-sspr)，為您的組織設定密碼重設。 您也可能想要複查 [授權要求](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-licensing?WT.mc_id=Portal-Microsoft_Azure_Support)。 您的組織中必須至少有一個指派的授權。
    - **僅限雲端使用者**-任何 Office 365 (O365) 付費 SKU 或 Azure AD Basic
    - **雲端和/或內部部署使用者**-Azure AD Premium P1 或 P2、Enterprise Mobility + Security (EMS) 或 Secure Productive Enterprise (SPE) 
- 如需有關自助密碼重設的其他問題，請參閱 [我們的常見問題解答](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-faq?WT.mc_id=Portal-Microsoft_Azure_Support)。

**我收到錯誤訊息**

請參閱本文以尋找常見的錯誤及其解決方法： [自助密碼重設疑難排解](https://docs.microsoft.com/azure/active-directory/authentication/active-directory-passwords-troubleshoot?WT.mc_id=Portal-Microsoft_Azure_Support)

**密碼重設原則發生問題**

- 如果您的密碼重設原則行為意外，或是您有有關密碼重設原則的問題，請參閱本文： [Azure Active Directory 中的密碼原則和限制](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support)。
- 密碼重設原則不適用於管理員。 Microsoft 對任何 Azure 系統管理員角色強制實施強預設雙門密碼重設原則。 確定您正在使用非系統管理員的使用者進行測試。 如需系統管理員重設原則的詳細資訊，請參閱下列文章： [系統管理員重設原則差異](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy?WT.mc_id=Portal-Microsoft_Azure_Support#administrator-reset-policy-differences)。

**我不想要讓使用者註冊其他安全性資訊以進行密碼重設**

您可以使用 API、PowerShell 或 Azure AD 連線，為使用者預先填入 (電子郵件和電話屬性) 的資料。 若要深入瞭解，請參閱：

- [部署密碼重設，但不需要使用者註冊](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support#set-and-read-authentication-data-using-powershell)
- [密碼重設所使用的資料](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-data?WT.mc_id=Portal-Microsoft_Azure_Support)

**我想要讓使用者註冊其其他安全性資訊以進行密碼重設**

1. 讓您的使用者向 [aka.ms/ssprsetup](https://mysignins.microsoft.com/security-info)註冊自助服務密碼重設的安全性資訊。
1. 在使用者或由系統管理員) 為使用者 (填入資料後，請指引使用者 [aka.ms/sspr](https://passwordreset.microsoftonline.com/) ，讓使用者可以自行重設自己的密碼。
1. 如果使用者仍遇到問題，表示他們 **最可能是** 同盟或 **密碼雜湊同步** 使用者。 這表示密碼寫回服務可能發生問題。