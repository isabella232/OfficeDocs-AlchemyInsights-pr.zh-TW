---
title: 929 deflectTransport 規則的收件匣規則
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/15/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 45c542191dd5ef67cef464e1f204358471c21948
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: zh-TW
ms.lasthandoff: 02/12/2019
ms.locfileid: "29928575"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="a8d3d-102">郵件流程規則 （也稱為傳輸規則）</span><span class="sxs-lookup"><span data-stu-id="a8d3d-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="a8d3d-103">郵件流程規則的一般概觀： [Mail flow 規則 （傳輸規則） 在 [Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="a8d3d-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>
    
- <span data-ttu-id="a8d3d-104">設定郵件流程規則： [Mail flow 規則程序在 Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="a8d3d-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>
    
- <span data-ttu-id="a8d3d-105">建立、 修改及刪除郵件流程規則：[管理郵件流程規則](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="a8d3d-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>
    
<span data-ttu-id="a8d3d-p101">您也可以管理 Exchange Online PowerShell 中的郵件流程規則。如需詳細資訊，請參閱[Get-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) （檢視） [New-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) （建立） [Remove-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) （刪除）、 [Set-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) （修改現有的） [Disable-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) （停用現有） 和[Enable-transportrule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule)（啟用現有）。</span><span class="sxs-lookup"><span data-stu-id="a8d3d-p101">You can also manage mail flow rules in Exchange Online PowerShell. For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span> 
  
<span data-ttu-id="a8d3d-108">額外的郵件流程規則指令程式： [Get-transportruleaction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) （清單可用的動作）、 [Get-transportrulepredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) （清單可用條件和例外狀況）、 [Export-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) （匯出規則） 及[匯入 TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) （匯入規則）。</span><span class="sxs-lookup"><span data-stu-id="a8d3d-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span> 
  

