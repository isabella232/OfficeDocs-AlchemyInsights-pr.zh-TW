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
ms.openlocfilehash: b9bd6dff48f78063e3d47f5fe2f834f59eb9868a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47745121"
---
# <a name="fix-0x8004de40-error-in-onedrive"></a>修正 OneDrive 中的0x8004de40 錯誤

如果您收到 OneDrive 的0x8004de40 錯誤：

- 在連線至您的 Acitve 目錄網域時，重新開機受影響的電腦。
- 如果重新開機未修正問題，請從 Azure AD 中脫離裝置並重新加入裝置。 

**附注**：您應該在公司網路上執行這些步驟。 當您無法連線到公司基礎結構 (例如旅行) 時，請勿執行這些步驟。 

- 開啟提高權限的命令提示字元。 
- 若要開啟提升許可權的命令提示字元，請按一下 [ **開始**]，用滑鼠右鍵按一下 [ **命令提示**字元]，然後按一下 [以 **管理員身分執行**]。
- 輸入 *dsregcmd/leave* ，然後按 **enter**鍵。
- 完成時，請輸入 *dsregcmd/join* ，然後按 **enter**。
- 完成後，請關閉命令提示字元。
- 重新開機電腦，並登入 OneDrive。