---
title: 安全性群組問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162925"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="1f4e9-102">安全性群組問題</span><span class="sxs-lookup"><span data-stu-id="1f4e9-102">Issue with security groups</span></span>

<span data-ttu-id="1f4e9-103">**如果您收到網路錯誤 AADDS104**</span><span class="sxs-lookup"><span data-stu-id="1f4e9-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="1f4e9-104">不正確的網路安全性群組規則是 Azure Active Directory Domain Services (AD DS) 網路錯誤最常見的原因。</span><span class="sxs-lookup"><span data-stu-id="1f4e9-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="1f4e9-105">虛擬網路的網路安全性群組必須允許存取特定連接埠和通訊協定。</span><span class="sxs-lookup"><span data-stu-id="1f4e9-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="1f4e9-106">如果這些連接埠遭到封鎖，Azure 平台就無法監控或更新受管理的網域。</span><span class="sxs-lookup"><span data-stu-id="1f4e9-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="1f4e9-107">Azure AD 和 Azure AD DS 之間的同步處理也會受到影響。</span><span class="sxs-lookup"><span data-stu-id="1f4e9-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="1f4e9-108">請務必將預設連接埠保持開啟，以避免服務中斷。</span><span class="sxs-lookup"><span data-stu-id="1f4e9-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="1f4e9-109">若要瞭解並解決網路安全性群組設定問題的常見警示，請參閱[新增及驗證安全性群組](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules)。</span><span class="sxs-lookup"><span data-stu-id="1f4e9-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
