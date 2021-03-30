---
title: Azure Active Directory 加入
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
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403782"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="da72a-102">Azure Active Directory 加入</span><span class="sxs-lookup"><span data-stu-id="da72a-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="da72a-103">如果您是第一次設定裝置註冊，請確定您已在 [Azure Active Directory 中查看裝置管理的簡介](/azure/active-directory/devices/overview) ，它會引導您瞭解如何在 azure AD 的控制項下取得裝置。</span><span class="sxs-lookup"><span data-stu-id="da72a-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="da72a-104">如果您直接向 Azure AD 註冊裝置，並將其註冊到 Intune，您必須確定您已 [設定 intune](/mem/intune/enrollment/device-enrollment) 並且先進行 [授權](/mem/intune/fundamentals/licenses-assign) 。</span><span class="sxs-lookup"><span data-stu-id="da72a-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="da72a-105">確定您有權在 Azure AD 中執行作業。</span><span class="sxs-lookup"><span data-stu-id="da72a-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="da72a-106">只有 Azure AD 中的全域系統管理員可以管理裝置註冊的設定。</span><span class="sxs-lookup"><span data-stu-id="da72a-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="da72a-107">若要執行 Azure AD 加入實施，請參閱 [Plan AZURE Ad join](/azure/active-directory/devices/azureadjoin-plan)。</span><span class="sxs-lookup"><span data-stu-id="da72a-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="da72a-108">如需解決 Azure AD join 常見問題的詳細資訊，請參閱 [Azure Ad 聯結常見問題](/azure/active-directory/devices/faq) 和 Windows 10 專業版裝置，請參閱 [無法將 Windows 10 專業版電腦加入 Azure ad-必須升級至 Microsoft 社區](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)。</span><span class="sxs-lookup"><span data-stu-id="da72a-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
