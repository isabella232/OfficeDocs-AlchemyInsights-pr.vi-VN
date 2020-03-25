---
title: DLP không hoạt động như mong đợi
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932644"
---
# <a name="dlp-not-working-as-expected"></a>DLP không hoạt động như mong đợi

**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền. Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu. Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.

Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần. Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này. Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.

 **Thiết lập DLP**

Bạn có vấn đề với **ngăn mất dữ liệu (DLP)** trong Office 365 không hoạt động như mong đợi? Nếu có, đảm bảo rằng **chính sách DLP** của bạn được thiết lập chính xác và dữ liệu của bạn chứa những gì **chính sách DLP** đang tìm kiếm khi nó được đánh giá.
  
Chính sách DLP cho phép bạn xác định và bảo vệ thông tin nhạy cảm trong tổ chức của bạn. Thiết lập chính sách DLP, sử dụng thông tin [ở đây](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp).
  
 **Chính sách DLP nào tìm kiếm**
  
Khi sử dụng các **loại thông tin nhạy cảm tích hợp** trong Office 365 Trung tâm bảo mật và tuân thủ, chính sách DLP tìm các mẫu và yếu tố cụ thể khi phát hiện các loại nhạy cảm.
  
- **Tích hợp các loại thông tin nhạy cảm**

    Để biết thông tin về các loại nhạy cảm và chính sách DLP sẽ tìm kiếm khi phát hiện loại nhạy cảm, hãy xem: [những loại thông tin nhạy cảm tìm kiếm](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Các loại thông tin nhạy cảm tùy chỉnh**

    Nếu bạn đang cố gắng tạo các loại thông tin nhạy cảm tùy chỉnh, hãy sử dụng bài viết sau để biết thông tin về cách tạo loại nhạy cảm tùy chỉnh: [tạo loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**Kiểm tra chính sách DLP**

Để kiểm tra dữ liệu của bạn bằng loại thông tin nhạy cảm được tích hợp hoặc tùy chỉnh, hãy **Classifications** > sử dụng tùy chọn **loại thử nghiệm** trong phân**loại thông tin nhạy cảm**. Để biết thêm thông tin, xem [kiểm tra các loại thông tin nhạy cảm tùy chỉnh](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Báo cáo**
  
- Nhận thông tin chi tiết dữ liệu nhạy cảm với [báo cáo DLP.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Xem chi tiết cụ thể của sự kiện với [báo cáo](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports)việc làm.
