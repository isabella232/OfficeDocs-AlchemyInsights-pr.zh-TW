---
title: Azure AD 多重要素驗證
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: 8a912b32dee23e8c6eae0ad7bc72228d49ceeb92
ms.sourcegitcommit: 4f7ff981bbb3a98663cd164d0a10bb082cdf7ec9
ms.translationtype: HT
ms.contentlocale: zh-TW
ms.lasthandoff: 03/25/2020
ms.locfileid: "42946610"
---
# <a name="unexpected-multi-factor-authentication"></a>Azure AD 多重要素驗證

如果您的租用戶是在 2019 年 10 月 21 日之後建立，且意外收到 MFA 的提示，則可能已在租用戶中啟用[安全性預設值](http://aka.ms/securitydefaults)。 

若要管理安全性預設值：

1. 使用全域系統管理員認證登入[系統管理中心](https://go.microsoft.com/fwlink/p/?linkid=834822)。

2. 移至 [Azure Active Directory 屬性](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties)。

3. 在頁面底部，按一下 [管理安全性預設]****。

4. 按一下 [是]**** 可啟用安全性預設，以及 [否]**** 可停用安全性預設。
