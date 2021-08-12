---
title: Sự cố về hiệu suất SharePoint hoặc sự OneDrive
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
ms.openlocfilehash: 921aae7eba8487c5600f290fd671ef2675372e6af0478b913e38354856cbaa22
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53911864"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a>SharePoint hoặc OneDrive, không thể truy nhập hoặc không sẵn dùng đối với nhiều người dùng

SharePoint hoặc OneDrive có thể chậm, không thể tiếp cận hoặc không sẵn dùng hoặc có thể hiển thị các lỗi dịch vụ không sẵn dùng hoặc 503 vì một số lý do:
  
- Nếu site SharePoint hoặc OneDrive của bạn chậm hoặc bị trì hoãn đối với nhiều người dùng thì có thể xảy ra sự cố dịch vụ tạm thời trong đó người dùng gặp phải sự cố chậm trễ hoặc lỗi dẫn hướng không liên tục khi truy nhập site SharePoint hoặc nội dung OneDrive. Kiểm tra bảng [điều khiển Tình trạng dịch](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) vụ để xem liệu tổ chức của bạn có bị ảnh hưởng không.
  
- Người dùng có thể nhận được lỗi máy chủ *503* đang bận khi tìm cách dẫn hướng đến các SharePoint hoặc OneDrive của họ. Lỗi này có thể xảy ra do điều chỉnh trong dịch SharePoint vụ. SharePoint Online sử dụng điều chỉnh để duy trì hiệu suất tối ưu và độ tin cậy của dịch SharePoint Online. Điều chỉnh giới hạn số lượng hành động người dùng hoặc cuộc gọi đồng thời (theo tập lệnh hoặc mã) để ngăn chặn việc sử dụng quá nhiều tài nguyên. Để biết thêm thông tin về điều chỉnh, hãy xem [mục Tránh bị điều chỉnh hoặc chặn trong SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

- Nếu bạn trải nghiệm hiệu năng chậm **với** site hoặc trang **SharePoint** điển hoặc hiện đại, hãy sử dụng công [cụ Chẩn](https://aka.ms/perftool) đoán trang để phân tích trang.
  
- Nếu bạn vẫn gặp phải hiệu năng chậm nói chung, vui lòng xem lại các tài nguyên ở cuối bài viết này: Giới thiệu về tinh chỉnh [hiệu suất cho SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)
  