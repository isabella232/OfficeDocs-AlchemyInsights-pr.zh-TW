---
title: 查詢 Microsoft Graph API
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004345"
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923230"
---
# <a name="querying-the-microsoft-graph-api"></a>查詢 Microsoft Graph API

本主題也適用于仍在使用 Azure AD Graph API 的開發人員。 不過，**強烈** 建議您針對所有目錄、身分識別和存取管理案例使用 Microsoft Graph。

**驗證或授權問題**

- 如果您的應用程式 **無法取得標記** 以撥打 Microsoft Graph，請選擇 **取得存取權杖 (驗證)** Microsoft Graph 類別，以取得更多特定的說明和支援，以取得本主題。
- 當呼叫 Microsoft Graph 時，如果您的應用程式 **收到401或403授權錯誤**，請選擇 [**取得存取權被拒絕] 錯誤 (授權)** Microsoft Graph API 類別，以取得更多特定的說明和支援此主題。

**我想要使用 Microsoft Graph，但不確定開始的位置**

若要深入瞭解 Microsoft Graph，請參閱：

- [Microsoft Graph 概觀](https://docs.microsoft.com/graph/overview)
- [Microsoft Graph 中的身分識別與存取管理綜述](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [建立 Microsoft Graph 應用程式的快速入門](https://docs.microsoft.com/graph/)
- **microsoft Graph Explorer** -測試您租使用者或示範租使用者中的 Microsoft Graph APIs

**我想要使用 Microsoft Graph，但是它是否支援我需要的1.0 版目錄 APIs？**

Microsoft Graph 是目錄、身分識別和存取管理的建議 API。 不過，Azure AD Graph 和 Microsoft Graph 中的可能仍然有一些差距。 請參閱下列文章，這些文章會反白顯示最新的差異，以協助您選擇：

- [Azure AD Graph 和 Microsoft Graph 之間的資源類型差異](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Azure AD Graph 和 Microsoft Graph 之間的屬性差異](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD 和 Microsoft Graph 之間的方法差異](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**當我查詢 *使用者* 物件時，它的許多屬性都缺失**

`GET https://graph.microsoft.com/v1.0/users`只會傳回11個屬性，因為 Microsoft Graph 會自動選取要傳回的預設 *使用者* 屬性集。 如果您需要其他 *使用者* 屬性，請使用 $select 來挑選您的應用程式所需的屬性。 請先在 **Microsoft Graph Explorer** 中嘗試。

**部分使用者屬性值為 *null* ，即使我知道已經設定**

最可能的說明是已授與 *ReadBasic 所有* 許可權的應用程式。 這可讓應用程式讀取一組有限的使用者屬性，將所有其他屬性都傳回 null，即使先前已經設定。 嘗試授予應用程式 *使用者。* 請改為讀取權限。

如需詳細資訊，請參閱[Microsoft Graph 使用者](https://docs.microsoft.com/graph/permissions-reference#user-permissions)權力。

**在我的要求中使用 OData 查詢參數篩選資料時遇到問題**

雖然 microsoft Graph 支援廣泛的 OData 查詢參數，但這些參數中的許多參數並不完全支援從 Microsoft Graph 繼承 *directoryObject*) 的目錄服務 (資源。 在 Microsoft Graph 中，Azure AD Graph 中所提供的限制，都存在於大部分：

1. **不支援：不支援** *null* 或 *非 null* 值的 $count、$search 及 $filter
2. **不支援**：在特定屬性 $filter (請參閱可篩選屬性的資源主題) 
3. **不支援**：同時分頁、篩選和排序
4. **不支援**：在關聯上篩選。 例如，尋找 UK 中工程群組的所有成員。
5. **部分支援**： *user* (displayName 上的 $orderby，並只 userPrincipalName) 與 *群組*
6. **部分支援**： $filter (僅支援 *eq*、 *startswith*、  *and 和* 有限的 *任何*) 支援，$expand (擴充單一物件的關聯性會傳回所有關聯，但展開物件的關聯集合會受到限制) 

如需詳細資訊，請參閱 [使用查詢參數自訂回應](https://docs.microsoft.com/graph/query-parameters)。

**我所呼叫的 API 沒有作用-我可以在哪裡進行其他測試？**

**microsoft Graph Explorer** -測試您租使用者或示範租使用者中的 microsoft Graph APIs，也請參閱 Microsoft Graph Explorer 中的 **範例查詢**。

**當我查詢資料時，我似乎沒有完整的資料集回復**

如果您正在查詢集合 (如 *使用者*) 所示，Microsoft Graph 使用伺服器端的頁面限制，因此會永遠以預設頁面大小傳回結果。 您的應用程式應該會永遠預計會從服務傳回的集合逐步分頁。

如需詳細資訊，請參閱：

- [Microsoft Graph 最佳作法](https://docs.microsoft.com/graph/best-practices-concept)
- [在您的應用程式中分頁 Microsoft Graph 資料](https://docs.microsoft.com/graph/paging)

**我的應用程式速度太慢，也遭到節流。我可以進行哪些改進？**

視您的案例而定，您可以使用各種不同的選項，讓應用程式更具能力，在某些情況下，當您) 進行許多呼叫時，可能會降低服務 (的限制。

若要深入了解，請參閱：

- [Microsoft Graph 最佳作法](https://docs.microsoft.com/graph/best-practices-concept)
- [批次處理要求](https://docs.microsoft.com/graph/json-batching)
- [透過增量查詢追蹤變更](https://docs.microsoft.com/graph/delta-query-overview)
- [透過 webhooks 取得變更的通知](https://docs.microsoft.com/graph/webhooks)
- [節流指導](https://docs.microsoft.com/graph/throttling)

**在哪裡可以找到錯誤和已知問題的詳細資訊？**

- [Microsoft Graph 錯誤回應資訊](https://docs.microsoft.com/graph/errors)
- [Microsoft Graph 的已知問題](https://docs.microsoft.com/graph/known-issues)

**我可以在哪裡檢查服務可用性和線上狀態？**

可透過 microsoft Graph 存取之基礎服務的服務可用性和連線能力會影響 microsoft Graph 的整體可用性和效能。

- 若為 Azure Active Directory 服務健康情況，請檢查 [ [Azure 狀態] 頁面](https://azure.microsoft.com/status/)中列出的 [**安全性 + 身分識別** 服務] 狀態。
- 針對參與 Microsoft Graph 的 Office 服務，請檢查 [ [Office 服務健康情況] 儀表板](https://portal.office.com/adminportal/home#/servicehealth)中所列服務的狀態。
