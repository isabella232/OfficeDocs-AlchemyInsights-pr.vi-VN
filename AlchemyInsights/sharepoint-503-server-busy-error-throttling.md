---
title: SharePoint trực tuyến throttling
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931248"
---
# <a name="sharepoint-online-throttling"></a>SharePoint trực tuyến throttling

**Quan trọng**: nhiều SharePoint trực tuyến và OneDrive khách hàng chạy ứng dụng kinh doanh quan trọng đối với các dịch vụ chạy trong nền. Chúng bao gồm di chuyển nội dung, ngăn chặn mất dữ liệu (DLP) và giải pháp sao lưu. Trong những lần chưa từng có, chúng tôi đang thực hiện các bước để đảm bảo rằng các dịch vụ SharePoint Online và OneDrive vẫn có hiệu quả cao và đáng tin cậy cho người dùng của bạn phụ thuộc vào dịch vụ hơn bao giờ hết trong các tình huống làm việc từ xa.

Để hỗ trợ cho mục tiêu này, chúng tôi đã thực hiện các giới hạn điều chỉnh chặt chẽ hơn trên các ứng dụng nền (di chuyển, DLP và các giải pháp sao lưu) trong giờ ban ngày trong tuần. Bạn nên mong đợi rằng các ứng dụng này sẽ đạt được thông lượng rất hạn chế trong những thời gian này. Tuy nhiên, trong giờ tối và cuối tuần cho khu vực, Dịch vụ sẽ sẵn sàng xử lý số lượng yêu cầu cao hơn đáng kể từ ứng dụng nền.

**503 Server là lỗi bận**

Người dùng có thể nhận được một máy chủ 503 bận lỗi khi cố gắng di chuyển trang web SharePoint hoặc OneDrive. 

Lỗi này có thể do điều chỉnh trong dịch vụ SharePoint. SharePoint Online sử dụng điều chỉnh để duy trì hiệu suất tối ưu và độ tin cậy của dịch vụ SharePoint trực tuyến. Điều tiết giới hạn số hành động của người dùng hoặc các cuộc gọi đồng thời (theo tập lệnh hoặc mã) để tránh sử dụng quá nhiều tài nguyên. 

Để biết thêm thông tin về điều chỉnh xem, [tránh bị điều chỉnh hoặc chặn trong SharePoint trực tuyến](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).

Nếu bạn tin rằng lỗi này không liên quan đến điều chỉnh, bạn có thể kiểm tra nếu có bảo trì hoạt động xảy ra trên thuê của bạn bằng cách điều hướng đến [Trung tâm thông báo](https://portal.office.com/adminportal/home#/MessageCenter).

 Cuối cùng, đảm bảo bạn truy cập vào trang [y tế Dịch vụ](https://portal.office.com/adminportal/home#/servicehealth) để kiểm tra bất kỳ tư vấn/sự cố nào có thể xảy ra.

