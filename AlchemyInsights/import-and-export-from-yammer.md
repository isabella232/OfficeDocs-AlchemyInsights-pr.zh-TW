---
title: 從 Yammer 匯入和匯出
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9735"
- "9003224"
ms.openlocfilehash: dcdf569f96e51a62899761589ef6f9f317517c3a
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897727"
---
# <a name="import-and-export-from-yammer"></a><span data-ttu-id="16e51-102">從 Yammer 匯入和匯出</span><span class="sxs-lookup"><span data-stu-id="16e51-102">Import and export from Yammer</span></span>

<span data-ttu-id="16e51-103">**匯入**</span><span class="sxs-lookup"><span data-stu-id="16e51-103">**Import**</span></span>

<span data-ttu-id="16e51-104">使用者匯入選項會根據您的 Yammer 網路是[適用於 Microsoft 365 的原生模式](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode)與否而有所不同。</span><span class="sxs-lookup"><span data-stu-id="16e51-104">User-import options vary depending on whether your Yammer network is in [Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/overview-native-mode), or not.</span></span>

- <span data-ttu-id="16e51-105">**非原生模式**：可以使用群組設定內的[從通訊錄新增](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (限制為 100 個使用者) 將使用者匯入到群組，或使用網路系統管理員內的[大量更新](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users)，將使用者匯入到網路。</span><span class="sxs-lookup"><span data-stu-id="16e51-105">**Non-Native Mode**: Users can be imported to groups using [Add from Address Book](https://support.microsoft.com/office/manage-yammer-community-members-75253554-d0f3-4148-b835-e6a9a8a0c294) (limit to 100 users) within group settings, or to the network using [Bulk Update](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users) within Network Admin.</span></span>
- <span data-ttu-id="16e51-106">**原生模式**：群組成員資格和網路成員資格作業應該從 [Microsoft 365 系統管理入口網站](https://docs.microsoft.com/microsoft-365/admin/add-users)、[Azure AD 入口網站](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)，或是使用另一個 Azure AD 選項執行。</span><span class="sxs-lookup"><span data-stu-id="16e51-106">**Native Mode**: Group membership and network membership operations should be performed from the [Microsoft 365 admin portal](https://docs.microsoft.com/microsoft-365/admin/add-users), [Azure AD portal](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory), or using another Azure AD option.</span></span> <span data-ttu-id="16e51-107">原生模式的網路無法再存取大量更新和其他舊版功能。</span><span class="sxs-lookup"><span data-stu-id="16e51-107">Networks in Native Mode no longer have access to Bulk Update and other legacy features.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="16e51-108">Yammer 從未支援匯入來自網路系統管理員的內容，即使資料匯出功能已用於其他網路也一樣。</span><span class="sxs-lookup"><span data-stu-id="16e51-108">Yammer never supported importing content from within Network Admin even when the Data Export feature was used in another network.</span></span> <span data-ttu-id="16e51-109">合作夥伴解決方案或 Yammer REST API 可以重新發佈內容。</span><span class="sxs-lookup"><span data-stu-id="16e51-109">Content can be re-posted by partner solutions or the Yammer REST APIs.</span></span>

<span data-ttu-id="16e51-110">**匯出**</span><span class="sxs-lookup"><span data-stu-id="16e51-110">**Export**</span></span>

<span data-ttu-id="16e51-111">[匯出網路系統管理員內的網路資料](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data)，允許從 Yammer 網路匯出內容，包括訊息和檔案。</span><span class="sxs-lookup"><span data-stu-id="16e51-111">[Export Network Data within Network Admin](https://docs.microsoft.com/yammer/manage-security-and-compliance/export-yammer-enterprise-data) permits the export of content from Yammer networks, including messages and files.</span></span> <span data-ttu-id="16e51-112">附件可能會非常龐大，且會導致匯出需要大量時間才能完成。</span><span class="sxs-lookup"><span data-stu-id="16e51-112">Attachments can be extremely large and will cause exports to take significant time to complete.</span></span> <span data-ttu-id="16e51-113">我們建議使用[資料匯出 API](https://developer.yammer.com/docs/data-export-api)，依日或週以區塊匯出使用中網路。</span><span class="sxs-lookup"><span data-stu-id="16e51-113">We recommend that active networks are exported using the [Data Export API](https://developer.yammer.com/docs/data-export-api) in chunks by day or week.</span></span> <span data-ttu-id="16e51-114">Microsoft 支援服務不會為此目的提供自訂指令碼。</span><span class="sxs-lookup"><span data-stu-id="16e51-114">Microsoft Support does not provide custom scripts for this purpose.</span></span>

<span data-ttu-id="16e51-115">有個別 [GDPR 匯出](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise)，匯出個別使用者的內容。</span><span class="sxs-lookup"><span data-stu-id="16e51-115">A separate [GDPR export](https://docs.microsoft.com/yammer/manage-security-and-compliance/gdpr-requests-in-yammer-enterprise) exists to export content for an individual user.</span></span>