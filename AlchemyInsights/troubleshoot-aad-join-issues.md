---
title: Azure AD 聯結問題疑難排解
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "6157"
ms.openlocfilehash: 8e902aea30e6891717e08027cc009576d390c9cf2ba1649cbbc68d64883937f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939910"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Azure AD 聯結問題疑難排解

1. 如果您是第一次設定裝置註冊，請確定您已在[Azure Active Directory 中查看裝置管理的簡介](https://docs.microsoft.com/azure/active-directory/devices/overview)，以指導您如何在 Azure AD 的控制項下取得裝置。 
1. 如果您直接向 Azure AD 註冊裝置，並將其註冊到 Intune，您必須確定您已 [設定 intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) 並且先進行 [授權](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) 。
1. 確定您有權在 Azure AD 中執行作業。 只有 Azure AD 中的全域系統管理員可以管理裝置註冊的設定。
1. 若要執行 Azure AD 加入實施，請參閱 [Plan AZURE Ad join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)。

如需解決 azure ad join 常見問題的詳細資訊，請參閱[azure ad 聯結常見問題](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq)和 Windows 10 pro 裝置的相關資訊，請參閱[無法將 Windows 10 專業版機器加入 Azure AD-必須升級至-Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
