---
title: 646 如何設定 AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 44b2532c634bf17d87c562f9506cc1e81cc7e84a
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/23/2019
ms.locfileid: "32399762"
---
# <a name="configure-sync-features"></a>設定同步處理功能

Azure AD Connect 包含數個功能，已啟用根據預設，或更新版本，您可以啟用。 有些功能需要在特定環境的其他設定。

- [篩選](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)限制物件同步處理到 Azure AD。 依預設，所有使用者、 連絡人、 群組及 Windows 10 電腦帳戶已同步處理。 您可以包含或排除依據網域、 Ou、 或其他屬性的物件。

- [密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)會同步處理到 Azure AD 從內部部署 Active Directory 密碼雜湊。 這可讓密碼管理在一個位置，但使用相同的密碼，在這兩個內部部署和雲端環境。 因為 Active Directory 的授權來源，您可以使用您自己的密碼原則。

- [自助式密碼重設 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)允許使用者自行重設密碼定域機組中的時，仍然套用您內部部署的密碼原則。

- [裝置寫回](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)寫回至內部部署 Active Directory 讓他們可以使用條件式存取的 Azure AD 中允許已註冊的裝置。

- [防止意外刪除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)預設會啟用，協助防範太多同時刪除的物件 （同步處理每個超過 500 個物件）。 您可以變更此設定以符合組織的需求。

- 快速安裝預設會啟用[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)，以協助確保您的 Azure AD Connect 版本永遠是最新。
