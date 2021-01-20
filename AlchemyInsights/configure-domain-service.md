---
title: 設定網域服務
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
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884567"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a>無法啟用 AAD-DS 或部署失敗

若要解決 Azure AD Domain Services (AAD-DS) 未啟用或無法部署的問題，請執行下列步驟：

1. 如果您使用的是現有的虛擬網路，請檢查您的 NSG 是否有針對入口網站 https://aka.ms/aadds-networking 中需在 AAD-DS 中同步處理的連接埠封鎖規則。
2. 請檢查您的錯誤訊息是否在 https://aka.ms/aadds-troubleshoot-enable 中提供的疑難排解指南中得到回覆。
3. 嘗試在新的虛擬網路中部署 Azure AD Domain Services。
4. 根據快速入門手冊以了解如何部署 AAD-DS：[建立及設定 AAD 網域服務](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)。
5. 如果您在部署 Azure AD Domain Services 時發生問題，請參閱 [疑難排解 Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) 以解決常見錯誤即協助您再次進行工作。 

**無法停用 AAD-DS**

無法暫停 AAD-DS。 如果您想要停止使用受管理的網域，必須先將它刪除。
若要刪除受管理的網域，請參閱 [刪除 AAD 網域服務](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds)。



