---
title: quy tắc hộp thư đến 929 để deflectTransport Rules
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "929"
- "1800021"
ms.assetid: 9733ef4e-db8d-4345-a072-c251480875a1
ms.openlocfilehash: abb729c40fb87bcca8cc03c95aa4677597d20c08
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47778713"
---
# <a name="mail-flow-rules-also-known-as-transport-rules"></a>Các quy tắc dòng thư (còn được gọi là quy tắc truyền dẫn)

- Tổng quan chung về các quy tắc dòng thư: [quy tắc dòng thư (quy tắc truyền dẫn) trong Exchange Online](https://technet.microsoft.com/library/jj919238.aspx)

- Thiết lập quy tắc dòng thư: quy trình [quy tắc dòng thư trong Exchange Online](https://technet.microsoft.com/library/dn600436.aspx)

- Tạo, sửa đổi và xóa bỏ quy tắc dòng thư: [quản lý quy tắc dòng thư](https://technet.microsoft.com/library/jj657505.aspx)

Bạn cũng có thể quản lý các quy tắc dòng thư trong Exchange Online PowerShell. Để biết thêm thông tin, hãy xem [Get-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrule) (xem), [New-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/new-transportrule) (tạo), [loại bỏ-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/remove-transportrule) (Delete), [Set-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/set-transportrule) (sửa đổi hiện có), [Disable-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/disable-transportrule) (tắt tính năng hiện có) và [bật-TransportRule](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/enable-transportrule) (bật hiện có).

Các lệnh ghép ngắn về quy tắc dòng thư bổ sung: [Get-TransportRuleAction](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportruleaction) (danh sách các hành động sẵn dùng), [Get-TransportRulePredicate](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/get-transportrulepredicate) (danh sách điều kiện và ngoại lệ sẵn dùng), [Export-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/export-transportrulecollection) (quy tắc xuất) và [nhập-transportrulecollection](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance/import-transportrulecollection) (nhập quy tắc).
