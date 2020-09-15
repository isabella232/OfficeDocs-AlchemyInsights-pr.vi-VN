---
title: Truy nhập bị từ chối khi xem dòng công việc
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 710775e8b2dee98969df7a4c8410a3e61181aaf6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688824"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Truy nhập bị từ chối khi xem dòng công việc

Dòng công việc SharePoint 2013 cố gắng gửi email đến một nhóm SharePoint có thể không thành công với thông báo lỗi "truy nhập bị từ chối" nếu là thành viên của nhóm SharePoint không được đặt là tất cả mọi người.
  
 **Để giải quyết vấn đề này, hãy thực hiện các bước sau:**
  
 1. Cho phép mọi người nhìn thấy các thành viên của nhóm SharePoint.
  
 2. Loại bỏ nhóm SharePoint khỏi dòng đến hoặc CC của email.
  
 3. Rõ ràng thêm người dùng vào dòng đến hoặc CC nếu không thể thay đổi khả năng hiển thị thành viên cho nhóm SharePoint.
  
Để xem thêm chi tiết, vui lòng tham khảo http không được [phép đến/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  