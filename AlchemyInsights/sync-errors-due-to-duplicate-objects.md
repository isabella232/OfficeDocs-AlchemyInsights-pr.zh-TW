---
title: '902由於重複的物件而 (同步處理錯誤) '
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 902
ms.assetid: 9d9277a5-c825-4512-8d54-7138b2ee0c40
ms.openlocfilehash: 33b8ad0a33eb02eb9ec5bd26f94b00e5645b3fd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 09/14/2020
ms.locfileid: "47737332"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>由於重複的物件而產生同步處理錯誤

當 Microsoft 365 中的目錄同步處理完成時，您可能會收到下列其中一則錯誤訊息：

- 無法在 Microsoft Online Services 中更新此物件，因為與此物件關聯的下列屬性的值可能已經與您的本機目錄中的另一個物件相關聯。

- 您的 Microsoft Online Services 目錄中已存在具有相同 proxy 位址的同步處理物件。

- 由於下列與此物件相關聯的屬性的值可能已經與您的本機目錄服務中的另一個物件相關聯，所以無法更新此物件： UserPrincipalName。

若要找出並修正問題，請下載並執行 [IdFix DirSync 錯誤修正工具](https://www.microsoft.com/download/details.aspx?id=36832)。

如需詳細資訊，請參閱 [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。
