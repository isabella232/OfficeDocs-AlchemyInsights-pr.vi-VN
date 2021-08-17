---
title: DLP không hoạt động như mong đợi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: e1049f160a9b92040095b6725fa5771218a0956d17f99ea8a6e9cc279e7c73f6
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54079724"
---
# <a name="dlp-not-working-as-expected"></a>DLP không hoạt động như mong đợi

**Quan** trọng: Trong những khoảng thời gian chưa phát hành này, chúng tôi đang thực hiện các bước nhằm đảm bảo rằng các dịch vụ SharePoint Online và OneDrive luôn rất sẵn dùng – Vui lòng truy nhập điều chỉnh Tính năng Tạm thời [SharePoint Online](https://aka.ms/ODSPAdjustments) để biết thêm thông tin.

 **Thiết lập DLP**

Bạn đang gặp sự cố với **ngăn mất dữ liệu (DLP)** trong Office 365 việc không hoạt động như mong đợi? Nếu vậy, hãy đảm bảo rằng chính sách **DLP** của bạn được thiết lập chính xác và dữ liệu của bạn chứa những gì chính sách **DLP** đang tìm kiếm khi được đánh giá.
  
Chính sách của DLP cho phép bạn nhận dạng và bảo vệ thông tin nhạy cảm trong tổ chức của mình. Để thiết lập chính sách DLP, hãy sử dụng thông tin [tại đây.](https://docs.microsoft.com/microsoft-365/compliance/create-a-dlp-policy-from-a-template)
  
 **Chính sách của DLP sẽ tìm gì**
  
Khi dùng các **kiểu** thông tin nhạy cảm cài sẵn trong trung tâm Bảo mật và Tuân thủ, chính sách DLP sẽ tìm kiếm các mẫu hình và yếu tố cụ thể khi phát hiện các kiểu nhạy cảm này.
  
- **Các kiểu thông tin nhạy cảm dựng sẵn**

    Để biết thông tin về các kiểu Nhạy cảm cài sẵn và thông tin mà chính sách DLP tìm kiếm khi phát hiện kiểu Nhạy cảm, hãy xem: Kiểu thông tin nhạy cảm sẽ tìm [kiếm những gì.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

- **Các loại thông tin nhạy cảm tùy chỉnh**

    Nếu bạn đang tìm cách tạo kiểu thông tin nhạy cảm tùy chỉnh, hãy dùng bài viết sau đây để biết thông tin về cách tạo kiểu nhạy cảm tùy chỉnh: Tạo kiểu thông tin nhạy [cảm tùy chỉnh.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type)

**Kiểm tra chính sách DLP**

Để kiểm tra dữ liệu của bạn với kiểu thông tin nhạy cảm cài sẵn hoặc tùy chỉnh, hãy dùng tùy chọn Kiểu **kiểm** tra trong các **kiểu thông tin Phân** loại  >  **nhạy cảm.** Để biết thêm thông tin, hãy xem Kiểm [tra các kiểu thông tin nhạy cảm tùy chỉnh.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type#create-custom-sensitive-information-types-in-the-security--compliance-center)

 **Báo cáo**
  
- Nhận thông tin chuyên sâu về dữ liệu nhạy [cảm với Báo cáo DLP.](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#dlp-reports)

- Xem các chi tiết cụ thể của sự kiện với Báo [cáo Sự cố](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies#incident-reports).
