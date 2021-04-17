---
title: MC210173-SharePoint Designer tùy chỉnh tính năng biểu mẫu mới trong việc phản đối
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831828"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173-SharePoint Designer tùy chỉnh tính năng biểu mẫu mới trong việc phản đối

Chúng tôi đã xác định được sự cố ảnh hưởng đến chức năng của SharePoint Designer để [tạo các biểu mẫu tùy chỉnh](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) trong SharePoint Online. Sau khi kiểm tra cẩn thận, chúng tôi đã xác định rằng không có bản sửa lỗi đã biết về sự cố này và đã được bầu để tắt tính năng tạo biểu mẫu tùy chỉnh có hiệu lực như 3:00 AM UTC vào thứ bảy tháng tư 25, 2020. Thay đổi này không ảnh hưởng đến khả năng chỉnh sửa các biểu mẫu đã tạo trước đó hoặc các tính năng hiện có khác trong trình thiết kế SharePoint Online.

Sau khi thực hiện thay đổi này, người dùng có thể đã nhận được lỗi: "không thể lưu các thay đổi trong danh sách đối với máy chủ" khi tạo biểu mẫu mới.

Những người dùng trước đây đã thừa hưởng SharePoint Designer để tạo biểu mẫu tùy chỉnh thay vì có thể sử dụng [Powerapps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) cho mục đích này.

PowerApps là một công cụ dễ dàng và mạnh mẽ cho phép người dùng hoạt động trong trải nghiệm hiện đại của SharePoint Online để tạo và chỉnh sửa các biểu mẫu tùy chỉnh cho danh sách SharePoint và thư viện tài liệu ngay từ cửa sổ trình duyệt. PowerApps không yêu cầu kiến thức mã hóa truyền thống hoặc bất kỳ ứng dụng tải nào bổ sung nào chẳng hạn như InfoPath.

**Lưu ý**: người dùng SharePoint Online cổ điển sẽ cần tạm thời chuyển sang trải nghiệm hiện đại để truy nhập và sử dụng powerapps; Tuy nhiên, tất cả các biểu mẫu tùy chỉnh được tạo trong PowerApps có thể truy nhập được bởi người dùng SharePoint Online kinh nghiệm cổ điển.
