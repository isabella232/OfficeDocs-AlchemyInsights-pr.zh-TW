---
title: 加入 VM 的問題
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7924"
- "9004395"
ms.openlocfilehash: 77a889f05d6c4e7b19a1e0a66a99ffc0565c69d8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 01/18/2021
ms.locfileid: "49884565"
---
# <a name="issue-joining-vms"></a><span data-ttu-id="23cc7-102">加入 VM 的問題</span><span class="sxs-lookup"><span data-stu-id="23cc7-102">Issue joining VMs</span></span>

<span data-ttu-id="23cc7-103">若要嘗試在加入 VM 時發生的問題，請執行下列步驟：</span><span class="sxs-lookup"><span data-stu-id="23cc7-103">To resolve issues that occur while trying to join VMs, perform the following steps:</span></span>

1. <span data-ttu-id="23cc7-104">嘗試改以 **UPN** 格式 (例如 'joeuser@contoso.com')，取代 **SAMAccountName** 格式 ('CONTOSO\joeuser') 登入。</span><span class="sxs-lookup"><span data-stu-id="23cc7-104">Try to sign in using the **UPN** format (for example, 'joeuser@contoso.com') instead of the **SAMAccountName** format ('CONTOSO\joeuser').</span></span>
2. <span data-ttu-id="23cc7-105">請確認您已依照 *快速入門* 指南中所述的步驟啟用密碼同步處理。</span><span class="sxs-lookup"><span data-stu-id="23cc7-105">Ensure that you have enabled password synchronization in accordance with the steps outlined in the *Getting Started* guide.</span></span>
3. <span data-ttu-id="23cc7-106">請確認受影響的使用者帳戶不是 Azure AD 租用戶中的外部帳戶。</span><span class="sxs-lookup"><span data-stu-id="23cc7-106">Ensure that the affected user account is not an external account in the Azure AD tenant.</span></span> <span data-ttu-id="23cc7-107">外部使用者無法登入受管理的網域，因為 Azure AD Domain Services 沒有這些使用者帳戶的認證。</span><span class="sxs-lookup"><span data-stu-id="23cc7-107">External users cannot sign in to the managed domain since Azure AD Domain Services does not have credentials for such user accounts.</span></span>
4. <span data-ttu-id="23cc7-108">如果受影響的使用者帳戶是僅限雲端使用者帳戶，請確認在您啟用 Azure AD Domain Services 後使用者已變更其密碼。</span><span class="sxs-lookup"><span data-stu-id="23cc7-108">If the affected user account is a cloud-only user account, ensure that users have changed their password after you enabled Azure AD Domain Services.</span></span> <span data-ttu-id="23cc7-109">此步驟會導致 Azure AD Domain Services 必要的認證雜湊產生。</span><span class="sxs-lookup"><span data-stu-id="23cc7-109">This step causes the credential hashes required for Azure AD Domain Services to be generated.</span></span>
5. <span data-ttu-id="23cc7-110">如果受影響的使用者帳戶是從內部部署目錄同步處理，請驗證已將 Azure AD Connect 的建議版本設定為執行完整同步處理。</span><span class="sxs-lookup"><span data-stu-id="23cc7-110">If the affected user accounts are synchronized from an on-premises directory, verify that the recommended release of Azure AD Connect has been configured to perform a full synchronization.</span></span>
6. <span data-ttu-id="23cc7-111">如果問題在確認步驟 4 之後仍然存在，請從您的同步處理電腦執行下列命令：</span><span class="sxs-lookup"><span data-stu-id="23cc7-111">If issues persists after confirming Step 4, execute the following commands from your sync machine:</span></span>
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     <span data-ttu-id="23cc7-112">`"net start 'Microsoft Azure AD Sync'"`.</span><span class="sxs-lookup"><span data-stu-id="23cc7-112">`"net start 'Microsoft Azure AD Sync'"`.</span></span>