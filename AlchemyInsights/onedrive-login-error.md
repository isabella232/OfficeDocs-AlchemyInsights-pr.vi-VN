---
title: OneDrive đăng nhập AADSTS50011
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
ms.openlocfilehash: 80aafa2aee7213e1b77d274509a7eb9741c20b525ed97f473093ac8c6514f3c7
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54112934"
---
# <a name="onedrive-login-error-aadsts50011"></a>OneDrive đăng nhập AADSTS50011

Nếu bạn nhận được lỗi "AADSTS50011: URL trả lời được chỉ định trong yêu cầu không khớp với trả lời" khi đăng nhập vào ứng dụng OneDrive, hãy kiểm tra như sau:

Phiên OneDrive của bạn cần phải bằng hoặc lớn hơn phiên bản 20.052.XXXX.XXXX. Để kiểm tra phiên bản của bạn, hãy bấm vào biểu OneDrive màu lam trong khu vực thông báo, chọn **Trợ giúp & Cài đặt > Cài đặt > Giới thiệu**.

Mạng của bạn có thể chặn lưu lượng truy **cập g.live.com** **và oneclient.sfx.ms.** Nếu lưu lượng đó bị chặn, bạn OneDrive thể tự cập nhật. Làm việc với người quản trị mạng của bạn để đảm bảo rằng bạn có quyền truy nhập vào các URL đó. [Các điểm cuối này phải có](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) thể tiếp cận được đối với các khách hàng sử dụng Microsoft 365 của mình.

Nếu bạn cần tải thủ công phiên bản hiện tại của OneDrive, hãy truy cập [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .
