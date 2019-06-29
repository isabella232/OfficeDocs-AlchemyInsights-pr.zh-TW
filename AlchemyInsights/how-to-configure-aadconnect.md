---
title: 646如何設定 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 0569cb10c1d1dd422709de5d2569e43ee9d75386
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/28/2019
ms.locfileid: "35385321"
---
# <a name="configure-sync-features"></a>設定同步處理功能

Azure AD Connect 包含若干預設啟用的功能, 或您可以稍後啟用的功能。 某些功能需要在特定環境中進行其他設定。

- [篩選](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)會限制將物件同步處理至 Azure AD。 依預設, 會同步處理所有使用者、連絡人、群組及 Windows 10 電腦帳戶。 您可以根據網域、Ou 或其他屬性來包含或排除物件。

- [密碼雜湊同步](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)處理會將密碼雜湊從內部部署 Active Directory 同步處理至 Azure AD。 這可讓您在一個位置使用密碼管理, 但在內部部署和雲端環境中使用相同的密碼。 因為 Active Directory 是授權來源, 您可以使用自己的密碼原則。

- [自助密碼重設 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)可讓使用者在自己的內部部署密碼原則中重設自己在雲端中的密碼。

- [裝置回寫](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)允許 Azure AD 中的註冊裝置被寫回至內部部署 Active Directory, 讓它們可用於條件式存取。

- [防止意外刪除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)預設為啟用, 以協助防止過多的同時刪除物件 (每個同步處理500個以上的物件)。 您可以變更此設定, 以符合組織的需求。

- 預設會為快速安裝啟用[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade), 並協助確保您的 Azure AD Connect 版本永遠是最新的。
