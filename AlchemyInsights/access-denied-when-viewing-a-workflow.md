---
title: Access denied when viewing a Workflow
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 2b076ec5dca070555ce51b88631fb6bd619ed9269e59ccc799b23b8b95547c16
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53955223"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Access denied when viewing a Workflow

SharePoint 2013 Dòng công việc cố gắng gửi email đến nhóm SharePoint có thể thất bại với thông báo lỗi "Truy nhập Bị từ chối" nếu tư cách thành viên của nhóm SharePoint không được đặt thành Mọi người.
  
 **Để giải quyết vấn đề này, hãy thực hiện các bước sau:**
  
 1. Cho phép tất cả mọi người thấy các thành viên của SharePoint nhóm.
  
 2. Loại bỏ SharePoint nhóm người dùng khỏi dòng Tới hoặc CC của email.
  
 3. Thêm người dùng một cách rõ ràng vào dòng Tới hoặc CC nếu không thể thay đổi khả năng hiển thị tư cách thành viên SharePoint nhóm.
  
Để xem thêm chi tiết, vui lòng tham khảo HTTP Trái phép tới [/_vti_bin/client.svc/sp.utilities.utility.SendEmail.](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409)
  