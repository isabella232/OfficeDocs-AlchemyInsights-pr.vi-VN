---
title: Khắc phục sự cố kết hợp kết nối Azure AD
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
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401929"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a>Khắc phục sự cố kết hợp kết nối Azure AD

Rất khuyên bạn nên đảm bảo rằng một thiết bị có thể truy nhập các điểm cuối đăng ký thiết bị bên dưới tài khoản hệ thống bằng cách sử dụng [script kết nối đăng ký thiết bị kiểm tra](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).

1. Nếu bạn đang thiết lập đăng ký thiết bị lần đầu tiên, hãy đảm bảo bạn xem lại tính[năng quản lý thiết bị trong Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) để tìm hiểu cách tải các thiết bị dưới phần điều khiển của Azure AD.
1. Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và đăng ký chúng vào InTune, hãy đảm bảo rằng bạn đã [cấu hình InTune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) và có [cấp phép](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) tại chỗ trước.
1. Đảm bảo rằng bạn được phép thực hiện các hoạt động trong Azure AD và quảng cáo tại cơ sở. Chỉ có một người quản trị toàn cầu trong Azure AD có thể quản lý thiết đặt cho việc đăng ký thiết bị. Ngoài ra, nếu bạn đang thiết lập đăng ký tự động trong Active Directory tại chỗ của bạn, bạn sẽ cần phải là người quản trị của Active Directory và AD FS (nếu có).

Để biết thêm chi tiết về cách giải quyết các vấn đề có thể xảy ra với nối kết, hãy xem [khắc phục sự cố gia nhập](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) kết hợp để thiết lập kết hợp Azure và quản lý các thiết bị bằng cách sử dụng cổng thông tin Azure AD, hãy xem [thiết lập kết hợp Azure AD đã tham gia (tại chỗ) thiết bị](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) và [quản lý các thiết bị bằng Azure Portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).

Để giải quyết các sự cố phổ biến với kết hợp Azure Azure Active Directory (AD), hãy xem [câu hỏi thường gặp về gia nhập AZURE AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).
