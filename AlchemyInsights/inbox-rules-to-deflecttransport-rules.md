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
ms.custom: 929
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 880f4cb2c42a564362ad7832ebf8ced16fd26d77
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859378"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="e0fc1-102">Quy tắc dòng chảy thư (còn được gọi là quy tắc truyền tải)</span><span class="sxs-lookup"><span data-stu-id="e0fc1-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="e0fc1-103">Tổng quan của quy tắc dòng chảy thư: [thư chảy nội quy (quy tắc truyền tải) trong Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="e0fc1-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="e0fc1-104">Thiết lập quy tắc dòng chảy thư: [thư lưu quy tắc thủ tục trong Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="e0fc1-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="e0fc1-105">Tạo, chỉnh sửa và xóa quy tắc dòng chảy thư: [quản lý thư quy tắc dòng chảy](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="e0fc1-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="e0fc1-106">Bạn cũng có thể quản lý các quy tắc dòng chảy thư trong Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="e0fc1-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="e0fc1-107">Để biết thêm thông tin, hãy xem [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (xem), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (tạo), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Thiết lập-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (sửa đổi hiện có), [Vô hiệu hoá-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (vô hiệu hóa hiện có), và [Kích hoạt-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (cho phép tồn tại).</span><span class="sxs-lookup"><span data-stu-id="e0fc1-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="e0fc1-108">Lệnh ghép ngắn quy tắc dòng chảy bổ sung thư: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (danh sách có sẵn hành động), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (danh sách có điều kiện và ngoại lệ), [Xuất khẩu-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (xuất khẩu nội quy) và [ Nhập khẩu-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (nhập khẩu quy định).</span><span class="sxs-lookup"><span data-stu-id="e0fc1-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
