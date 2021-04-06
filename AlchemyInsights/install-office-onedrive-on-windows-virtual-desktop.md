---
title: 在 Windows 虛擬桌面上安裝 Office 和 OneDrive
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 04/05/2021
ms.locfileid: "51590274"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a>在 Windows 虛擬桌面上安裝 Office 和 OneDrive

1. [準備並自訂主 VHD 映像](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)。 如果尚未建立虛擬機器 (VM)，請建立它。

1. [在用電腦啟用模式中安裝 Office](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)。 共用電腦啟用可讓多個使用者存取 Office。

1. [在每一電腦模式下安裝 OneDrive](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)。 通常，OneDrive 是按使用者安裝的，但在這裡，它應該按機器安裝。