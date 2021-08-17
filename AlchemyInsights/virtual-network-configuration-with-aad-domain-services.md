---
title: 使用 AAD 網域服務的虛擬組態
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 03a6ec63ba8e2779b0fe3f0381606af2c0748f8b848baaa7cd88b61317bd7a5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54072835"
---
# <a name="virtual-configuration-with-aad-domain-services"></a>使用 AAD 網域服務的虛擬組態

使用 AAD 網域服務的虛擬組態涉及下列步驟： 

1. 正在檢查 [Microsoft Azure 入口網站] 上您的網域健康情況 https://aka.ms/aadds-health
2. 正在檢查您的 NSG 是否有針對入口網站上的 Azure AD Domain Services 同步處理的連接埠進行封鎖的規則 https://aka.ms/aadds-networking
3. 確保您的虛擬網路部署在與管理 Azure AD Domain Services 網域相同的 Azure 區域。
4. 確保您擁有的現有網域名稱並未與虛擬網路使用的網域名稱相同。

如需有關 Azure 虛擬網路與支援 AAD 網域服務的 的設計考量詳細資訊，請參閱 [虛擬網路考量](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations)。

