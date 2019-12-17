---
title: Vấn đề hiệu suất-SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068443"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint hoặc OneDrive chậm, không thể truy nhập hoặc không khả dụng cho nhiều người dùng

SharePoint hoặc OneDrive có thể chậm, không truy nhập được hoặc không có sẵn hoặc có thể hiển thị dịch vụ không khả dụng hoặc 503 lỗi, vì nhiều lý do:
  
- Nếu trang web SharePoint hoặc OneDrive của bạn chậm hoặc chậm trễ cho nhiều người dùng, có thể có sự cố dịch vụ tạm thời trong đó người dùng gặp phải gián đoạn chậm hoặc điều hướng lỗi khi truy cập trang web SharePoint hoặc nội dung OneDrive. Kiểm tra [bảng điều khiển tình trạng dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng hay không.
  
- Người dùng có thể nhận được một *máy chủ 503 bận* lỗi khi cố gắng di chuyển trang web SharePoint hoặc OneDrive. Lỗi này có thể do điều chỉnh trong dịch vụ SharePoint. SharePoint Online sử dụng điều chỉnh để duy trì hiệu suất tối ưu và độ tin cậy của dịch vụ SharePoint trực tuyến. Điều tiết giới hạn số hành động của người dùng hoặc các cuộc gọi đồng thời (theo tập lệnh hoặc mã) để tránh sử dụng quá nhiều tài nguyên. Để biết thêm thông tin về điều chỉnh xem, [tránh bị điều chỉnh hoặc chặn trong SharePoint trực tuyến](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Nếu bạn gặp phải hiệu suất chậm với một trang web SharePoint hoặc **hiện đại** hoặc **cổ điển** , sử dụng [công cụ chẩn đoán trang](https://aka.ms/perftool) để phân tích các trang.
  
- Nếu bạn vẫn gặp phải hiệu suất chung chậm, vui lòng đánh giá tài nguyên ở cuối bài viết này: [giới thiệu về hiệu suất điều chỉnh cho SharePoint trực tuyến](https://go.microsoft.com/fwlink/?linkid=2024334)
  