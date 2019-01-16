---
title: Không thể thêm mặc định năm 2010 phê duyệt quy trình làm việc
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2060c9a1-e714-4d93-925e-629c82c35986
ms.openlocfilehash: 758b0339b842478f9609eb716b5b4ddab6579c80
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320048"
---
# <a name="cant-add-default-2010-approval-workflow"></a>Không thể thêm mặc định năm 2010 phê duyệt quy trình làm việc

Trong một bộ sưu tập trang web Microsoft SharePoint, bạn không thể thêm một công việc toàn cầu tái sử dụng (ví dụ như "phê duyệt - SharePoint 2010") một danh sách hoặc thư viện.
  
Để giải quyết vấn đề này, hãy làm theo các bước sau: 
  
1. Mở trang web gốc của bộ sưu tập trang web trong SharePoint Designer 2013.
  
2. Theo **Các đối tượng trang web**, hãy chọn **công việc**. 
  
3. Trong phần **mới** của ribbon **quy trình công việc** , hãy chọn **Công việc tái sử dụng**. 
  
4. Các hình thức **Tạo ra công việc tái sử dụng** , hãy nhập tên * **Repair2010***. Đối với **Nền tảng loại**, chọn **SharePoint 2010 quy trình làm việc**, và sau đó chọn **OK**. 
  
5. Trong phần **lưu** của ribbon **luồng công việc** , chọn **xuất bản**. 
  
6. Trong phần **quản lý** các ribbon **luồng công việc** , chọn **Xuất bản trên toàn cầu**. Trong hộp thoại xác nhận xuất hiện, chọn **OK**. 
  
7. Trình duyệt web, xác định vị trí các trang web gốc của bộ sưu tập trang web, và sau đó truy cập vào **Thiết lập trang web** \> **Tính năng bộ sưu tập trang web**. Sau đó, bật/tắt tính năng **công việc** : 
  
· Nếu các tính năng là *kích hoạt* , hãy nhấp vào **vô hiệu hóa,** và sau đó nhấp vào **kích hoạt**. 
  
· Nếu các tính năng *Deactivated* , bấm **kích hoạt**. 
  
Thông tin chi tiết vui lòng tham khảo sau đây [bài viết](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).
  

