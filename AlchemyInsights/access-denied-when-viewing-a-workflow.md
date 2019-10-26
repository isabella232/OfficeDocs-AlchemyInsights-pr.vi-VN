---
title: Truy nhập bị từ chối khi xem luồng công việc
ms.author: pebaum
author: Techwriter40
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 4ca65583fbd98867026e9e3cc8f36fe38798aa85
ms.sourcegitcommit: 0b06093dabd685f76cc39b1d7c0f8b03883b6e79
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/25/2019
ms.locfileid: "36747770"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Truy nhập bị từ chối khi xem luồng công việc

SharePoint 2013 luồng công việc cố gắng gửi email đến một nhóm SharePoint có thể thất bại với thông báo lỗi "truy cập từ chối" nếu các thành viên của nhóm SharePoint không được đặt thành tất cả mọi người.
  
 **Để khắc phục sự cố này, thực hiện các bước sau:**
  
 1. Cho phép tất cả mọi người xem các thành viên của nhóm SharePoint.
  
 2. Loại bỏ nhóm SharePoint từ hoặc CC dòng email.
  
 3. Rõ ràng thêm người dùng đến hoặc CC dòng nếu Hiển thị thành viên không thể thay đổi cho nhóm SharePoint.
  
Để xem thêm chi tiết xin vui lòng tham khảo [http trái phép để/_vti_bin/client.SVC/SP.Utilities.Utility.SendEmail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  