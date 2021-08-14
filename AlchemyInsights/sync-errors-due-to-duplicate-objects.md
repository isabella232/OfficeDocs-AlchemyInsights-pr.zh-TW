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
ms.openlocfilehash: a047afd63484423520ed80fbf223f0e50f3e02624bd9859d4dcbbd94cf23143f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998772"
---
# <a name="sync-errors-due-to-duplicate-objects"></a>由於重複的物件而產生同步處理錯誤

在 Microsoft 365 中完成目錄同步處理時，您可能會收到下列其中一則錯誤訊息：

- 無法在 Microsoft Online Services 中更新此物件，因為與此物件關聯的下列屬性的值可能已經與您的本機目錄中的另一個物件相關聯。

- 您的 Microsoft Online Services 目錄中已存在具有相同 proxy 位址的同步處理物件。

- 由於下列與此物件相關聯的屬性的值可能已經與您的本機目錄服務中的另一個物件相關聯，所以無法更新此物件： UserPrincipalName。

若要找出並修正問題，請下載並執行 [IdFix DirSync 錯誤修正工具](https://github.com/Microsoft/idfix)。

如需詳細資訊，請參閱 [KB2647098](https://support.microsoft.com/help/2647098/duplicate-or-invalid-attributes-prevent-directory-synchronization-in-o)。
