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
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403821"
---
# <a name="troubleshoot-azure-ad-join-issues"></a>Azure AD 聯結問題疑難排解

1. 如果您是第一次設定裝置註冊，請確定您已在 [Azure Active Directory 中查看裝置管理的簡介](https://docs.microsoft.com/azure/active-directory/devices/overview) ，它會引導您瞭解如何在 azure AD 的控制項下取得裝置。 
1. 如果您直接向 Azure AD 註冊裝置，並將其註冊到 Intune，您必須確定您已 [設定 intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) 並且先進行 [授權](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) 。
1. 確定您有權在 Azure AD 中執行作業。 只有 Azure AD 中的全域系統管理員可以管理裝置註冊的設定。
1. 若要執行 Azure AD 加入實施，請參閱 [Plan AZURE Ad join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)。

如需解決 Azure AD join 常見問題的詳細資訊，請參閱 [Azure Ad JOIN 常見問題](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) 和 Windows 10 專業版裝置，請參閱 [無法將 Windows 10 專業版電腦加入 Azure ad-需要升級至 Microsoft 社區](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)
