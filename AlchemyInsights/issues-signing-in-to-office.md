---
title: 在 Microsoft 365 應用程式中登入的問題
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2556"
ms.openlocfilehash: 7a8a0b68fc211e99b22e857d51d1de54e53a69357f75a0c60b1e83078cd5b27f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54088027"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Microsoft 365 應用程式中的空白登入畫面

若要修正此問題，請嘗試下列步驟：
- 為[Windows](https://support.microsoft.com/help/4027667/windows-10-update)和[Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)安裝最新的更新。
- 重設 internet Explorer 選項：移至 **工具**  >  **網際網路選項**  >  **Advanced**  >  **Reset internet Explorer 設定** (請注意，您會失去) 的自訂設定，然後嘗試再次登入 Office。
- 停用 Windows Defender 應用程式防護 (WDAG) 或任何類似的防火牆或防毒程式：
    1. 在 [控制台] 中，移至 [**程式**]，然後選擇 [**開啟] 或 [關閉 Windows 功能**]。
    2. 如果已啟用 Windows Defender 應用程式防護，請嘗試停用。<br/>
    **附注：** 您可能需要重新開機電腦。
- 確定任何應用程式或防火牆/反病毒程式都未封鎖 BrokerPlugin [AAD WAM 外掛程式](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) 。
- 使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br/>
    **附注：** Office 2016 的登錄路徑已變更為16.0。  (Ex： \Software\Microsoft\ Office \16.0\Common\Identity\)

如需詳細資訊，請參閱[update to Office 2016 build 16.0.7967 on on Windows 10 上的連線問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。