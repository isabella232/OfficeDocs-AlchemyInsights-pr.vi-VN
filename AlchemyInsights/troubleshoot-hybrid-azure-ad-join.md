---
title: Khắc phục sự cố kết hợp Azure AD kết hợp
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 23da360965a5972e328844d505698c91ece61788240d8fdb8909fff3a7ef0d7f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53939293"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Khắc phục sự cố kết hợp Azure AD kết hợp

Đề xuất cao Hãy đảm bảo rằng thiết bị có thể truy nhập các điểm cuối Đăng ký Thiết bị dưới tài khoản hệ thống bằng cách sử dụng tập lệnh Kiểm tra Khả năng kết nối [Đăng ký Thiết bị.](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/)

1. Nếu bạn đang thiết lập đăng ký thiết bị lần đầu tiên, hãy đảm bảo xem lại giới thiệu của tôi về quản lý thiết bị trong[Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) để tìm hiểu cách nhận thiết bị dưới quyền kiểm soát của Azure AD.
1. Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và đăng ký thiết [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) bị vào Intune, hãy đảm bảo rằng bạn đã đặt cấu hình [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) và được cấp phép trước tiên.
1. Đảm bảo rằng bạn được phép thực hiện các thao tác trong Azure AD và AD tại chỗ. Chỉ người quản trị toàn cầu trong Azure AD mới có thể quản lý cài đặt cho đăng ký thiết bị. Ngoài ra, nếu bạn đang thiết lập đăng ký tự động trong Active Directory tại chỗ, bạn sẽ cần phải là người quản trị của Active Directory và AD FS (nếu có).

Để biết thêm chi tiết về [](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) cách giải quyết các vấn đề tiềm ẩn với kết hợp kết hợp, hãy xem Khắc phục sự cố Kết hợp Kết hợp để thiết lập kết hợp Azure AD và Quản lý thiết bị bằng cổng thông tin [Azure Ad,](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) hãy xem Thiết lập kết hợp Azure AD kết hợp (liên kết với tên miền tại cơ sở) và Quản lý thiết bị bằng cổng thông [tin Azure](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Để giải quyết các sự cố phổ biến với liên kết Azure Active Directory kết hợp (AD), hãy xem Câu hỏi thường gặp về kết hợp Azure AD kết [hợp.](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq)
