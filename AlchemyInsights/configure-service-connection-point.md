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
ms.openlocfilehash: 5ccb55996ccef4b55c8d80de6e35f4ba27e3dfa18dfcaeaf6f6ad1c54b6bb376
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965956"
---
# <a name="configure-service-connection-point-scp"></a>設定服務連線點 (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **原因**：無法讀取 SCP 物件並取得 Azure AD 租用戶資訊
- **解決方案**：請參閱 [設定服務連線點](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join) (部分機器翻譯) 章節


**行動計劃**

- 檢查裝置是否已收到 GPO 進行控制的驗證。
- 確保 GPO 已建立登錄機碼。
- 請確保已使用目錄識別碼和 onmicrosoft 網域建立 2 個機碼。

**設定 SCP 的用戶端登錄設定**

使用下列範例來建立群組原則物件 (GPO)，以部署在裝置登錄中設定 SCP 項目之登錄設定。

1. 開啟群組原則管理主控台，然後在網域中建立的新 GPO。
     - 提供您新建立 GPO 的名稱 (例如 ClientSideSCP)

2. 編輯 GPO 並找到下列路徑：**[電腦設定] > [喜好設定] > [Windows 設定] > [登錄]**。

3. 以滑鼠右鍵按一下 **[登錄]**，然後選取 **[新增] > [登錄項目]**。

4. 在 **[一般]** 索引標籤上，設定下列設定：
  
- **動作**：更新
    
- **登錄區**：HKEY_LOCAL_MACHINE
    
- **機碼路徑**：SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **值名稱**：TenantId
    
- **值類型**：REG_SZ
    
- **值資料**：Azure AD 實例的 GUID 或目錄識別碼 (此值位於 **[Azure 入口網站] > [Azure Active Directory] > [屬性] > [目錄識別碼]**)
 
- 按一下 **[確定]**。
 
5. 以滑鼠右鍵按一下 **[登錄]**，然後選取 **[新增] > [登錄項目]**。

6. 在 **[一般]** 索引標籤上，設定下列設定：
  
- **動作**：更新
    
- **登錄區**：HKEY_LOCAL_MACHINE
    
- **機碼路徑**：SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **值名稱**：TenantName
    
- **值類型**：REG_SZ
    
- **值資料**：如果您使用同盟環境 (例如 AD FS)，則為已驗證的網域名稱。 如果您使用受管理環境，則為您已驗證的網域名稱或您的 onmicrosoft.com 網域名稱 (例如 contoso.onmicrosoft).com

- 按一下 **[確定]**。

7. 關閉新建立 GPO 的編輯器。

8. 將新建立 GPO 連結到所需的 OU，其中包含屬於您控制推出母體之已加入網域的電腦。

如需詳細資訊，請參閱[混合式 Azure AD Join 的受控驗證 - Azure AD | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) (部分機器翻譯) 和[針對已進行混合式 Azure Active Directory Join 的裝置進行疑難排解 | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) (部分機器翻譯)。









