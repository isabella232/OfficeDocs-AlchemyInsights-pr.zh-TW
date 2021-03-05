---
title: 設定 MIM 同步處理服務
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50430721"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="c1188-102">設定 MIM 同步處理服務</span><span class="sxs-lookup"><span data-stu-id="c1188-102">Configure MIM Sync service</span></span>

<span data-ttu-id="c1188-103">Microsoft Identity Manager (MIM) 同步處理服務是 MIM 的元件。</span><span class="sxs-lookup"><span data-stu-id="c1188-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="c1188-104">其為集中式內部部署服務，可儲存及整合具有多個內部部署目錄和資料庫的組織資訊。</span><span class="sxs-lookup"><span data-stu-id="c1188-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="c1188-105">如果 MIM 最近的更新已解決問題，或包含於下一節提及的其他問題，您或許可以使用 MIM 同步處理解決問題。</span><span class="sxs-lookup"><span data-stu-id="c1188-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="c1188-106">**建議的步驟**</span><span class="sxs-lookup"><span data-stu-id="c1188-106">**Recommended steps**</span></span>

1. <span data-ttu-id="c1188-107">確定您使用的是 MIM 同步處理的最新更新，並查看 [MIM Sync 版本資訊](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history)以判斷更新中的問題是否解決。</span><span class="sxs-lookup"><span data-stu-id="c1188-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="c1188-108">如果問題發生在 Generic LDAP、Generic SQL、Lotus Domino 或 Web Services 連接器上，請確保您使用的是[一般連接器](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)的最新更新。</span><span class="sxs-lookup"><span data-stu-id="c1188-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="c1188-109">如果 MIM 同步執行因發生錯誤而停止，請參閱[執行錯誤碼](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes)表格，以判斷可能的原因。</span><span class="sxs-lookup"><span data-stu-id="c1188-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="c1188-110">如果執行因發生 **extension-dll-exception** 而停止，請按一下這些文字以開啟 **[接器空間物件屬性]** 視窗，然後按一下 **[堆疊追蹤...]** 以查看關於根本原因的詳細資訊，如 [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) 所述。</span><span class="sxs-lookup"><span data-stu-id="c1188-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="c1188-111">如果密碼變更通知服務 (PCNS) 元件在密碼同步處理期間於事件記錄中報告 **錯誤 6025**，請查看疑難排解指南 [PCNS 報告錯誤 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)。</span><span class="sxs-lookup"><span data-stu-id="c1188-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="c1188-112">如果 FIM 服務管理代理程式的完整同步處理速度緩慢，請檢查 TempDB 的 **[auto grow]** 設定，如[完整同步處理緩慢或當機的疑難排解](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)所述。</span><span class="sxs-lookup"><span data-stu-id="c1188-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="c1188-113">如果您使用 FIM 服務管理代理程式時遇到「failed-creation-via-web-services」伺服器停止的錯誤，請參閱[支援資訊：failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) 以瞭解原因概觀。</span><span class="sxs-lookup"><span data-stu-id="c1188-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

