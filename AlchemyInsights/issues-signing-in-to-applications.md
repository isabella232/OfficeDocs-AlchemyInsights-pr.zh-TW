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
# <a name="issues-signing-in-to-applications"></a><span data-ttu-id="8216c-102">登入應用程式時的問題</span><span class="sxs-lookup"><span data-stu-id="8216c-102">Issues signing in to applications</span></span>

<span data-ttu-id="8216c-103">若要偵測與使用者登入相關的原因或診斷問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="8216c-103">To detect the cause or diagnose problems related to user sign-in, perform the following steps:</span></span>

1. <span data-ttu-id="8216c-104">啟動 [登入診斷](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)。</span><span class="sxs-lookup"><span data-stu-id="8216c-104">Launch the [Sign-in Diagnostic](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
2. <span data-ttu-id="8216c-105">輸入您擁有與使用者、應用程式、登入時間、要求識別碼或相互關聯識別碼有關的詳細資料，尋找要分析的活動。</span><span class="sxs-lookup"><span data-stu-id="8216c-105">Find the event to analyze by entering the details you have about the user, application, time of sign in, request Id, or correlation Id.</span></span>
3. <span data-ttu-id="8216c-106">檢閱診斷結果 - 顯示有關所發生的事件以及可採取哪些動作以進行變更的詳細資料 (如果需要變更的話)。</span><span class="sxs-lookup"><span data-stu-id="8216c-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="8216c-107">下列為登入應用程式時可能會遇到的一些常見問題：</span><span class="sxs-lookup"><span data-stu-id="8216c-107">The following are some common issues you may experience when signing in to applications:</span></span>

1. <span data-ttu-id="8216c-108">您或使用者 **已完成 Azure AD 登入，但卻看到非預期的提示** - 請參閱文章 [在登入應用程式出現未預期的同意提示](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) 以及 [在同意執行應用程式時出現未預期的錯誤](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)。</span><span class="sxs-lookup"><span data-stu-id="8216c-108">You or the user **has complete an Azure AD sign in, but are seeing an unexpected prompt** - See the articles [Unexpected consent prompt when signing in to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) and [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>
2. <span data-ttu-id="8216c-109">您或使用者 **已直接登入應用程式，但無法從自訂入口網站或存取面板上的深層連結登入該應用程式**：請參閱 [疑難排解從 Azure AD [我的應用程式] 登入應用程式問題](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)。</span><span class="sxs-lookup"><span data-stu-id="8216c-109">You or a user **has signed in to an application directly, but can't sign in to it from a deeplink on the custom portal or the access panel**: See [Troubleshoot problems signing in to an application from Azure AD My Apps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).</span></span>
3. <span data-ttu-id="8216c-110">您或使用者 **已完成 Azure AD 登入，但應用程式顯示錯誤訊息，而且不讓使用者完成登入流程**：這個問題是因為應用程式未接受 Azure AD 發出的回應。</span><span class="sxs-lookup"><span data-stu-id="8216c-110">You or a user **has completed an Azure AD sign in, but the application displays an error message and doesn't let the user finish the sign-in flow**: The problem is that the app didn't accept the response that Azure AD issued.</span></span> <span data-ttu-id="8216c-111">請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) 以進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8216c-111">Follow [these steps](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) to troubleshoot.</span></span>
4. <span data-ttu-id="8216c-112">您或使用者 **無法登入已設定為密碼單一登入的非圖庫應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) 以進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8216c-112">You or a user **can’t sign in to a non-gallery application configured for password single sign-on**: Follow the guidance in [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to troubleshoot.</span></span>
5. <span data-ttu-id="8216c-113">您或使用者 **無法登入已設定為密碼單一登入的 Azure AD 圖庫應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) 以進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8216c-113">You or a user **can’t sign in to an Azure AD Gallery application configured for password single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) to troubleshoot.</span></span>
6. <span data-ttu-id="8216c-114">您或使用者 **無法登入 Microsoft 應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) 以進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8216c-114">You or a user **can't sign in to a Microsoft application**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) to troubleshoot.</span></span>
7. <span data-ttu-id="8216c-115">您或使用者 **無法登入已設定為同盟單一登入的非圖庫應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) 以進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8216c-115">You or a user **can't sign in to a non-gallery application configured for federated single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) to troubleshoot.</span></span>
8. <span data-ttu-id="8216c-116">您或使用者 **無法登入已設定為同盟單一登入的 Azure AD 圖庫應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) 以進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8216c-116">You or a user **can't sign in to an Azure AD Gallery application configured for federated single sign-on**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to troubleshoot.</span></span>
9. <span data-ttu-id="8216c-117">您或使用者 **無法登入自訂開發的應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) 以進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8216c-117">You or a user **can't sign in to a custom-developed application**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) to troubleshoot.</span></span>
10. <span data-ttu-id="8216c-118">您或使用者 **無法登入使用 Azure AD 應用程式 proxy 的內部部署應用程式**：請遵循 [下列步驟](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) 以進行疑難排解。</span><span class="sxs-lookup"><span data-stu-id="8216c-118">You or a user **can't sign in to an on-premises application using the Azure AD application proxy**: Follow [these steps](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) to troubleshoot.</span></span>

