---
title: Lỗi đăng nhập OneDrive AADSTS50011
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982551"
---
# <a name="onedrive-login-error-aadsts50011"></a>Lỗi đăng nhập OneDrive AADSTS50011

Nếu bạn nhận được lỗi "AADSTS50011: URL trả lời được xác định trong yêu cầu không khớp trả lời" khi đăng nhập vào ứng dụng OneDrive, hãy kiểm tra các mục sau:

Phiên bản OneDrive của bạn cần bằng hoặc lớn hơn phiên bản 20.052. XXXX. XXXX. Để kiểm tra phiên bản của bạn, hãy bấm vào biểu tượng OneDrive màu lam trong khu vực thông báo, chọn **Trợ giúp & thiết đặt > thiết đặt > giới thiệu về**.

Mạng của bạn có thể chặn lưu lượng đến **g.Live.com** và **oneclient.SFX.MS**. Nếu lưu lượng đó bị chặn, OneDrive không thể cập nhật chính nó. Làm việc với người quản trị mạng của bạn để đảm bảo bạn có quyền truy nhập vào những URL đó. [Những điểm cuối này](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) sẽ có thể truy cập đối với khách hàng bằng cách sử dụng các gói Microsoft 365.

Nếu bạn cần lấy phiên bản hiện tại của OneDrive, hãy truy nhập [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
