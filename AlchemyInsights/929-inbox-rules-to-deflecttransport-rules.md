---
title: 929 các quy tắc hộp thư đến để quy tắc deflectTransport
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
ms.contentlocale: vi-VN
ms.lasthandoff: 02/12/2019
ms.locfileid: "29928606"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="e5b0a-102">Quy tắc dòng chảy thư (còn được gọi là quy tắc truyền tải)</span><span class="sxs-lookup"><span data-stu-id="e5b0a-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="e5b0a-103">Tổng quan của quy tắc dòng chảy thư: [thư chảy nội quy (quy tắc truyền tải) trong Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="e5b0a-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>
    
- <span data-ttu-id="e5b0a-104">Thiết lập quy tắc dòng chảy thư: [thư lưu quy tắc thủ tục trong Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="e5b0a-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>
    
- <span data-ttu-id="e5b0a-105">Tạo, chỉnh sửa và xóa quy tắc dòng chảy thư: [quản lý thư quy tắc dòng chảy](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="e5b0a-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>
    
<span data-ttu-id="e5b0a-p101">Bạn cũng có thể quản lý các quy tắc dòng chảy thư trong Exchange Online PowerShell. Để biết thêm thông tin, hãy xem [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (xem), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (tạo), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Thiết lập-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (sửa đổi hiện có), [Vô hiệu hoá-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (vô hiệu hóa hiện có), và [Kích hoạt-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (cho phép tồn tại).</span><span class="sxs-lookup"><span data-stu-id="e5b0a-p101">You can also manage mail flow rules in Exchange Online PowerShell. For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span> 
  
<span data-ttu-id="e5b0a-108">Lệnh ghép ngắn quy tắc dòng chảy bổ sung thư: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (danh sách có sẵn hành động), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (danh sách có điều kiện và ngoại lệ), [Xuất khẩu-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (xuất khẩu nội quy) và [ Nhập khẩu-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (nhập khẩu quy định).</span><span class="sxs-lookup"><span data-stu-id="e5b0a-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span> 
  

