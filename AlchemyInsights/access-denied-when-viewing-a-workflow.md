---
title: Truy cập từ chối khi xem một công việc
ms.author: kirks
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: b7a3805d30cac44781adbbb00c0f0ed3496ff17b
ms.sourcegitcommit: a9be2e396022382e92cf40c0d0d82f2f59c2e259
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/12/2019
ms.locfileid: "34883613"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Truy cập từ chối khi xem một công việc

SharePoint 2013 quy trình công việc mà cố gắng để gửi email đến một nhóm SharePoint có thể thất bại với một thông báo lỗi "Truy cập từ chối" nếu các thành viên của nhóm SharePoint không được thiết lập để tất cả mọi người.
  
 **Để giải quyết vấn đề này, hãy làm các bước sau:**
  
 1. Cho phép tất cả mọi người để xem các thành viên của nhóm SharePoint.
  
 2. Loại bỏ nhóm SharePoint từ k/g hoặc sao của email.
  
 3. Một cách rõ ràng thêm người dùng k/g hoặc sao dòng nếu tầm nhìn của thành viên không thể thay đổi cho SharePoint group.
  
Để xem thêm chi tiết xin vui lòng tham khảo [HTTP trái phép để /_vti_bin/client.svc/sp.utilities.utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  