---
title: 使用者圖片仍顯示在 Microsoft Teams 組織圖中
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/13/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13834"
- "9007457"
ms.openlocfilehash: be4c6feb55e6b7c4667566946d8d3640cc0ffb1d
ms.sourcegitcommit: b47c6d5e74819b73becaf1dc5eacc72eaf7c1055
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/15/2021
ms.locfileid: "59334364"
---
# <a name="user-picture-still-appears-in-the-microsoft-teams-organization-chart"></a>使用者圖片仍顯示在 Microsoft Teams 組織圖中

如果組織的一或多個個人已遭停用或移除，而其個人檔案相片仍出現在組織圖中，則可能是設定 **ShowInAddressLists** 是設定為 False： 

1. 移至 Microsoft 365 系統管理中心 > [作用中使用者[]](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/users)，然後選取相片仍顯示的使用者。 
1. 選取 [郵件 **]** 索引標籤，並確定 [在全域通訊清單中顯示 **]** 設定為 [否 **]**。

如果將 **ShowInAddressLists** 設為 [否 **]** 無法運作，請檢查下列事項： 

- 使用者可能會從 Exchange 中的收件者清單中顯示。 如需詳細資訊，請參閱[管理 Exchange Online 中的地址清單](https://docs.microsoft.com/exchange/address-books/address-lists/manage-address-lists#use-the-eac-to-hide-recipients-from-address-lists)。 
- 使用者可能會從 Azure Active Directory 的通訊清單中顯示。 如需詳細資訊，請參閱 [[Set-AzureADUser]](https://docs.microsoft.com/powershell/module/azuread/set-azureaduser?view=azureadps-2.0)。 