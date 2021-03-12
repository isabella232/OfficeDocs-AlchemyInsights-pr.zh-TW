---
title: 複本集
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/10/2021
ms.locfileid: "50716267"
---
# <a name="replica-set"></a><span data-ttu-id="510d7-102">複本集</span><span class="sxs-lookup"><span data-stu-id="510d7-102">Replica set</span></span>

<span data-ttu-id="510d7-103">AADDS 也稱為受管理的網域。</span><span class="sxs-lookup"><span data-stu-id="510d7-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="510d7-104">這實際上是兩個由後端執行及維護的網域控制站。</span><span class="sxs-lookup"><span data-stu-id="510d7-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="510d7-105">這兩個 Dc 包含一個主要 DC 和一個複寫 DC。</span><span class="sxs-lookup"><span data-stu-id="510d7-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="510d7-106">AADDS (managed domain) 中的備份是由 Azure 平臺所管理的自動程式。</span><span class="sxs-lookup"><span data-stu-id="510d7-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="510d7-107">在受管理的網域發生問題時，Azure 支援可協助您從備份還原。</span><span class="sxs-lookup"><span data-stu-id="510d7-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="510d7-108">您可以在虛擬網路中建立每個複本集。</span><span class="sxs-lookup"><span data-stu-id="510d7-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="510d7-109">每個虛擬網路都必須 peered 到主控受管理網域之複本集的其他每個虛擬網路。</span><span class="sxs-lookup"><span data-stu-id="510d7-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="510d7-110">這種設定會建立支援目錄複寫的網狀網路拓朴。</span><span class="sxs-lookup"><span data-stu-id="510d7-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="510d7-111">虛擬網路可支援多個複本集，只要每個複本集位於不同的虛擬子網中。</span><span class="sxs-lookup"><span data-stu-id="510d7-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="510d7-112">如需複本集的詳細資訊，請參閱 [概念複本集](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets)。</span><span class="sxs-lookup"><span data-stu-id="510d7-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
