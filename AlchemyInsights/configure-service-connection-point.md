---
title: 設定服務連線點 (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/19/2021
ms.locfileid: "50897734"
---
# <a name="configure-service-connection-point-scp"></a><span data-ttu-id="9896c-102">設定服務連線點 (SCP)</span><span class="sxs-lookup"><span data-stu-id="9896c-102">Configure Service connection Point (SCP)</span></span>

<span data-ttu-id="9896c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span><span class="sxs-lookup"><span data-stu-id="9896c-103">**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**</span></span>

- <span data-ttu-id="9896c-104">**原因**：無法讀取 SCP 物件並取得 Azure AD 租用戶資訊</span><span class="sxs-lookup"><span data-stu-id="9896c-104">**Reason**: Unable to read the SCP object and get the Azure AD tenant information</span></span>
- <span data-ttu-id="9896c-105">**解決方案**：請參閱[設定服務連線點](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join) (部分機器翻譯) 章節</span><span class="sxs-lookup"><span data-stu-id="9896c-105">**Resolution**: Refer to the section [Configure a Service Connection Point](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)</span></span>


<span data-ttu-id="9896c-106">**行動計劃**</span><span class="sxs-lookup"><span data-stu-id="9896c-106">**Action plan**</span></span>

- <span data-ttu-id="9896c-107">檢查裝置是否已收到 GPO 進行控制的驗證。</span><span class="sxs-lookup"><span data-stu-id="9896c-107">Check whether the device has received the GPO for the controlled validation.</span></span>
- <span data-ttu-id="9896c-108">確保 GPO 已建立登錄機碼。</span><span class="sxs-lookup"><span data-stu-id="9896c-108">Ensure that the GPO has created the registry keys.</span></span>
- <span data-ttu-id="9896c-109">請確保已使用目錄識別碼和 onmicrosoft 網域建立 2 個機碼。</span><span class="sxs-lookup"><span data-stu-id="9896c-109">Ensure that you have 2 keys created with your Directory ID and onmicrosoft domain.</span></span>

<span data-ttu-id="9896c-110">**設定 SCP 的用戶端登錄設定**</span><span class="sxs-lookup"><span data-stu-id="9896c-110">**Configure client-side registry setting for SCP**</span></span>

<span data-ttu-id="9896c-111">使用下列範例來建立群組原則物件 (GPO)，以部署在裝置登錄中設定 SCP 項目之登錄設定。</span><span class="sxs-lookup"><span data-stu-id="9896c-111">Use the following example to create a Group Policy Object (GPO) to deploy a registry setting that configures an SCP entry in the registry of your devices.</span></span>

1. <span data-ttu-id="9896c-112">開啟群組原則管理主控台，然後在網域中建立的新 GPO。</span><span class="sxs-lookup"><span data-stu-id="9896c-112">Open a Group Policy Management console and create a new GPO in your domain.</span></span>
     - <span data-ttu-id="9896c-113">提供您新建立 GPO 的名稱 (例如 ClientSideSCP)</span><span class="sxs-lookup"><span data-stu-id="9896c-113">Provide your newly created GPO a name (for example, ClientSideSCP)</span></span>

2. <span data-ttu-id="9896c-114">編輯 GPO 並找到下列路徑：**[電腦設定] > [喜好設定] > [Windows 設定] > [登錄]**。</span><span class="sxs-lookup"><span data-stu-id="9896c-114">Edit the GPO and locate the following path: **Computer Configuration > Preferences > Windows Settings > Registry**.</span></span>

3. <span data-ttu-id="9896c-115">以滑鼠右鍵按一下 **[登錄]**，然後選取 **[新增] > [登錄項目]**。</span><span class="sxs-lookup"><span data-stu-id="9896c-115">Right-click on **Registry** and select **New > Registry Item**.</span></span>

4. <span data-ttu-id="9896c-116">在 **[一般]** 索引標籤上，設定下列設定：</span><span class="sxs-lookup"><span data-stu-id="9896c-116">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="9896c-117">**動作**：更新</span><span class="sxs-lookup"><span data-stu-id="9896c-117">**Action**: Update</span></span>
    
- <span data-ttu-id="9896c-118">**登錄區**：HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="9896c-118">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="9896c-119">**機碼路徑**：SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="9896c-119">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="9896c-120">**值名稱**：TenantId</span><span class="sxs-lookup"><span data-stu-id="9896c-120">**Value name**: TenantId</span></span>
    
- <span data-ttu-id="9896c-121">**值類型**：REG_SZ</span><span class="sxs-lookup"><span data-stu-id="9896c-121">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="9896c-122">**值資料**：Azure AD 實例的 GUID 或目錄識別碼 (此值位於 **[Azure 入口網站] > [Azure Active Directory] > [屬性] > [目錄識別碼]**)</span><span class="sxs-lookup"><span data-stu-id="9896c-122">**Value data**: The GUID or Directory ID of your Azure AD instance (This value can be found in **Azure portal > Azure Active Directory > Properties > Directory ID**)</span></span>
 
- <span data-ttu-id="9896c-123">按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="9896c-123">Click **OK**.</span></span>
 
5. <span data-ttu-id="9896c-124">以滑鼠右鍵按一下 **[登錄]**，然後選取 **[新增] > [登錄項目]**。</span><span class="sxs-lookup"><span data-stu-id="9896c-124">Right-click on **Registry** and select **New > Registry Item**.</span></span>

6. <span data-ttu-id="9896c-125">在 **[一般]** 索引標籤上，設定下列設定：</span><span class="sxs-lookup"><span data-stu-id="9896c-125">On the **General** tab, configure the following:</span></span>
  
- <span data-ttu-id="9896c-126">**動作**：更新</span><span class="sxs-lookup"><span data-stu-id="9896c-126">**Action**: Update</span></span>
    
- <span data-ttu-id="9896c-127">**登錄區**：HKEY_LOCAL_MACHINE</span><span class="sxs-lookup"><span data-stu-id="9896c-127">**Hive**: HKEY_LOCAL_MACHINE</span></span>
    
- <span data-ttu-id="9896c-128">**機碼路徑**：SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span><span class="sxs-lookup"><span data-stu-id="9896c-128">**Key Path**: SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD</span></span>
    
- <span data-ttu-id="9896c-129">**值名稱**：TenantName</span><span class="sxs-lookup"><span data-stu-id="9896c-129">**Value name**: TenantName</span></span>
    
- <span data-ttu-id="9896c-130">**值類型**：REG_SZ</span><span class="sxs-lookup"><span data-stu-id="9896c-130">**Value type**: REG_SZ</span></span>
    
- <span data-ttu-id="9896c-131">**值資料**：如果您使用同盟環境 (例如 AD FS)，則為已驗證的網域名稱。</span><span class="sxs-lookup"><span data-stu-id="9896c-131">**Value data**: Your verified domain name if you are using federated environment such as AD FS.</span></span> <span data-ttu-id="9896c-132">如果您使用受管理環境，則為您已驗證的網域名稱或您的 onmicrosoft.com 網域名稱 (例如 contoso.onmicrosoft).com</span><span class="sxs-lookup"><span data-stu-id="9896c-132">Your verified domain name or your onmicrosoft.com domain name (for example, contoso.onmicrosoft).com if you are using managed environment</span></span>

- <span data-ttu-id="9896c-133">按一下 **[確定]**。</span><span class="sxs-lookup"><span data-stu-id="9896c-133">Click **OK**.</span></span>

7. <span data-ttu-id="9896c-134">關閉新建立 GPO 的編輯器。</span><span class="sxs-lookup"><span data-stu-id="9896c-134">Close the editor for the newly created GPO.</span></span>

8. <span data-ttu-id="9896c-135">將新建立 GPO 連結到所需的 OU，其中包含屬於您控制推出母體之已加入網域的電腦。</span><span class="sxs-lookup"><span data-stu-id="9896c-135">Link the newly created GPO to the desired OU containing domain-joined computers that belong to your controlled rollout population.</span></span>

<span data-ttu-id="9896c-136">如需詳細資訊，請參閱[混合式 Azure AD Join 的受控驗證 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) (部分機器翻譯) 和[針對已進行混合式 Azure Active Directory Join 的裝置進行疑難排解 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) (部分機器翻譯)。</span><span class="sxs-lookup"><span data-stu-id="9896c-136">For more information, see [Controlled validation of hybrid Azure AD join - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) and  [Troubleshooting hybrid Azure Active Directory joined devices | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).</span></span>









