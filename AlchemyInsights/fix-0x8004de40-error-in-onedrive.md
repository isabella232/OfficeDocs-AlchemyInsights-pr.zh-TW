---
title: 修正 OneDrive 中的 0x8004de40 錯誤
ms.author: kirks
author: Techwriter40
ms.date: 6/20/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: d436184bdc0e283db217ea734fb2c8e05f85b4e7
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36525050"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>修正 OneDrive 中的 0x8004de40 錯誤

如果您收到 OneDrive 0x8004de40 錯誤：

- 重新啟動受影響的電腦連線到您啟用目錄的網域時。
- 如果重新開啟才不會修正這個問題，解除加入並重新加入您的裝置從 Azure AD。 

**附註**： 您應在公司網路上同時執行這些步驟。 當您不可以連線到您公司的基礎結構 （例如，當旅行） 時，不執行這些步驟。 

- 開啟提升權限的命令提示字元。 
- 若要開啟提升權限的命令提示字元處，按一下 [-**開始**，以滑鼠右鍵按一下 [**命令提示字元處**，，然後按一下 [**以管理員身分執行**。
- 輸入*dsregcmd /leave* ，然後按**Enter**鍵。
- 完成後，輸入*dsregcmd /join* ，然後按**Enter**鍵。
- 完成時，關閉命令提示字元。
- 將電腦重新開機並登入 OneDrive。