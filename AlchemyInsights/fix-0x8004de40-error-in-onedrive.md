---
title: 修正 OneDrive 中的0x8004de40 錯誤
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 0edb3e19b5dea240c9f2846dc503e65d92113cb7
ms.sourcegitcommit: 477cce131dc4a3c212ab18a8763a50b2f3bb20b1
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/09/2021
ms.locfileid: "51649739"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>修正 OneDrive 中的0x8004de40 錯誤

如果您是執行 Windows 7，但收到此錯誤，請 [更新以啟用 tls 1.1 和 tls 1.2 做為 Windows WinHTTP 中的預設安全通訊協定](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)。

如果您正在執行 Windows 10，而且 OneDrive 收到0x8004de40 錯誤：

- 在連線至您的 Acitve 目錄網域時，重新開機受影響的電腦。
- 如果重新開機未修正問題，請從 Azure AD 中脫離裝置並重新加入裝置。 

**附注**：您應該在公司網路上執行這些步驟。 當您未連線到公司基礎結構時，請勿執行這些步驟，例如，旅行) 時 (。 

1. 選取 [ **開始**]，用滑鼠右鍵按一下 [ **命令提示** 字元]，然後選取 [ **以系統管理員身分執行**]，開啟提升許可權的命令提示字元

1. 輸入 *dsregcmd/leave* ，然後按 **enter** 鍵。

1. 完成時，請輸入 *dsregcmd/join* ，然後按 **enter**。

1. 完成後，請關閉命令提示字元。

1. 重新開機電腦，並登入 OneDrive。