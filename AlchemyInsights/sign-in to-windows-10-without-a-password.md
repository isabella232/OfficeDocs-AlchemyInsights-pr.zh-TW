---
title: 不使用密碼即登入 Windows 10
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
- "9001690"
- "3766"
ms.openlocfilehash: fbf190d433eabfee5b45348d05d918222a385314a431812aa5f5926aacf11560
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54107498"
---
# <a name="sign-in-to-windows-10-without-using-a-password"></a>不使用密碼即登入 Windows 10

若要避免在 Windows 啟動時輸入密碼，建議您使用其中一個 Windows Hello 安全登入選項，例如 PIN、面孔識別或指紋（如果有的話）。 如果您真的想要停用安全登入，請參閱下列的「自動登入 Windows 10」指示。

**安全 Windows Hello 替代帳戶密碼**

移至 **設定 > 帳戶 > 登入選項** (或按一下 [這裡](ms-settings:signinoptions?activationSource=GetHelp)) 。 將會列出可用的登入選項。 例如：

![登入選項。](media/sign-in-options.png)

按一下或點擊其中一個選項加以設定。 當您下一次啟動或解除鎖定 Windows 時，您將可以使用新的選項，而不是密碼。 

**自動登入至 Windows 10**

**附注**：自動登入非常方便，但會帶來安全性風險，尤其是當您的電腦可由多人存取時。 

1. 按一下或點擊工作列中的 [ **開始** ] 按鈕。

2. 輸入 **netplwiz** ，然後按 Enter 鍵，以開啟 [使用者帳戶] 視窗。

3. 在 [**使用者帳戶**] 中，按一下 [Windows 開始時要自動登入的帳戶。

4. 取消選取 [使用者必須輸入使用者名稱和密碼才能使用此電腦] 核取方塊。

    ![使用者必須輸入 [使用者名稱] 和 [密碼] 選項。](media/users-must-enter-username.png)

5. 按一下 ****[確定]。 系統會要求您輸入並確認您所選取之帳戶的密碼。 按一下 [確定] 完成。 下次 Windows 10 啟動時，會自動登入您選取的帳戶。
