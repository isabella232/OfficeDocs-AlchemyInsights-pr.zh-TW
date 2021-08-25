---
title: Microsoft Teams 組織結構圖中未顯示的使用者圖片
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/23/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "12620"
- "9007457"
ms.openlocfilehash: 661b04913581ddd6650316298134ff9835ef3a90
ms.sourcegitcommit: 3986fa5377895cfc9fd98aca0739e599ebafb712
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/23/2021
ms.locfileid: "58467369"
---
# <a name="user-picture-not-showing-in-microsoft-teams-organization-chart"></a>Microsoft Teams 組織結構圖中未顯示的使用者圖片

如果組織中的一個或多個個人在組織結構圖中遺失其設定檔相片，則設定 **ShowInAddressLists** 可能會設定為 **False**：

1. 移至 [Microsoft 365 系統管理中心] > [**[作用中使用者]**](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)，然後選取遺失相片的使用者。 
1. 選取 **[郵件]** 索引標籤，並確定 **[全域通訊清單中的顯示]** 設定為 **[是]**。 

如果將 **ShowInAddressLists** 設為 **[是]** 無法運作，請檢查下列事項：

- 使用者可能會從 Exchange 中的收件者清單中隱藏。 如需詳細資訊，請參閱[[管理 Exchange Online 中的地址清單]](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)。 
- 使用者可能會從 Azure Active Directory 的通訊清單中隱藏。 如需詳細資訊，請參閱 [[Set-AzureADUser]](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)。 
