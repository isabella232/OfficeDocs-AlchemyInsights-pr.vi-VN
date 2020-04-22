---
title: Hạn chế quyền truy cập trong SharePoint hoặc OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: ed8e97b20c96a7b46995c969074cc4cef3a787d9
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43715906"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a>Hạn chế quyền truy cập trong SharePoint hoặc OneDrive

Trong SharePoint và OneDrive, bạn hạn chế quyền truy cập vào các mục như tệp, thư mục và danh sách bằng cách cấp quyền truy cập chỉ cho các nhóm hoặc cá nhân bạn muốn có quyền truy cập. Theo mặc định, quyền trong SharePoint được kế thừa từ cao hơn trong hệ thống phân cấp. Vì vậy, một tệp kế thừa các quyền của nó từ thư mục, kế thừa các quyền của nó từ thư viện, kế thừa các quyền từ trang web.
  
Bạn có thể chia sẻ ở một mức độ cao hơn (chẳng hạn như bằng cách chia sẻ toàn bộ trang web) và sau đó phá vỡ thừa kế nếu bạn không muốn chia sẻ tất cả các mục trên trang web. Tuy nhiên, chúng tôi không khuyên bạn nên điều này vì nó làm cho việc duy trì các quyền phức tạp hơn và khó hiểu trong tương lai. Đây là những gì bạn có thể làm thay vì:
  
- Ví dụ: nếu bạn muốn chia sẻ tất cả nội dung của thư mục ngoại trừ một tệp trong đó, hãy di chuyển tệp đó sang vị trí mới không được chia sẻ.
    
- Nếu bạn có hai cặp con trong một thư mục, và bạn muốn chia sẻ một cặp với nhóm A và B và cho phép chỉ nhóm quyền truy cập vào thư mục con thứ hai, hãy chia sẻ cặp cha với nhóm A và thêm nhóm B vào con đầu tiên.
    
[Dừng chia sẻ tệp hoặc thư mục](https://go.microsoft.com/fwlink/?linkid=2008861)
  

