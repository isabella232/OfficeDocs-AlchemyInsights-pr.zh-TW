---
title: 將 SharePoint 程式庫對應至網路磁片磁碟機
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 4b8245c3-a179-4524-ae83-0c22d539c202
ms.openlocfilehash: 6b7cb38362baa26bd39fe7478ef6dd1971b5b063
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 05/19/2021
ms.locfileid: "52542812"
---
# <a name="map-a-sharepoint-library-to-a-network-drive"></a>將 SharePoint 程式庫對應至網路磁片磁碟機

不要對應網路磁片磁碟機，使用新的 OneDrive 同步處理用戶端來同步處理 SharePoint 檔案，該用戶端會根據需要提供檔案。 不必使用本機儲存空間，即可在 OneDrive 中存取所有檔案。 如需詳細資訊，請參閱[Sync SharePoint and Teams files with a computer](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88) and [Save disk space with OneDrive files On Windows 10](https://support.microsoft.com/office/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e)。

如果您選擇要對應磁片磁碟機，而不是使用[新的 OneDrive 同步處理用戶端](https://support.microsoft.com/office/sync-sharepoint-and-teams-files-with-your-computer-6de9ede8-5b6e-4503-80b2-6190f3354a88)，請務必遵循下列步驟：

- [疑難排解連線至 SharePoint Online 的對應網路磁碟機](/sharepoint/support/administration/troubleshoot-mapped-network-drives)

- [用戶端不具備 TLS 1.2 支援時，會發生驗證錯誤](/sharepoint/troubleshoot/administration/authentication-errors-tls12-support#network-drive-mapped-to-a-sharepoint-library)  

**附注：** 如果您使用 Internet Explorer 10 搭配 Windows 8 或 Windows 7，而且在對應磁片磁碟機時 **無法存取**「接收 **存取權**」或「路徑」，請安裝此 [修復程式](https://support.microsoft.com/topic/error-when-you-open-a-sharepoint-document-library-in-windows-explorer-or-map-a-network-drive-to-the-library-after-you-install-internet-explorer-10-96e640ba-059f-9b09-bb91-2a0319ee8b1d)以解決此問題。