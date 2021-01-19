---
title: Sự đồng ý của người quản trị vấn đề
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
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901517"
---
# <a name="admin-consent-issues"></a>Sự đồng ý của người quản trị vấn đề

1. Bật dòng công việc [chấp thuận quản trị](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) để cho phép người dùng yêu cầu phê duyệt người quản trị trực tiếp từ màn hình chấp thuận.

1. Nếu bạn hoặc người dùng ứng dụng của bạn đang gặp phải lỗi không mong muốn trong quá trình chấp thuận, hãy xem bài viết này để biết các bước khắc phục sự cố: [lỗi không mong muốn khi thực hiện việc đồng ý với một ứng dụng](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).

1. Tìm hiểu thêm về [sự đồng ý của người quản trị trên nền tảng Microsoft Identity](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), cách [đồng ý nhắc](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) công việc và cách [đánh giá yêu cầu cho sự đồng ý của người quản trị đối tượng thuê](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).

1. Các ứng dụng tích hợp với nền tảng định danh Microsoft theo dõi một mô hình ủy quyền cung cấp cho người dùng và người quản trị kiểm soát dữ liệu có thể truy nhập như thế nào. Việc thực hiện mô hình ủy quyền đã được Cập Nhật trên điểm cuối Microsoft Identity Platform và thay đổi cách ứng dụng phải tương tác với nền tảng định danh Microsoft. Xem [các quyền và sự đồng ý trong điểm cuối Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) để biết tổng quan về mô hình ủy quyền này, bao gồm phạm vi, quyền và đồng ý.