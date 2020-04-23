---
title: 929 quy tắc hộp thư đến để deflectTransport quy tắc
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: 6b6e64c0332a579e8f6132b08f2f89b15eb4de27
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43724614"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a><span data-ttu-id="3d0eb-102">Quy tắc luồng thư (còn được gọi là quy tắc truyền tải)</span><span class="sxs-lookup"><span data-stu-id="3d0eb-102">Mail flow rules (also known as transport rules)</span></span>

- <span data-ttu-id="3d0eb-103">Tổng quan chung về quy tắc luồng thư: [quy tắc luồng thư (quy tắc truyền tải) trong Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span><span class="sxs-lookup"><span data-stu-id="3d0eb-103">General overview of mail flow rules: [Mail flow rules (transport rules) in Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)</span></span>

- <span data-ttu-id="3d0eb-104">Thiết lập quy tắc luồng thư: quy [trình quy tắc luồng thư trong Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span><span class="sxs-lookup"><span data-stu-id="3d0eb-104">Setup mail flow rules: [Mail flow rule procedures in Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)</span></span>

- <span data-ttu-id="3d0eb-105">Tạo, sửa đổi và xóa quy tắc luồng thư: [quản lý quy tắc luồng thư](https://technet.microsoft.com/library/jj657505.aspx)</span><span class="sxs-lookup"><span data-stu-id="3d0eb-105">Create, modify, and delete mail flow rules: [Manage mail flow rules](https://technet.microsoft.com/library/jj657505.aspx)</span></span>

<span data-ttu-id="3d0eb-106">Bạn cũng có thể quản lý quy tắc luồng thư trong Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="3d0eb-106">You can also manage mail flow rules in Exchange Online PowerShell.</span></span> <span data-ttu-id="3d0eb-107">Để biết thêm thông tin, xem [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (xem), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (tạo), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (xóa), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (sửa đổi hiện có), [vô hiệu hóa-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (vô hiệu hóa hiện có), và [kích hoạt-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (kích hoạt sẵn có).</span><span class="sxs-lookup"><span data-stu-id="3d0eb-107">For more information, see [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (view), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (create), [Remove-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (modify existing), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (disable existing), and [Enable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (enable existing).</span></span>

<span data-ttu-id="3d0eb-108">Các lệnh ghép ngắn quy tắc luồng thư bổ sung: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (danh sách các hành động có sẵn), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (danh sách các điều kiện có sẵn và ngoại lệ), [transportrulecollection xuất](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) khẩu (quy tắc xuất khẩu), và [transportrulecollection nhập](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) khẩu (quy tắc nhập).</span><span class="sxs-lookup"><span data-stu-id="3d0eb-108">Additional mail flow rule cmdlets: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (list available actions), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (list available conditions and exceptions), [Export-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (export rules), and [Import-TransportRuleCollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (import rules).</span></span>
