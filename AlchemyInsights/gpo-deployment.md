---
title: GPO 部署
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "8602"
ms.openlocfilehash: d31f77e70e8456a4076a8146025f1f8ada977a06
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416938"
---
# <a name="gpo-deployment"></a>GPO 部署

Azure Active Directory Domain Services (Azure AD DS) 中使用者和電腦物件的設定通常是使用群組原則物件 (GPO) 進行管理。 Azure AD DS 包含內建 GPO，適用於 AADDC 使用者和 AADDC 電腦容器。 您可以自訂這些內建 GPO，以便視環境需要設定群組原則。 Azure AD DC 系統管理員群組的成員擁有 Azure AD DS 網域中的群組原則管理權限，而且也能建立自訂 GPO 和組織單位 (OU)。 如需哪些群組原則及其運作方式的詳細資訊，請參閱 [群組原則一覽](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-server-2012-R2-and-2012/hh831791(v=ws.11))。

在混合式環境中，內部部署 AD DS 環境中設定的群組原則不會同步處理到 Azure AD DS。 若要在 Azure AD DS 中定義使用者或電腦的組態設定，請編輯其中一個預設 GPO，或建立自訂 GPO。

本文《[管理群組原則](https://docs.microsoft.com/azure/active-directory-domain-services/manage-group-policy)》說明如何安裝群組原則管理工具、如何大量編輯內建的 GPO 以及如何建立自訂 GPO。
