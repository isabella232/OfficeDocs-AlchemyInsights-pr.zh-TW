---
title: 修正 OneDrive 中的0x8004de40 錯誤
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 2256fb66cb7a4e2adcff9fda16a80c87e2997f0c
ms.sourcegitcommit: 8f6a1be929b275faa295ba8aeeae17898a47c3b0
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 06/21/2019
ms.locfileid: "35133968"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>修正 OneDrive 中的0x8004de40 錯誤

如果您收到 OneDrive 的0x8004de40 錯誤:

- 在連線至您的 Acitve Directory 網域時, 重新開機受影響的電腦。
- 如果重新開機無法修正問題, 請將裝置從 Azure AD 脫離並重新加入。 

**附注**: 執行這些步驟時, 您應該在公司網路上。 當您無法連線到公司基礎結構 (例如出差時) 時, 請勿執行這些步驟。 

- 開啟提升許可權的命令提示字元。 
- 若要開啟提升許可權的命令提示字元, 請按一下 [**開始**], 用滑鼠右鍵按一下 [**命令提示**字元], 然後按一下 [以**管理員身分執行**]。
- 輸入*dsregcmd/leave* , 然後按**enter**鍵。
- 完成時, 請輸入*dsregcmd/join* , 然後按**enter**。
- 完成後, 請關閉命令提示字元。
- 重新開機電腦, 然後登入 OneDrive。