---
title: 密碼寫回無法運作
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
- "9004595"
- "8210"
ms.openlocfilehash: d7766f908f025b5db8299aa45d01dc5389b321ec
ms.sourcegitcommit: 2f39850ac0fba9fbeba9b8b7939ae79b505d3b67
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2021
ms.locfileid: "50232679"
---
# <a name="password-writeback-is-not-working"></a>密碼寫回無法運作

**設定密碼寫回時有問題**

- 密碼寫回是一項高級功能。
- 請務必瞭解授權需求：
  - 您的組織中必須至少有一個指派的授權
  - **僅限雲端使用者** -任何 Office 365 (O365) 付費 SKU 或 Azure AD Basic
  - **雲端和/或內部部署使用者** -Azure AD Premium P1 或 P2、Enterprise 可移動性 + SECURITY (EMS) 或安全生產力 (SPE) 
    - 若要深入瞭解授權需求，請參閱 [AZURE AD 自助密碼重設的授權需求](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-licensing)
- 您有至少一個系統管理員帳戶和一個具有適當授權的測試使用者帳戶。
- 您必須將 Azure AD Connect 連線至網域主控站模擬器，以供密碼寫回工作使用。 您可以設定 Azure AD Connect，以使用主要的網域控制站，方法是在 Active Directory 同步處理連接器的 **屬性** 上按一下滑鼠右鍵，然後選取 [ **設定目錄磁碟分割**]。 從那裡，尋找 [ **網域控制站連線設定** ] 區段，然後選取 [ **只使用偏好的網域控制站**] 方塊。
  > [!NOTE]
  > 如果首選 DC 不是 PDC 模擬器，Azure AD Connect 仍會到達 PDC 以進行密碼回寫。
- 已在您的租使用者中設定並啟用密碼重設。 如需詳細資訊，請參閱 [讓使用者重設其 AZURE AD 密碼](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-getting-started)。
- 確定要用來啟用密碼寫回的系統管理員帳戶， (Azure AD 中建立的雲端系統管理員帳戶不在內部部署 AD) 
- 您有一個或多個樹系 AD 內部部署執行 Windows Server 2008 R2、Windows Server 2012 或 Windows Server 2012 R2 （安裝了最新的 service pack）
- 您已安裝 Azure AD Connect 工具，且已準備好要同步處理至雲端的 AD 環境。 在測試密碼寫回之前，請先確定您已完成從 Azure AD Connect 中的 AD 和 Azure AD 的完整匯入和完整同步處理。
- 若要深入瞭解，請參閱如何 [在 AZURE AD Connect 中執行完整同步和完整匯入](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-operations)

**我在密碼寫回連線時出現問題**

1. 下載並啟用[AZURE AD Connect](https://www.microsoft.com/download/details.aspx?id=47594)的最新版本
2. 防火牆設定： Azure AD Connect 工具 (1.1.443 及更新版本) 需要 **輸出 HTTPS** 存取權：
    - passwordreset.microsoftonline.com
    - windows 網路
3. 允許閒置連線至少保留2-3 分鐘

**密碼回寫時仍然存在問題**

- 如果您仍然有困難，請嘗試停用並重新啟用 Azure AD Connect 工具中的密碼回寫服務。
- 若要深入瞭解，請參閱如何 [停用及重新啟用密碼回寫功能](https://docs.microsoft.com/azure/active-directory/active-directory-passwords-troubleshoot)
