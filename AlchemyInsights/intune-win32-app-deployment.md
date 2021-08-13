---
title: Intune Win32 應用程式部署
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6446"
- "6700004"
ms.openlocfilehash: d169dc0dd4e3cd9d94681d7db16ce3051677b708df02d3c9bd461855daabb295
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925876"
---
# <a name="intune-win32-app-deployment"></a>Intune Win32 應用程式部署

Microsoft Intune 允許在 Windows 10 裝置上部署 Win32 應用程式，包括但不限於MSI和.EXE。 使用的部署機制要求目標設裝置有 Intune Management Extension (IME)。 由於將 powershell 腳本或 win32 應用程式部署定位到使用者/裝置，將自動安裝 IME。

若要部署 Win32 應用程式，還必須符合一組先決條件，其中包括：

- 支援的平台：Windows 10 版本1607 或更新版本 (企業版、專業版和教育版)。
- 支援的結構： x86 和 x64。
- 裝置管理： 已加入和自動註冊 AAD (包括加入混合式網域和自動註冊群組原則)。
- 應用程式套件格式：由 [Microsoft Win32 內容準備工具](https://docs.microsoft.com/mem/intune/apps/apps-win32-prepare)準備的 .**intunewin** 檔案。
- 限制：
    - 大小上限：8GB。
    - 不支援的結構： ARM。

如需有關這些步驟的詳細資訊，請參閱[「在 Microsoft Intune 中新增、指派及監視 Win32 應用程式」](https://docs.microsoft.com/mem/intune/apps/apps-win32-add)的文件。

有關 Windows 上應用程式部署 (包括 Win32 應用程式) 疑難排解的詳細資訊，請參閱以下文件

- [應用程式安裝問題的疑難排解](https://docs.microsoft.com/mem/intune/apps/troubleshoot-app-install)  
- [Win32 應用程式的疑難排解](https://docs.microsoft.com/mem/intune/apps/apps-win32-troubleshoot)