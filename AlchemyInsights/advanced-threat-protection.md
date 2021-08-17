---
title: 適用於 Office 365 的 Microsoft Defender
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1036
ms.assetid: ''
ms.openlocfilehash: 61236d1e0174248cdb49284d6c6c7d49df51e7e9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/13/2021
ms.locfileid: "58315069"
---
# <a name="microsoft-defender-for-office-365"></a>適用於 Office 365 的 Microsoft Defender

- 保管庫附件、保管庫連結和反網路釣魚屬於 Office 365 的 Microsoft Defender 的一部分。 EnterpriseE5、教育版 A5 和 Microsoft 365 商務進階版包含適用于 Office 365 的 Microsoft Defender。 所有其他計畫都需要增益集的 Microsoft Defender Office 365 訂閱。

- 您需要指派適當的授權，以保護您的使用者，以供 Office 365 的 Microsoft Defender 使用。 請參閱 [同時新增使用者並指派授權](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users) ，以取得將授權大量套用給使用者的指示。

- 全域管理員或安全性管理員可以在 **電子郵件 & 共同作業區段** \> **原則 & 規則** \> **威脅原則** 中，存取 Microsoft 365 Defender 入口網站中 Office 365 功能的 Microsoft Defender。

- 保管庫附件和保管庫連結原則可以設定為特定網域、群組成員或個別使用者的範圍。 您也可以根據網域、群組成員資格或個別使用者，指定保管庫附件和保管庫連結原則的例外狀況。

- 沒有預設的保管庫附件原則可以保護電子郵件。 您需要在電子郵件中建立保管庫附件保護的[原則](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-attachments-policies)。

  保管庫SharePoint、OneDrive 及 Microsoft Teams 的附件會以全域方式啟用或停用，而且不需要保管庫附件原則。 如需詳細資訊，請參閱[保管庫 SharePoint、OneDrive 和 Microsoft Teams 的附件](https://docs.microsoft.com/microsoft-365/security/office-365-security/mdo-for-spo-odb-and-teams)。

- 沒有預設的保管庫連結原則可以保護電子郵件或 Microsoft Teams。 您必須在電子郵件和 Teams 中建立保管庫連結保護的[原則](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)。

  保管庫Office 365 應用程式的連結保護會套用至組織中所有授權使用 Office 365 的使用者，不論是否包含在使用中保管庫連結原則中的使用者。 如需詳細資訊，請參閱[保管庫連結設定 Office 365 應用程式](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-links#safe-links-settings-for-office-365-apps)。
