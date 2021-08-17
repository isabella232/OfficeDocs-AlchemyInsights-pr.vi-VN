---
title: Không thể kích hoạt các Office
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: eb62dfce9f9507dd8806d91343cd39fe76e65594473683c1393d524f6c2d8a27
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/11/2021
ms.locfileid: "57893933"
---
# <a name="unable-to-activate-office"></a>Không thể kích hoạt các Office

**Lưu** ý: Nếu bạn đang sử dụng phiên bản cũ hơn của Windows (Ví dụ: Windows 7), hãy đảm bảo rằng TLS 1.2 được bật làm mặc định. Để biết thêm thông tin, hãy xem Cập nhật để bật [TLS 1.1 và TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)làm giao thức bảo mật mặc định trong WinHTTP trong Windows.

- Kiểm tra xem trạng thái đăng ký của bạn đã hết hạn chưa.
- Đảm bảo bạn có đăng ký cho phép giấy phép máy khách, chẳng hạn như Office 365 Business hoặc Business Premium và đảm bảo người dùng có [giấy phép được gán.](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users)
- Đảm bảo người dùng đăng nhập vào Office với chính tài khoản đã được gán giấy phép.
- Hãy kiểm tra [Office 365 Trạng tác Dịch vụ Để](https://docs.microsoft.com/office365/enterprise/view-service-health) xem liệu có bất kỳ sự cố đã biết nào với dịch vụ này không.
- Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy của bạn để xác nhận rằng họ không chặn những Microsoft 365 truy nhập vào internet của bạn. Vui lòng [xem Office 365 URL và dải địa chỉ IP mới.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL và dải địa chỉ IP")

**Mẹo** Trên Windows tính, chúng tôi có thể chẩn đoán và tự động khắc phục một số sự cố Office đăng nhập thường gặp cho bạn. Tải xuống và chạy Microsoft Công cụ Trợ giúp Phục hồi và Hỗ trợ **[cách sử dụng](https://aka.ms/SaRA-OfficeSignInScenario)** công cụ tự động của chúng tôi.

Sử dụng các hành động khắc phục sự cố sau đây:

- Mở một tài Ứng dụng Office và đăng xuất [khỏi mọi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) tài khoản người dùng hiện có. [Loại](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) bỏ [và gán lại giấy](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office, rồi đăng nhập vào tài [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sử dụng tài khoản người dùng bị ảnh hưởng.
- Chạy Trình khắc phục [sự cố Kích hoạt](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Đặt lại Office thái kích hoạt](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Đặt lại Office thái kích hoạt")
- [Thực hiện Sửa chữa Trực tuyến Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Để biết thêm các giải pháp khắc phục sự cố, hãy xem:  

- [Lỗi Sản phẩm Chưa được cấp phép và kích hoạt trong Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["Rất tiếc, chúng tôi không thể kết nối với tài khoản của bạn. Vui lòng thử lại sau" khi bạn kích hoạt Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)