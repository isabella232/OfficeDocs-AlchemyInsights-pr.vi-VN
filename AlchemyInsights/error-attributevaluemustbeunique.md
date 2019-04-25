---
title: Lỗi AttributeValueMustBeUnique
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: bf8ac830-6f0c-4616-827d-987616700e59
ms.openlocfilehash: 7fc1190fb7b93dce945e366cf8b90112a97a2f3f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/23/2019
ms.locfileid: "32402725"
---
# <a name="error-attributevaluemustbeunique"></a>Lỗi: AttributeValueMustBeUnique

Các lý do phổ biến nhất cho các lỗi AttributeValueMustBeUnique là hai đối tượng với khác nhau SourceAnchor (immutableId) có cùng một giá trị cho các thuộc tính ProxyAddresses và/hoặc UserPrincipalName. Để khắc phục lỗi AttributeValueMustBeUnique:
  
1. Xác định proxyAddresses trùng lặp, userPrincipalName hoặc giá trị thuộc tính đó gây ra lỗi. Cũng xác định hai (hay nhiều) các đối tượng được tham gia vào cuộc xung đột. Báo cáo được tạo ra bởi Azure quảng cáo kết nối sức khỏe cho đồng bộ có thể giúp bạn xác định hai đối tượng.
    
2. Xác định các đối tượng mà nên tiếp tục có giá trị trùng lặp và đối tượng mà không nên.
    
3. Loại bỏ các giá trị trùng lặp từ các đối tượng mà không cần phải có giá trị đó. Lưu ý rằng bạn nên thực hiện những thay đổi trong thư mục nơi mà các đối tượng có nguồn gốc từ. Trong một số trường hợp, bạn có thể cần xóa một trong các đối tượng trong cuộc xung đột.
    
4. Nếu bạn thực hiện những thay đổi trong các cơ sở trên quảng cáo, cho Azure quảng cáo kết nối đồng bộ thay đổi đối với các lỗi được cố định.
    

