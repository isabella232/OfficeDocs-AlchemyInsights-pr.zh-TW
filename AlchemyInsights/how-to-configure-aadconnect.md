---
title: 646如何設定 AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704480"
---
# <a name="configure-sync-features"></a>設定同步處理功能

Azure AD Connect 包含許多預設已啟用的功能，也就是您可以稍後啟用的功能。 有些功能需要在特定環境中進行其他設定。

- [篩選](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) 限制將物件同步處理到 Azure AD。 依預設，會同步處理所有的使用者、連絡人、群組和 Windows 10 電腦帳戶。 您可以根據網域、Ou 或其他屬性包含或排除物件。

- [密碼雜湊同步](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) 處理會將內部部署 Active Directory 的密碼雜湊同步處理到 Azure AD。 這允許在一個位置使用密碼管理，但在內部部署和雲端環境中使用相同的密碼。 因為 Active Directory 是授權來源，所以您可以使用您自己的密碼原則。

- [自助密碼重設 (SSPR) ](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) 可讓使用者在自己的內部部署密碼原則的情況下，在雲端中重設自己的密碼。

- [裝置回寫](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) 允許將 Azure AD 中的註冊裝置寫回內部部署 Active Directory，以供使用者用來進行條件式存取。

- [[防止意外刪除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)] 預設會啟用，以協助防止同步處理同時刪除的物件 (每個同步處理) 超過500個物件。 您可以變更此設定，以符合組織的需求。

- 預設會為快速安裝啟用[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)，並協助確保您的 Azure AD Connect 版本永遠都是最新的。
