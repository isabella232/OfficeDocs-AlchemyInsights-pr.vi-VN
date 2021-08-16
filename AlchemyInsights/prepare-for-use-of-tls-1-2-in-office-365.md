---
title: Chuẩn bị cho việc sử dụng TLS 1.2 trong Microsoft 365
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Critical
ms.custom:
- "1266"
- "1600052"
ms.assetid: d5c84f5c-a3ca-4abd-8633-7e9ff01328a9
ms.openlocfilehash: 79a9dc3833f8329adeb24d27014d08c14eb93d1f5f840c5cfa2ce10991107b1c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54040420"
---
# <a name="prepare-for-use-of-tls-12-in-microsoft-365"></a>Chuẩn bị cho việc sử dụng TLS 1.2 trong Microsoft 365

Vào 31/10/2018, Microsoft 365 sẽ tiếp tục chuyển sang TLS 1.2. Bắt đầu từ ngày 15 tháng 10 năm 2020, O365 sẽ bắt đầu việc bỏ dùng TLS 1.0 và 1.1 trên toàn dịch vụ. Việc triển khai thay đổi này sẽ tiếp tục trong vài tuần và tháng tiếp theo, nhưng khách hàng nên giả định không có cuộc gọi TLS 1.0/1.1 nào hoạt động khi tham gia với O365 bắt đầu từ ngày 15 tháng 10 năm 2020. Như đã liên lạc trước đó (MC126199 vào Tháng Mười Hai 2017, MC128929 vào Tháng Hai 2018, MC186827 vào Tháng Bảy 2019 và MC218794 vào Tháng Bảy 2020), chúng tôi đang chuyển tất cả các dịch vụ trực tuyến của mình sang Transport Layer Security (TLS) 1.2+ để cung cấp mã hóa cao cấp nhất và đảm bảo dịch vụ của chúng tôi được bảo mật hơn theo mặc định. Khách hàng vẫn có thể chọn có TLS 1.0/1.1 trên máy chủ và tài nguyên của mình nhưng họ nên giả định chỉ TLS 1.2 trở lên sẽ hoạt động khi tương tác với các tài nguyên O365.
  
Để tìm hiểu thêm về những thay đổi này, vui lòng xem [tại đây](https://docs.microsoft.com/microsoft-365/compliance/prepare-tls-1.2-in-office-365?view=o365-worldwide) và [tại đây.](https://docs.microsoft.com/microsoft-365/compliance/tls-1.0-and-1.1-deprecation-for-office-365?view=o365-worldwide)

  