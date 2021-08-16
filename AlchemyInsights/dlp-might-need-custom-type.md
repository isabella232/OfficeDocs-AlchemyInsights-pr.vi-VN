---
title: DLP có thể cần một loại tùy chỉnh
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030816"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP có thể cần một loại tùy chỉnh

**Quan** trọng: Trong những khoảng thời gian chưa phát hành này, chúng tôi đang thực hiện các bước nhằm đảm bảo rằng các dịch vụ SharePoint Online và OneDrive luôn rất sẵn dùng – Vui lòng truy nhập điều chỉnh Tính năng Tạm thời [SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**DLP có thể yêu cầu một loại thông tin tùy chỉnh**

Với chính sách ngăn mất dữ liệu (DLP), bạn có thể nhận dạng và bảo vệ dữ liệu nhạy cảm trong tổ chức của mình. Trong một số kịch bản, bạn có thể cần tạo kiểu thông tin nhạy **cảm** tùy chỉnh của riêng mình để bảo vệ dữ liệu của tổ chức bạn.

Ví dụ: tổ chức của bạn có thể cần xác định và bảo vệ ID nhân viên hoặc dữ liệu khác ở một số định dạng dành riêng cho tổ chức của bạn. Nếu vậy, hãy xem các bài viết sau đây để biết thêm thông tin.
  
 **Tùy chỉnh kiểu thông tin nhạy cảm dựng sẵn**
  
Nếu một kiểu thông tin nhạy cảm cài sẵn sẽ đáp ứng được nhu cầu của bạn chỉ bằng một vài tinh chỉnh, bạn có thể tùy chỉnh kiểu thông tin nhạy cảm [cài sẵn.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Ví dụ: bạn có thể thêm hoặc loại bỏ các từ khóa hoặc thêm hoặc loại bỏ bằng chứng hỗ trợ như ngày hoặc địa chỉ.
  
 **Tạo kiểu thông tin nhạy cảm tùy chỉnh**
  
Nhưng nếu bạn cần nhận dạng và bảo vệ hoàn toàn [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) các loại thông tin nhạy cảm khác, bạn có thể tạo kiểu thông tin nhạy cảm tùy chỉnh trong giao diện người dùng của Trung tâm Bảo mật & Tuân thủ.
  
**Tạo kiểu thông tin nhạy cảm tùy chỉnh trong Trung tâm Bảo & Tuân thủ PowerShell**

Cuối cùng, nếu UI không cung cấp tất cả tùy chọn bạn cần, bạn có thể tạo loại thông tin nhạy cảm tùy chỉnh trong Trung tâm Bảo [mật & Compliance Center PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Bằng cách bắt đầu với một tệp XML, bạn có thể dùng tất cả các tùy chọn sẵn dùng.
