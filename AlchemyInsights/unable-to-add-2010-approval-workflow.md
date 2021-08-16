---
title: Không thể thêm dòng công việc Phê duyệt 2010
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: e74c842f8b4be321664f8c2f1f58c570d0724d80edb1264add0647bf313bc82f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54020358"
---
# <a name="unable-to-add-2010-approval-workflow"></a>Không thể thêm dòng công việc Phê duyệt 2010

Trong tuyển tập trang Microsoft SharePoint, bạn không thể thêm dòng công việc có thể dùng lại toàn cầu (chẳng hạn như "Phê duyệt - SharePoint 2010") vào danh sách hoặc thư viện.
  
Để giải quyết vấn đề này, hãy làm theo các bước sau: 
  
1. Mở website gốc của tuyển tập site trong SharePoint Designer 2013.
  
2. Dưới **Đối tượng Site,** chọn **Dòng công việc**. 
  
3. Trong phần **Mới của** ribbon Dòng công **việc,** hãy chọn Dòng công **việc có thể dùng lại**. 
  
4. Trên biểu **mẫu Tạo Dòng công việc Có thể dùng** lại, hãy nhập tên ** Sửa *chữa2010* **. Đối **với Loại nền** tảng, bấm SharePoint công việc **2010**, rồi bấm **OK.** 
  
1. Trong phần **Lưu của** ribbon Dòng công **việc,** chọn Phát **hành**. 
  
2. Trong phần **Quản lý** của ribbon Dòng **công việc,** hãy chọn **Phát hành Toàn cầu**. Trong hộp thoại xác nhận xuất hiện, chọn **OK.** 
  
3. In a web browser, locate the root website of the site collection, and then access **Site Cài đặt** Site \> **Collection Features**. Chuyển đổi tính năng **Dòng công** việc: 
  
· Nếu tính năng này *đã là Kích hoạt,* bấm **Hủy kích hoạt,** rồi bấm Kích **hoạt.** 
  
· Nếu tính năng này bị *Hủy kích hoạt,* hãy bấm Kích **hoạt.** 
  
Để biết thêm thông tin, vui lòng tham khảo bài viết [sau.](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409)
  

