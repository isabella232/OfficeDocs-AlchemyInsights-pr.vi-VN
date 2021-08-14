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
ms.openlocfilehash: b223bad66fb7cc6d1d7c0a2b3ccc7a081c061b4974060dbcafec84dfb24eb782
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923666"
---
# <a name="when-do-my-profile-changes-sync-to-the-sharepoint-user-profile-application"></a>Khi nào thì thay đổi hồ sơ của tôi đồng bộ với Ứng SharePoint Người dùng?

SharePoint Trực tuyến sử dụng công việc bộ hẹn giờ Nhập Active Directory (AD Import) để nhập người dùng và nhóm vào Ứng dụng Hồ sơ Người dùng. 
  
1. Tính năng Nhập AD sẽ đồng bộ các thay đổi SharePoint Online Directory Store với Ứng dụng Hồ sơ Người dùng. Những thay đổi này được xử lý theo lô.
    
2. Công việc bộ đặt thời gian sẽ chạy cho đến khi các thay đổi được đồng bộ.
    
> [!NOTE]
> Thời gian cần công việc để chạy tùy thuộc vào số lượng thay đổi cần xử lý. Một số lượng lớn các thay đổi sẽ mất nhiều thời gian hơn. Thỏa thuận Mức Dịch vụ (SLA) nêu rằng một thay đổi đối với người dùng trong SharePoint Online Directory sẽ được phản ánh trong Ứng dụng Hồ sơ Người dùng trong 24 giờ. 
  
[Thông tin thêm về đồng bộ hồ sơ người dùng SharePoint Online](https://go.microsoft.com/fwlink/?linkid=875671)
  

