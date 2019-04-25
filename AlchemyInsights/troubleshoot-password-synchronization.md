---
title: Khắc phục sự cố đồng bộ hoá mật khẩu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 1320c0fe839337188162824439be6f15f86b6c90
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32390477"
---
# <a name="troubleshoot-password-synchronization"></a>Khắc phục sự cố đồng bộ hoá mật khẩu

Để khắc phục sự cố mà không có mật khẩu là đồng bộ hóa với phiên bản Azure quảng cáo kết nối 1.1.614.0 hoặc sau này:
  
1. Mở một phiên Windows PowerShell mới trên máy chủ Azure quảng cáo kết nối của bạn với tùy chọn **Run as Administrator** . 
    
2. Chạy **thiết lập-ExecutionPolicy thành RemoteSigned** hoặc **thiết lập-ExecutionPolicy không giới hạn**. 
    
3. Khởi động thuật sĩ Azure quảng cáo kết nối.
    
4. Điều hướng đến các ** nhiệm vụ bổ sung ** trang, chọn ** khắc phục **, và nhấp vào **tiếp theo**. 
    
5. Trên trang giải đáp thắc mắc, hãy nhấp vào trình đơn **khởi động để bắt đầu việc khắc phục sự cố** trong PowerShell. 
    
6. Trong menu chính, chọn **Khắc phục sự cố đồng bộ hoá mật khẩu**. 
    
7. Trong trình đơn phụ, chọn **đồng bộ hoá mật khẩu không hoạt động ở tất cả**. 
    
 **Hiểu các kết quả của công tác khắc phục sự cố**
  
Nhiệm vụ khắc phục sự cố thực hiện kiểm tra sau đây:
  
- Xác nhận rằng tính năng đồng bộ hoá mật khẩu được kích hoạt cho người thuê nhà Azure quảng cáo của bạn.
    
- Xác nhận rằng Azure quảng cáo kết nối máy chủ không phải là trong dàn chế độ.
    
- Đối với mỗi chỗ hiện kết nối hoạt động thư mục (mà tương ứng với một cụm nhánh Active Directory hiện có):
    
- 
  - Xác nhận rằng tính năng đồng bộ hoá mật khẩu được kích hoạt.
    
  - Đang tìm kiếm sự kiện nhịp tim đồng bộ hoá mật khẩu trong Nhật ký sự kiện ứng dụng của Windows.
    
  - Đối với mỗi hoạt động thư mục tên miền dưới đầu nối Active Directory tại chỗ:
    
  - Xác nhận rằng tên miền là thể truy cập từ Azure quảng cáo kết nối máy chủ.
    
  - Xác nhận rằng các tài khoản Dịch vụ miền Active Directory (AD DS) được sử dụng bởi kết nối Active Directory tại chỗ có đúng tên người dùng, mật khẩu, và các quyền cần thiết để đồng bộ hoá mật khẩu.
    
Để thêm trợ giúp khắc phục sự cố đồng bộ mật khẩu, hãy xem [đồng bộ hoá mật khẩu khắc phục với Azure quảng cáo kết nối đồng bộ](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).
  

