---
title: 啟動 OneDrive 時發生0x8004de40 錯誤
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
- "6886"
- "9003837"
ms.openlocfilehash: 23c57356c8bd94c1cbafb538c9318208429754115a7c4e88abc93d293b5ea6e1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946570"
---
# <a name="0x8004de40-error-when-launching-onedrive"></a>啟動 OneDrive 時發生0x8004de40 錯誤

如果您在登入 OneDrive 時收到錯誤 **0x8004de40** ，請在連線至您的公司或學校網域時，重新開機電腦。 如果重新開機後收到此錯誤，請在連線至您的工作或學校網域時，嘗試此動作：

1. 按一下 [開始]，  **然後在搜尋方塊中，** 于命令提示字元應用程式上按一下滑鼠右鍵，然後選取 [**以系統管理員身分執行**]。 如果系統提示您輸入系統管理員密碼或進行確認，請輸入密碼或按一下 [ **允許**]。  

2. 在 [命令提示字元] 視窗中，輸入 **dsregcmd/leave**  ，並等待命令完成。 然後輸入 **dsregcmd/join** ，並等待命令完成。
3. 重新開機電腦。
