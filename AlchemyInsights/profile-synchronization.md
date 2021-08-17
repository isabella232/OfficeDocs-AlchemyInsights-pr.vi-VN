---
title: Đồng bộ hóa hồ sơ
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6b695be8-eaf5-44ff-b0ae-1e0d89e7ab36
ms.openlocfilehash: a841db70c238bdae58edfca634fe49a04ddce78a
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58320731"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Khi nào thì thay đổi hồ sơ của tôi đồng bộ với Ứng SharePoint Người dùng?

SharePoint Trực tuyến sử dụng công việc bộ hẹn giờ Nhập Active Directory (AD Import) để nhập người dùng và nhóm vào Ứng dụng Hồ sơ Người dùng. 
  
1. Tính năng Nhập AD sẽ đồng bộ các thay đổi SharePoint Online Directory Store với Ứng dụng Hồ sơ Người dùng. Những thay đổi này được xử lý theo lô.
    
2. Công việc bộ đặt thời gian sẽ chạy cho đến khi các thay đổi được đồng bộ.
    
**Lưu** ý : Thời gian cần để chạy công việc phụ thuộc vào số lượng thay đổi cần xử lý. Một số lượng lớn các thay đổi sẽ mất nhiều thời gian hơn. Thỏa thuận Mức Dịch vụ (SLA) nêu rằng một thay đổi đối với người dùng trong SharePoint Online Directory sẽ được phản ánh trong Ứng dụng Hồ sơ Người dùng trong 24 giờ. 
  
[Xem thêm thông tin về việc đồng bộ hồ sơ người SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

