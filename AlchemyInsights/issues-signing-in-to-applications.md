---
title: 登入應用程式時的問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49886801"
---
# <a name="issues-signing-in-to-applications"></a>登入應用程式時的問題

若要偵測與使用者登入相關的原因或診斷問題，請執行下列步驟：

1. 啟動 [登入診斷](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。
2. 輸入您擁有與使用者、應用程式、登入時間、要求識別碼或相互關聯識別碼有關的詳細資料，尋找要分析的活動。
3. 檢閱診斷結果 - 顯示有關所發生的事件以及可採取哪些動作以進行變更的詳細資料 (如果需要變更的話)。

下列為登入應用程式時可能會遇到的一些常見問題：

1. 您或使用者 **已完成 Azure AD 登入，但卻看到非預期的提示** - 請參閱文章 [在登入應用程式出現未預期的同意提示](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) 以及 [在同意執行應用程式時出現未預期的錯誤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。
2. 您或使用者 **已直接登入應用程式，但無法從自訂入口網站或存取面板上的深層連結登入該應用程式**：請參閱 [疑難排解從 Azure AD [我的應用程式] 登入應用程式問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)。
3. 您或使用者 **已完成 Azure AD 登入，但應用程式顯示錯誤訊息，而且不讓使用者完成登入流程**：這個問題是因為應用程式未接受 Azure AD 發出的回應。 請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) 以進行疑難排解。
4. 您或使用者 **無法登入已設定為密碼單一登入的非圖庫應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) 以進行疑難排解。
5. 您或使用者 **無法登入已設定為密碼單一登入的 Azure AD 圖庫應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) 以進行疑難排解。
6. 您或使用者 **無法登入 Microsoft 應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) 以進行疑難排解。
7. 您或使用者 **無法登入已設定為同盟單一登入的非圖庫應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) 以進行疑難排解。
8. 您或使用者 **無法登入已設定為同盟單一登入的 Azure AD 圖庫應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) 以進行疑難排解。
9. 您或使用者 **無法登入自訂開發的應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) 以進行疑難排解。
10. 您或使用者 **無法登入使用 Azure AD 應用程式 proxy 的內部部署應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) 以進行疑難排解。

