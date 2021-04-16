---
title: Đã xảy ra lỗi khi xác nhận lỗi mã truy nhập trong khi phân tích máy tính tại chỗ
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
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813710"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Lỗi "đã xảy ra lỗi khi xác nhận mã truy nhập" trong khi phân tích máy tính để bàn triển khai

Lỗi này thường được quan sát thấy khi mã xác thực hết hạn. Thông thường, làm mới trang sẽ làm mới mã thông báo. Tuy nhiên, sự cố này có thể tồn tại nếu có bất kỳ chính sách truy nhập có điều kiện nào được áp dụng cho tài khoản đang được sử dụng để phân tích trên máy tính bảng. Bạn có thể xem lại đăng nhập Azure AD trong các Nhật ký trong cổng thông tin Azure để xem liệu có bất kỳ lỗi đăng nhập nào cho tài khoản đang được sử dụng cho máy tính để bàn onboarding không.

Để biết thêm thông tin về truy nhập có điều kiện, hãy truy cập [lên kế hoạch triển khai truy nhập](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)có điều kiện.