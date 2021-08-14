---
title: Sự cố về chấp thuận của người quản trị
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004354"
- "7786"
ms.openlocfilehash: 08d3bfa84fd5ab31d7165090c392866d863898545ade7631e820a100eef89dea
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53952595"
---
# <a name="admin-consent-issues"></a>Sự cố về chấp thuận của người quản trị

1. Cho phép dòng [công việc chấp thuận của](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) người quản trị để cho phép người dùng yêu cầu phê duyệt trực tiếp từ màn hình chấp thuận.

1. Nếu bạn hoặc người dùng ứng dụng của bạn đang gặp lỗi ngoài dự kiến trong quá trình chấp thuận, hãy xem bài viết này để biết các bước khắc phục sự cố: Lỗi không mong muốn khi thực hiện đồng ý với [ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Tìm hiểu thêm về [sự chấp thuận](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)của người quản trị trên Nền tảng định danh Microsoft , cách hoạt động của lời nhắc chấp thuận cũng như cách đánh giá yêu cầu chấp thuận quản trị [toàn đối tượng thuê.](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) [](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent)

1. Các ứng dụng tích hợp với Nền tảng định danh Microsoft theo mô hình ủy quyền cho phép người dùng và người quản trị kiểm soát cách truy nhập dữ liệu. Việc triển khai mô hình ủy quyền đã được cập nhật trên điểm cuối Nền tảng định danh Microsoft và thay đổi cách thức một ứng dụng phải tương tác với cơ sở dữ Nền tảng định danh Microsoft. Hãy [xem Các quyền và sự chấp thuận trong Nền tảng định danh Microsoft cuối để](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) có cái nhìn tổng quan về mô hình ủy quyền này, bao gồm phạm vi, quyền và sự chấp thuận.