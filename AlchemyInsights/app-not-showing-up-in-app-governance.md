---
title: Ứng dụng của tôi không hiển thị trong Quản trị Ứng dụng
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12734"
ms.openlocfilehash: a8d176fdee073e41b61de6f53c728601da955aaa
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454985"
---
# <a name="my-app-isnt-showing-up-in-app-governance"></a>Ứng dụng của tôi không hiển thị trong Quản trị Ứng dụng

Nếu ứng dụng của bạn không hiển thị trong Quản trị Ứng dụng, hãy kiểm tra các mục sau:

1. Đi tới [Azure AD và](https://aad.portal.azure.com/) tìm ID ứng dụng cho ứng dụng của bạn bằng cách tìm kiếm tên ứng dụng ở thanh trên cùng trên trang Tổng quan.

1. Access Graph Explorer và tìm kiếm ID ứng dụng trong tên dịch vụ chính của bạn bằng cách dùng truy vấn này và thay thế bằng ID ứng dụng liên <appId> quan: < https://graph.microsoft.com/v1.0/servicePrincipals? $search= "appId: <appId> "thông >

1. Nếu không có kết quả nào được trả về, hãy tìm kiếm ID ứng dụng trong ứng dụng bằng cách sử dụng truy vấn này và thay thế bằng ID ứng dụng liên <appId> quan: < https://graph.microsoft.com/v1.0/applications? $search= "appId: <appId> ">

Nếu bạn gặp sự cố với truy vấn, hãy xem Nhận [hỗ trợ](https://docs.microsoft.com/microsoft-365/business-video/get-help-support). 

Để biết thêm thông tin hoặc thông tin chuyên sâu về các Ứng dụng trong Việc quản trị Ứng dụng, hãy xem [Tìm hiểu về khả năng hiển thị và thông tin chuyên sâu.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-overview)

Để biết thêm thông tin về cách xem các ứng dụng của bạn, hãy xem [Xem ứng dụng của bạn](https://docs.microsoft.com/microsoft-365/compliance/app-governance-visibility-insights-view-apps).
