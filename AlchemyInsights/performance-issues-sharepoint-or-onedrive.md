---
title: Các vấn đề về hiệu suất-SharePoint hoặc OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771923"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint hoặc OneDrive chậm, không thể truy nhập hoặc không có sẵn cho nhiều người dùng

SharePoint hoặc OneDrive có thể chậm, không thể truy nhập hoặc không sẵn dùng hoặc có thể hiển thị các lỗi không sẵn dùng hoặc 503, vì một vài lý do:
  
- Nếu site SharePoint hoặc OneDrive của bạn chậm hoặc bị trì hoãn đối với nhiều người dùng, có thể có sự cố dịch vụ tạm thời mà người dùng gặp phải sự chậm trễ hoặc dẫn hướng lỗi khi truy nhập site SharePoint hoặc nội dung OneDrive. Kiểm tra [bảng điều khiển trạng thái dịch vụ](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) để xem liệu tổ chức của bạn có bị ảnh hưởng không.
  
- Người dùng có thể nhận được một *máy chủ 503 là lỗi bận rộn* khi tìm cách dẫn hướng đến các site SharePoint hoặc OneDrive. Lỗi này có thể được gây ra bởi điều chỉnh bên trong dịch vụ SharePoint. SharePoint Online sử dụng điều chỉnh để duy trì hiệu năng và độ tin cậy tối ưu của dịch vụ SharePoint Online. Throttling giới hạn số lượng hành động của người dùng hoặc cuộc gọi đồng thời (theo script hoặc mã) để ngăn chặn việc sử dụng tài nguyên. Để biết thêm thông tin về việc xem thử điều chỉnh, [tránh bị Throttled hoặc bị chặn trong SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Nếu bạn **gặp sự hiệu** suất chậm với trang hoặc site SharePoint **hiện đại hoặc hiện đại** , hãy sử dụng [công cụ chẩn đoán trang](https://aka.ms/perftool) để phân tích các trang.
  
- Nếu bạn vẫn còn trải nghiệm hiệu năng chậm chung, vui lòng xem lại các tài nguyên ở cuối bài viết này: [giới thiệu về hiệu năng Tuning cho SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  