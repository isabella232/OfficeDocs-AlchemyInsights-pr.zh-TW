---
title: 登入 Microsoft 365 應用程式時的問題
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
ms.openlocfilehash: e6cbab7401fd6168041e7fc31ac97e3be036536d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833022"
---
# <a name="blank-sign-in-screen-in-microsoft-365-apps"></a>Microsoft 365 應用程式中的空白登入畫面

若要修正此問題，請嘗試下列步驟：
- 安裝最新的 [Windows](https://support.microsoft.com/help/4027667/windows-10-update) 和 [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)更新。
- 重設 internet Explorer 選項：移至 **工具**  >  **網際網路選項**  >  **Advanced**  >  **Reset internet Explorer 設定** (請注意，您會失去) 的自訂設定，然後再次嘗試登入 Office。
- 停用 Windows Defender Application Guard (WDAG) 或任何類似的防火牆或防毒程式：
    1. 在 [控制台] 中，移至 [ **程式**]，然後選擇 [ **開啟或關閉 Windows 功能**]。
    2. 如果已啟用 Windows Defender Application Guard，請嘗試停用它。<br/>
    **附注：** 您可能需要重新開機電腦。
- 確定任何應用程式或防火牆/反病毒程式都未封鎖 BrokerPlugin [AAD WAM 外掛程式](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-1) 。
- 使用 Windows 認證管理員[清除 Office 認證](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer)。<br/>
    **附注：** Office 2016 的登錄路徑已變更為16.0。  (Ex： \Software\Microsoft\Office\16.0\Common\Identity\)

如需詳細資訊，請參閱在 [Windows 10 上更新到 Office 2016 build 16.0.7967 後，登入的連線問題](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)。