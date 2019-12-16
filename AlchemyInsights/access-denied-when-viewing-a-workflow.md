---
title: Truy nhập bị từ chối khi xem luồng công việc
ms.author: pebaum
author: pebaum
ms.date: 11/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 47ceb983-f9a4-4c55-a40c-03d5c3d75dc9
ms.openlocfilehash: 1cfda8e08ada05858a28f2bede8c31261f9de351
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2019
ms.locfileid: "40050547"
---
# <a name="access-denied-when-viewing-a-workflow"></a>Truy nhập bị từ chối khi xem luồng công việc

SharePoint 2013 luồng công việc cố gắng gửi email đến một nhóm SharePoint có thể thất bại với thông báo lỗi "truy cập từ chối" nếu các thành viên của nhóm SharePoint không được đặt thành tất cả mọi người.
  
 **Để khắc phục sự cố này, thực hiện các bước sau:**
  
 1. Cho phép tất cả mọi người xem các thành viên của nhóm SharePoint.
  
 2. Loại bỏ nhóm SharePoint từ hoặc CC dòng email.
  
 3. Rõ ràng thêm người dùng đến hoặc CC dòng nếu Hiển thị thành viên không thể thay đổi cho nhóm SharePoint.
  
Để xem thêm chi tiết, vui lòng tham khảo http không được [phép/_vti_bin/client.SVC/SP.Utilities.Utility.sendemail](https://go.microsoft.com/fwlink/?linkid=2044694&amp;clcid=0x409).
  