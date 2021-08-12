---
title: Đã xảy ra lỗi khi xác thực mã thông báo truy nhập trong khi đang bật Phân tích trên máy tính
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946637"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Lỗi "Đã xảy ra lỗi khi xác thực mã thông báo truy nhập" trong khi trình chiếu Phân tích Trên máy tính

Lỗi này thường xảy ra khi mã thông báo xác thực hết hạn. Thông thường, làm mới trang sẽ làm mới mã thông báo. Tuy nhiên, sự cố này có thể vẫn tiếp diễn nếu có bất kỳ chính sách truy nhập có điều kiện nào được áp dụng cho tài khoản đang được sử dụng để phân tích trên máy tính. Bạn có thể xem lại nhật ký Đăng nhập Azure AD trong Cổng thông tin Azure để xem liệu có bất kỳ lỗi đăng nhập nào đối với tài khoản đang được sử dụng cho việc tiếp nhận Phân tích Máy tính hay không.

Để biết thêm thông tin về Truy nhập có Điều kiện, hãy truy cập lập [kế hoạch triển khai Truy nhập có Điều kiện của bạn](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).