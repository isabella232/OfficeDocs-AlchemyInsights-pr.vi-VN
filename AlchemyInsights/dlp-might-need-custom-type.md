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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446713"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP có thể cần một loại tùy chỉnh

Quan **trọng:** Trong những khoảng thời gian chưa phát hành này, chúng tôi đang thực hiện các bước nhằm đảm bảo rằng dịch vụ SharePoint Online và OneDrive luôn khả dụng cao – Vui lòng truy nhập điều chỉnh Tính năng Tạm thời [SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

**DLP có thể yêu cầu một loại thông tin tùy chỉnh**

Với chính sách ngăn mất dữ liệu (DLP), bạn có thể nhận dạng và bảo vệ dữ liệu nhạy cảm trong tổ chức của mình. Trong một số kịch bản, bạn có thể cần tạo kiểu thông tin nhạy cảm tùy chỉnh của riêng mình để bảo vệ dữ liệu của tổ chức bạn. Để biết thêm thông tin, hãy xem Tìm [hiểu về các kiểu thông tin nhạy cảm và](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) Định nghĩa thực thể kiểu thông tin [Nhạy cảm.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Để biết thêm thông tin về cách tạo kiểu và chính sách thông tin nhạy cảm tùy chỉnh, hãy xem: 

**Tùy chỉnh kiểu thông tin nhạy cảm dựng sẵn**

Nếu một kiểu thông tin nhạy cảm cài sẵn sẽ đáp ứng được nhu cầu của bạn chỉ bằng một vài tinh chỉnh, hãy xem Tùy chỉnh kiểu thông tin nhạy cảm [cài sẵn.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Ví dụ: bạn có thể thêm hoặc loại bỏ các từ khóa hoặc thêm hoặc loại bỏ bằng chứng hỗ trợ như ngày hoặc địa chỉ.

**Tạo kiểu thông tin nhạy cảm tùy chỉnh**

Nhưng nếu bạn cần nhận dạng và bảo vệ hoàn toàn các loại thông tin nhạy cảm khác, bạn có thể tạo kiểu thông tin nhạy cảm tùy chỉnh trong trường Trung tâm tuân thủ Microsoft 365. Để biết thêm thông tin, hãy xem [Bắt đầu với các kiểu thông tin nhạy cảm tùy chỉnh.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Tạo kiểu thông tin nhạy cảm tùy chỉnh trong Trung tâm Bảo & Tuân thủ PowerShell**

Cuối cùng, nếu giao diện người dùng không cung cấp tất cả tùy chọn bạn cần, bạn có thể tạo loại thông tin nhạy cảm tùy chỉnh trong Trung tâm Bảo mật & Tuân thủ PowerShell. Bằng cách bắt đầu với một tệp XML, bạn có thể dùng tất cả các tùy chọn sẵn dùng. Để biết thêm thông tin, hãy [xem Tạo kiểu thông tin nhạy cảm tùy chỉnh bằng PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Trước tiên, để kiểm tra [](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) chính sách của bạn trong chế độ kiểm tra, hãy xem mục Triển khai chính sách trong chế độ kiểm tra và Tạo, kiểm tra và [tinh chỉnh chính sách DLP.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 