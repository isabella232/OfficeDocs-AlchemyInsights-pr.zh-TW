---
title: 移除 Office 的先前 MSI 版本
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 12/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003886"
- "6940"
ms.openlocfilehash: 45e3cac521bc1c2a90dc7d3ddd4958233c3cf7bbd2ea007e581f343bca7b5631
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "54023765"
---
# <a name="remove-prior-msi-versions-of-office"></a>移除 Office 的先前 MSI 版本

建議您先移除之前 Windows Installer (MSI) 版本的 Office，再安裝 Office 365 專業增強版。 以下說明如何執行此動作：

1. 如果您使用 MSI 安裝 Office，您可以使用 Office 部署工具 (ODT) 卸載 Office。 您可以在 **configuration.xml** 檔案中使用 RemoveMSI 元素。
1. 遵循本文中的指示： [Office 365 安全性 & 規範中心。](https://go.microsoft.com/fwlink/p/?linkid=2077143)