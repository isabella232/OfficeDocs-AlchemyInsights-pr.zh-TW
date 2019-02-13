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
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: dd6d6986b23c8adcc98fe713bacf32fb5bf8b4b6
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29915554"
---
# <a name="configure-sync-features"></a>設定同步處理功能

Azure AD 連接包含數項功能的啟用根據預設，或您可以稍後啟用。有些功能需要特定的環境中的其他設定。
  
- [篩選](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering)限制物件已同步處理至 Azure AD。依預設，所有使用者、 連絡人、 群組及 Windows 10 進行同步處理電腦帳戶。您可以包含或排除物件根據網域、 Ou、 或其他屬性。 
    
- [密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization)會從內部部署 Active Directory 至 Azure AD 的密碼雜湊同步處理。這可讓密碼管理的單一位置，但是相同的密碼中同時使用內部部署和雲端環境。因為 Active Directory 的授權來源，您可以使用自己的密碼原則。 
    
- [自助式密碼重設 (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr)可讓使用者在雲端自己密碼重設時仍套用您內部部署的密碼原則。 
    
- [裝置回寫](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback)可寫入回內部部署 Active Directory 讓他們可以用於設定格式化的條件存取 Azure AD 中的已登錄的裝置。 
    
- [避免意外刪除](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes)預設會啟用以協助防止太多同時物件刪除 （同步處理個別超過 500 個物件）。您可以變更此設定可符合組織的需求。 
    
- Express 安裝預設會啟用[自動升級](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade)並有助於確保您的 Azure AD 連接版本永遠是最新。 
    

