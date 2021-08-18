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
ms.openlocfilehash: d89fb92ce1775e5a77808a1893a315419b4d54706dc737327c51f7c4c4e488e2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088063"
---
# <a name="issue-joining-vms"></a>加入 VM 的問題

若要嘗試在加入 VM 時發生的問題，請執行下列步驟：

1. 嘗試改以 **UPN** 格式 (例如 'joeuser@contoso.com')，取代 **SAMAccountName** 格式 ('CONTOSO\joeuser') 登入。
2. 請確認您已依照 *快速入門* 指南中所述的步驟啟用密碼同步處理。
3. 請確認受影響的使用者帳戶不是 Azure AD 租用戶中的外部帳戶。 外部使用者無法登入受管理的網域，因為 Azure AD Domain Services 沒有這些使用者帳戶的認證。
4. 如果受影響的使用者帳戶是僅限雲端使用者帳戶，請確認在您啟用 Azure AD Domain Services 後使用者已變更其密碼。 此步驟會導致 Azure AD Domain Services 必要的認證雜湊產生。
5. 如果受影響的使用者帳戶是從內部部署目錄同步處理，請驗證已將 Azure AD Connect 的建議版本設定為執行完整同步處理。
6. 如果問題在確認步驟 4 之後仍然存在，請從您的同步處理電腦執行下列命令：
 
     `"net stop 'Microsoft Azure AD Sync'"`  
     `"net start 'Microsoft Azure AD Sync'"`.