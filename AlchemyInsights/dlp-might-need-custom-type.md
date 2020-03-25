---
title: DLP có thể cần một loại tùy chỉnh
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932680"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP có thể cần một loại tùy chỉnh

**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền. Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu. Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.

Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần. Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này. Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.

**DLP có thể yêu cầu loại thông tin tùy chỉnh**

Với chính sách ngăn chặn mất dữ liệu (DLP), bạn có thể xác định và bảo vệ dữ liệu nhạy cảm trong tổ chức của mình. Trong một số trường hợp, bạn có thể cần phải tạo loại thông tin nhạy cảm **tùy chỉnh** của riêng mình để bảo vệ dữ liệu của tổ chức.

Ví dụ: tổ chức của bạn có thể cần phải xác định và bảo vệ ID nhân viên hoặc dữ liệu khác ở một số định dạng cụ thể cho sơ của bạn. Nếu có, hãy xem các bài viết sau để biết thêm thông tin.
  
 **Tùy chỉnh loại thông tin nhạy cảm tích hợp sẵn**
  
Nếu một loại thông tin nhạy cảm được tích hợp sẵn đáp ứng nhu cầu của bạn chỉ bằng một vài tinh chỉnh, bạn có thể [tùy chỉnh loại thông tin nhạy cảm tích hợp sẵn](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Ví dụ: bạn có thể thêm hoặc xóa từ khóa hoặc thêm hoặc xóa bằng chứng hỗ trợ như ngày hoặc địa chỉ.
  
 **Tạo loại thông tin nhạy cảm tùy chỉnh**
  
Nhưng nếu bạn cần xác định và bảo vệ một loại thông tin nhạy cảm khác nhau hoàn toàn, bạn có thể [tạo một loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) trong giao diện người dùng của Trung tâm tuân thủ & bảo mật.
  
**Tạo một loại thông tin nhạy cảm tùy chỉnh trong bảo mật & tuân thủ trung tâm PowerShell**

Cuối cùng, nếu giao diện người dùng không cung cấp tất cả các tùy chọn bạn cần, bạn có thể [tạo một loại thông tin nhạy cảm tùy chỉnh trong bảo mật & tuân thủ trung tâm PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Bằng cách bắt đầu với một tập tin XML, bạn có thể sử dụng tất cả các tùy chọn có sẵn.
