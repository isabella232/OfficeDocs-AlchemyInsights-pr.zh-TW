---
title: 複本集
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 45cf530c3258fa3c7008c3e8251fdb7b74be6911d0487f58c5ce2530e25ca282
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54110671"
---
# <a name="replica-set"></a>複本集

AADDS 也稱為受管理的網域。 這實際上是兩個由後端執行及維護的網域控制站。 這兩個 Dc 包含一個主要 DC 和一個複寫 DC。 AADDS (managed domain) 中的備份是由 Azure 平臺所管理的自動程式。 在受管理的網域發生問題時，Azure 支援可協助您從備份還原。

您可以在虛擬網路中建立每個複本集。 每個虛擬網路都必須 peered 到主控受管理網域之複本集的其他每個虛擬網路。 這種設定會建立支援目錄複寫的網狀網路拓朴。 虛擬網路可支援多個複本集，只要每個複本集位於不同的虛擬子網中。

如需複本集的詳細資訊，請參閱 [概念複本集](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)。
