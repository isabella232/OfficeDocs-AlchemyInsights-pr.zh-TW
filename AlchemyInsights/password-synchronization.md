---
title: 密碼同步處理
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/24/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004595"
- "8619"
ms.openlocfilehash: 601649f6e5212ca03df5fcc32cd1d02c133e9170
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/04/2021
ms.locfileid: "50449084"
---
# <a name="password-synchronization"></a><span data-ttu-id="abde7-102">密碼同步處理</span><span class="sxs-lookup"><span data-stu-id="abde7-102">Password synchronization</span></span>

<span data-ttu-id="abde7-103">**密碼雜湊同步處理完全無法運作**</span><span class="sxs-lookup"><span data-stu-id="abde7-103">**Password Hash Synchronization does not work at all**</span></span>

<span data-ttu-id="abde7-104">當密碼雜湊同步處理無法運作時，客戶遇到的一些常見問題包括：</span><span class="sxs-lookup"><span data-stu-id="abde7-104">Some common issues customers encounter when Password Hash Synchronization does not work are:</span></span>

- <span data-ttu-id="abde7-105">Azure AD Connect 所使用的 Active Directory 帳戶不會被授與內部部署 Active Directory 的「 **複製目錄變更** 」和「複寫 **目錄變更」所有** 許可權（密碼同步處理所需）。您必須將這些許可權授與 Active Directory 帳戶，以修正此問題。</span><span class="sxs-lookup"><span data-stu-id="abde7-105">The Active Directory account used by Azure AD Connect to communicate with on-premises Active Directory is not granted **Replicate Directory Changes** and **Replicate Directory Changes All** permissions, which are required for password synchronization - You need to fix this by granting these permissions to the Active Directory account.</span></span>
- <span data-ttu-id="abde7-106">在管理員將使用者 Sign-In 方法從 [ **密碼同步** 處理] 變更為另一個選項（例如，Azure ad connect 嚮導中的 [ **同盟與 AD FS** ]）之後，就會停用密碼雜湊同步處理。您可以在 azure ad connect 嚮導中重新啟用 **密碼雜湊同步** 處理功能，以修正此問題。</span><span class="sxs-lookup"><span data-stu-id="abde7-106">Password hash synchronization is disabled after an administrator changed the User Sign-In method from **Password Synchronization** to another option such as **Federation with AD FS** in the Azure AD Connect wizard - You can fix this by re-enabling the **password hash synchronization** feature in the Azure AD Connect wizard.</span></span>
- <span data-ttu-id="abde7-107">內部部署 Active Directory 的連線問題。</span><span class="sxs-lookup"><span data-stu-id="abde7-107">Connectivity issue with on-premises Active Directory.</span></span> <span data-ttu-id="abde7-108">例如，有些網域控制站無法透過 Azure AD Connect 存取，或防火牆已封鎖 [所需的埠](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) -您必須確保 Azure AD Connect 伺服器與內部部署 Active Directory 之間的連線能夠正常運作，以修正此問題。</span><span class="sxs-lookup"><span data-stu-id="abde7-108">For example, some domain controllers are not accessible by Azure AD Connect, or the [ports required](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-ports) are blocked by Firewall - You need to fix this by ensuring that the connectivity between the Azure AD Connect server and the on-premises Active Directory works correctly.</span></span>
- <span data-ttu-id="abde7-109">Azure AD Connect 伺服器目前處於過渡模式，這會導致伺服器無法進行密碼雜湊-若要疑難排解問題，請遵循 section [使用 AZURE AD Connect sync 的密碼同步處理疑難排解](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)一節所述的步驟進行。不會同步處理密碼。</span><span class="sxs-lookup"><span data-stu-id="abde7-109">Azure AD Connect server currently being in staging mode, which will result the server not being able to the password hashes - To troubleshoot the issue, follow the steps described in section [Troubleshoot password synchronization with Azure AD Connect sync - No passwords are synchronized](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>

<span data-ttu-id="abde7-110">**密碼雜湊同步處理不適用於某些使用者**</span><span class="sxs-lookup"><span data-stu-id="abde7-110">**Password Hash Synchronization does not work for some of my users**</span></span>

1. <span data-ttu-id="abde7-111">如果您注意到密碼雜湊未同步處理使用者，請使用 Azure AD Connect 中的 **疑難排解** 工作進行調查並解決問題。</span><span class="sxs-lookup"><span data-stu-id="abde7-111">If you noticed that password hash is not syncing for a user, use the **troubleshoot** task in the Azure AD Connect to investigate and resolve the issue.</span></span> <span data-ttu-id="abde7-112">請執行下列工作：</span><span class="sxs-lookup"><span data-stu-id="abde7-112">Perform the following tasks:</span></span>

    <span data-ttu-id="abde7-113">a.</span><span class="sxs-lookup"><span data-stu-id="abde7-113">a.</span></span> [<span data-ttu-id="abde7-114">在嚮導中執行疑難排解工作</span><span class="sxs-lookup"><span data-stu-id="abde7-114">Run the troubleshooting task in the wizard</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-objectsync)

    <span data-ttu-id="abde7-115">b.</span><span class="sxs-lookup"><span data-stu-id="abde7-115">b.</span></span> [<span data-ttu-id="abde7-116">使用疑難排解 Cmdlet 調查特定用途的密碼雜湊同步處理問題</span><span class="sxs-lookup"><span data-stu-id="abde7-116">Use the troubleshooting cmdlet to investigate the password hash syncing issue for a specific use</span></span>](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)

2. <span data-ttu-id="abde7-117">已啟用 **[使用者必須在下次登入時變更密碼]** 選項的內部部署 Active Directory 使用者物件。</span><span class="sxs-lookup"><span data-stu-id="abde7-117">The on-premises Active Directory User object is enabled for **User must change password at next logon** option.</span></span> <span data-ttu-id="abde7-118">當此選項啟用時，使用者會被指派臨時密碼，並會在下次登入時提示您變更密碼。</span><span class="sxs-lookup"><span data-stu-id="abde7-118">When this option is enabled, the user is assigned a temporary password and will be prompted to change the password on the next logon.</span></span> <span data-ttu-id="abde7-119">Azure AD Connect 不會將臨時密碼同步處理到 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="abde7-119">Azure AD Connect does not synchronize temporary passwords to Azure AD.</span></span>

<span data-ttu-id="abde7-120">若要解決上述問題，請執行下列其中一項工作：</span><span class="sxs-lookup"><span data-stu-id="abde7-120">To resolve the above issue, perform either of the following tasks:</span></span>

- <span data-ttu-id="abde7-121">請使用者登入內部部署應用程式 (例如，Windows 桌面) 並變更密碼。</span><span class="sxs-lookup"><span data-stu-id="abde7-121">Ask the user to sign in to on-premises application (for example, Windows Desktop) and change the password.</span></span> <span data-ttu-id="abde7-122">新密碼會同步處理至 Azure AD。</span><span class="sxs-lookup"><span data-stu-id="abde7-122">The new password will be synchronized to Azure AD.</span></span>
- <span data-ttu-id="abde7-123">讓管理員更新使用者的密碼，而不啟用 [ **使用者必須在下次登入時變更密碼]**，並與使用者共用新密碼。</span><span class="sxs-lookup"><span data-stu-id="abde7-123">Have an administrator update the user's password without enabling the option **User must change password at next logon**, and share the new password with the user.</span></span>

3. <span data-ttu-id="abde7-124">**未正確設定** 內部部署 Active Directory 使用者物件，以進行物件同步處理或密碼同步處理。</span><span class="sxs-lookup"><span data-stu-id="abde7-124">The on-premises Active Directory User object is **not correctly configured** for object synchronization or password synchronization.</span></span> <span data-ttu-id="abde7-125">若要解決此問題，請遵循 [使用 AZURE AD Connect Sync 疑難排解密碼雜湊同步處理](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization)中所述的步驟。</span><span class="sxs-lookup"><span data-stu-id="abde7-125">To troubleshoot this issue, follow the steps described in the [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>







