---
title: 疑難排解 OneDrive 效能
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 22d5e2b24ac9bdd70b0bb0a9a6e1a0af29ef2c0f
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/22/2019
ms.locfileid: "36533906"
---
# <a name="troubleshoot-onedrive-performance"></a>疑難排解 OneDrive 效能

如果您遇到速度較慢比預期的同步處理或與 OneDrive 類似的效能問題：

- 請確認沒有任何使用[服務健全狀況儀表板](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fportal.office.com%2Fadminportal%2Fhome%23%2Fservicehealth&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051385661&sdata=z3OU7adaVjJorTGK8v7Ipo35E5vkk35lVCEzgGYQoNo%3D&reserved=0)的已知的問題。

- [啟用隨選檔案](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2Fsave-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051395670&sdata=QN1F4v1q6pNV2hIZ5LCZTtIbuv%2FR7lH5C5g%2FAFJQhrM%3D&reserved=0)，讓您可以存取您在 OneDrive 中的所有檔案，而不需下載全部，然後使用您的裝置上的儲存空間。

- 網路規劃和效能[檢閱的最佳作法](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fdocs.microsoft.com%2Foffice365%2Fenterprise%2Fnetwork-planning-and-performance&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051405678&sdata=RQCPPj7XPAm4IK6jKf1xugHnxXqqJoKK%2BlEENg7WrDQ%3D&reserved=0)。

- [上傳與下載速度最大化](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FMaximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051405678&sdata=vR4z9GSeObeKY3ouE7oru4Vr%2FGn%2FghUoFBjpRQbfvhA%3D&reserved=0)，尤其是如果您第一次同步處理的裝置。

- 如果您正在同步處理超過 100000 個項目與文件庫，OneDrive 同步處理似乎停滯很長的時間，或 [狀態] 顯示處理的 xMB 0 KB。 」 [了解更多關於同步處理超過 100000 檔案](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FInvalid-file-names-and-file-types-in-OneDrive-OneDrive-for-Business-and-SharePoint-64883a5d-228e-48f5-b3d2-eb39e07630fa%23synctoomany&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051415686&sdata=E4zeoBeRBnlGB1haZXTy%2FJfXMBWSPZCbp6JQvt5qX2o%3D&reserved=0)，以及[300000 檔案的 OneDrive 的支援的限制](https://nam06.safelinks.protection.outlook.com/?url=https%3A%2F%2Fsupport.office.com%2Farticle%2FInvalid-file-names-and-file-types-in-OneDrive-OneDrive-for-Business-and-SharePoint-64883a5d-228e-48f5-b3d2-eb39e07630fa%23numberitemscanbesynced&data=02%7C01%7CHunter.Donald%40microsoft.com%7Cc12aea2d6a5043ee79d908d6c75354db%7C72f988bf86f141af91ab2d7cd011db47%7C1%7C0%7C636915558051425695&sdata=uqBKB3ykz9QDOPRmSf5YIKBUiNa57IdQVzeLZWL%2BMWc%3D&reserved=0)。

- 當使用者超過使用量限制時，SharePoint Online 節流處理任何進一步的要求，從該使用者帳戶在短期間內。 節流生效時，會受到節流的所有使用者動作。
