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
# <a name="configure-mim-sync-service"></a>設定 MIM 同步處理服務

Microsoft Identity Manager (MIM) 同步處理服務是 MIM 的元件。 其為集中式內部部署服務，可儲存及整合具有多個內部部署目錄和資料庫的組織資訊。 如果 MIM 最近的更新已解決問題，或包含於下一節提及的其他問題，您或許可以使用 MIM 同步處理解決問題。

**建議的步驟**

1. 確定您使用的是 MIM 同步處理的最新更新，並查看 [MIM Sync 版本資訊](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history)以判斷更新中的問題是否解決。
2. 如果問題發生在 Generic LDAP、Generic SQL、Lotus Domino 或 Web Services 連接器上，請確保您使用的是[一般連接器](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history)的最新更新。
3. 如果 MIM 同步執行因發生錯誤而停止，請參閱[執行錯誤碼](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes)表格，以判斷可能的原因。
4. 如果執行因發生 **extension-dll-exception** 而停止，請按一下這些文字以開啟 **[接器空間物件屬性]** 視窗，然後按一下 **[堆疊追蹤...]** 以查看關於根本原因的詳細資訊，如 [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx) 所述。
5. 如果密碼變更通知服務 (PCNS) 元件在密碼同步處理期間於事件記錄中報告 **錯誤 6025**，請查看疑難排解指南 [PCNS 報告錯誤 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx)。
6. 如果 FIM 服務管理代理程式的完整同步處理速度緩慢，請檢查 TempDB 的 **[auto grow]** 設定，如[完整同步處理緩慢或當機的疑難排解](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx)所述。
7. 如果您使用 FIM 服務管理代理程式時遇到「failed-creation-via-web-services」伺服器停止的錯誤，請參閱[支援資訊：failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) 以瞭解原因概觀。

