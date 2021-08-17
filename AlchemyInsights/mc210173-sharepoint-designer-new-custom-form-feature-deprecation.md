---
title: MC210173 - Trình SharePoint tính năng Biểu mẫu tùy chỉnh mới
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
ms.openlocfilehash: f72d6ce6931b39d5d4a4835cee0ed2952407b13187213cca5bd483acb1e192bf
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54077702"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a>MC210173 - Trình SharePoint tính năng Biểu mẫu tùy chỉnh mới

Chúng tôi đã xác định một sự cố ảnh hưởng tới SharePoint Designer của bạn [trong việc tạo biểu mẫu tùy](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) chỉnh SharePoint Online. Sau khi kiểm tra cẩn thận, chúng tôi đã xác định rằng không có bản sửa lỗi đã biết nào cho sự cố này và đã chọn tắt tính năng tạo Biểu mẫu tùy chỉnh có hiệu lực kể từ 3:00 AM UTC vào Thứ Bảy, 25 Tháng Tư 2020. Thay đổi này không ảnh hưởng đến khả năng chỉnh sửa biểu mẫu đã tạo trước đó hoặc các tính năng hiện có khác trong trình SharePoint Online Designer.

Sau khi thực hiện thay đổi này, người dùng có thể đã nhận được lỗi: "Không thể lưu các thay đổi trong danh sách vào máy chủ", khi tạo biểu mẫu mới.

Những người dùng trước đây đã tận dụng SharePoint Designer để tạo Biểu mẫu tùy chỉnh thì thay vào đó sẽ có thể sử dụng [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) cho mục đích này.

PowerApps là một công cụ dễ dàng và mạnh mẽ cho phép người dùng hoạt động trong trải nghiệm Hiện đại SharePoint Online để tạo và chỉnh sửa biểu mẫu tùy chỉnh cho danh sách SharePoint và thư viện tài liệu ngay từ cửa sổ trình duyệt. PowerApps không yêu cầu kiến thức mã hóa truyền thống hoặc bất kỳ bản tải xuống ứng dụng bổ sung nào như InfoPath.

**Lưu** ý : SharePoint Online Classic, người dùng sẽ cần tạm thời chuyển sang trải nghiệm Hiện đại để truy nhập và sử dụng PowerApps; tuy nhiên, tất cả các Biểu mẫu tùy chỉnh đã tạo trong PowerApps đều có thể truy nhập bởi SharePoint người dùng trải nghiệm Online Classic.
