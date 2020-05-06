---
title: 管理組織的全域通訊清單和離線通訊錄
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: a7142d68f0197aaca733766daf30fe8a46f13f9e
ms.sourcegitcommit: 8b50994a2979778ce8474ce83bd86b60e7d2cb2f
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/05/2020
ms.locfileid: "44022387"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a>管理組織全域通訊清單 (GAL) 和離線通訊錄 (OAB)

全域通訊清單 (GAL) 是組織中已啟用郵件功能的物件 (可接收電子郵件的任何收件者類型) 清單。 系統會在每個組織中自動建立一個 GAL。 您可以建立額外的 GAL 以依組織或位置區隔使用者，但是一個使用者一次只能看到和使用一個 GAL。

部分電子郵件用戶端 (例如 Windows 版 Outlook) 會下載 GAL 供離線使用。 這稱為離線通訊錄 (OAB)。 在 Exchange Online 中，OAB 會每 8 小時更新一次，然後用戶端必須下載它，才能更新其本機 OAB 複本。 收件者所做的任何變更，都必須先在 GAL 中顯示，之後才可以在 OAB 中變更。

以下是一些常用的 GAL 和 OAB 程序：

- 基於多種原因，您可能想要讓某些物件從 GAL 中隱藏。 請參閱[隱藏通訊清單中的收件者](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)。
- 如果您需要為特定使用者群組提供組織 GAL 的自訂檢視，請參閱 [Exchange Online 中的通訊錄原則](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)。
- [在 Exchange Online 中建立全域通訊清單](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)，並且，若要了解如何使用 GAL 權限，請參閱 [Exchange Online 中的通訊清單](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)。 請注意，如果您建立新的 GAL，則可能也想要建立新的 OAB。 請參閱[離線通訊錄程序](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)。
