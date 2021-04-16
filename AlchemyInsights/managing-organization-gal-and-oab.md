---
title: 管理組織的全域通訊清單和離線通訊錄
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002895"
- "5550"
ms.openlocfilehash: c6ad2fcb85ef68c42cea11ebe0d1564e957b4720
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51794823"
---
# <a name="managing-organization-global-address-list-gal-and-offline-address-book-oab"></a><span data-ttu-id="9765b-102">管理組織全域通訊清單 (GAL) 和離線通訊錄 (OAB)</span><span class="sxs-lookup"><span data-stu-id="9765b-102">Managing organization global address list (GAL) and offline address book (OAB)</span></span>

<span data-ttu-id="9765b-103">全域通訊清單 (GAL) 是組織中已啟用郵件功能的物件 (可接收電子郵件的任何收件者類型) 清單。</span><span class="sxs-lookup"><span data-stu-id="9765b-103">A global address list (GAL) is a list of mail-enabled objects (any type of recipient that can receive an email) in the organization.</span></span> <span data-ttu-id="9765b-104">系統會在每個組織中自動建立一個 GAL。</span><span class="sxs-lookup"><span data-stu-id="9765b-104">One GAL is automatically created in every organization.</span></span> <span data-ttu-id="9765b-105">您可以建立額外的 GAL 以依組織或位置區隔使用者，但是一個使用者一次只能看到和使用一個 GAL。</span><span class="sxs-lookup"><span data-stu-id="9765b-105">You can create additional GALs to separate users by organization or location, but a single user can only see and use one GAL at a time.</span></span>

<span data-ttu-id="9765b-106">部分電子郵件用戶端 (例如 Windows 版 Outlook) 會下載 GAL 供離線使用。</span><span class="sxs-lookup"><span data-stu-id="9765b-106">Some email clients, such as Outlook for Windows, download the GAL for offline use.</span></span> <span data-ttu-id="9765b-107">這稱為離線通訊錄 (OAB)。</span><span class="sxs-lookup"><span data-stu-id="9765b-107">This is known as an offline address book (OAB).</span></span> <span data-ttu-id="9765b-108">在 Exchange Online 中，OAB 會每 8 小時更新一次，然後用戶端必須下載它，才能更新其本機 OAB 複本。</span><span class="sxs-lookup"><span data-stu-id="9765b-108">In Exchange online, an OAB is updated only once every 8 hours, and then clients must download it to update their local OAB copy.</span></span> <span data-ttu-id="9765b-109">收件者所做的任何變更，都必須先在 GAL 中顯示，之後才可以在 OAB 中變更。</span><span class="sxs-lookup"><span data-stu-id="9765b-109">Any recipient change has to first be visible in the GAL to later make it to the OAB.</span></span>

<span data-ttu-id="9765b-110">以下是一些常用的 GAL 和 OAB 程序：</span><span class="sxs-lookup"><span data-stu-id="9765b-110">Here are some commonly used GAL and OAB procedures:</span></span>

- <span data-ttu-id="9765b-111">基於多種原因，您可能想要讓某些物件從 GAL 中隱藏。</span><span class="sxs-lookup"><span data-stu-id="9765b-111">For a variety of reasons, you might want some objects to be hidden from the GAL.</span></span> <span data-ttu-id="9765b-112">請參閱[隱藏通訊清單中的收件者](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists)。</span><span class="sxs-lookup"><span data-stu-id="9765b-112">Please see [Hide recipients from address lists](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#hide-recipients-from-address-lists).</span></span>
- <span data-ttu-id="9765b-113">如果您需要為特定使用者群組提供組織 GAL 的自訂檢視，請參閱 [Exchange Online 中的通訊錄原則](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies)。</span><span class="sxs-lookup"><span data-stu-id="9765b-113">If you need to give specific groups of users customized views of the organization's GAL, see [Address book policies in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-book-policies/address-book-policies).</span></span>
- <span data-ttu-id="9765b-114">[在 Exchange Online 中建立全域通訊清單](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list)，並且，若要了解如何使用 GAL 權限，請參閱 [Exchange Online 中的通訊清單](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists)。</span><span class="sxs-lookup"><span data-stu-id="9765b-114">[Create a global address list in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/create-global-address-list) and to learn how to work with GAL permissions, see [Address lists in Exchange Online](https://docs.microsoft.com/exchange/address-books/address-lists/address-lists).</span></span> <span data-ttu-id="9765b-115">請注意，如果您建立新的 GAL，則可能也想要建立新的 OAB。</span><span class="sxs-lookup"><span data-stu-id="9765b-115">Please note that if you create new GALs, you might also want to create a new OAB.</span></span> <span data-ttu-id="9765b-116">請參閱[離線通訊錄程序](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures)。</span><span class="sxs-lookup"><span data-stu-id="9765b-116">See [Offline address book procedures](https://docs.microsoft.com/exchange/address-books/offline-address-books/offline-address-book-procedures).</span></span>
