---
title: Không thể kích hoạt Office
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
ms.openlocfilehash: 9771a3244c5507312d43156525095fb9eaf7fa20
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51812594"
---
# <a name="unable-to-activate-office"></a>Không thể kích hoạt Office

- Kiểm tra xem trạng thái đăng ký của bạn đã hết hạn chưa.
- Đảm bảo bạn có thuê bao cho phép các giấy phép máy khách, chẳng hạn như Office 365 Business hoặc Business Premium và [đảm bảo người dùng có giấy phép được gán](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).
- Đảm bảo người dùng đăng nhập vào Office bằng cùng tài khoản có giấy phép được gán.
- Hãy kiểm tra trang trạng thái [dịch vụ của Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) để xem liệu có bất kỳ vấn đề nào đã biết với dịch vụ hay không.
- Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy để xác nhận rằng họ không ngăn chặn việc truy nhập ứng dụng Microsoft 365 vào Internet. Vui lòng xem các [URL của Office 365 và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL và dải địa chỉ IP của Office 365").

**Mẹo** Trên máy Windows, chúng tôi có thể chẩn đoán và tự động khắc phục một số vấn đề đăng nhập Office thông thường cho bạn. Tải xuống và chạy trình trợ  **[giúp phục hồi và hỗ trợ của Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** để sử dụng công cụ tự động của chúng tôi.

Sử dụng các hành động khắc phục sự cố sau đây:

- Mở một ứng dụng Office và [đăng xuất khỏi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) bất kỳ tài khoản người dùng hiện có nào. [Loại bỏ](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) và [gán lại](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) giấy phép Office, sau đó [đăng nhập vào Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) bằng tài khoản người dùng bị ảnh hưởng.
- Chạy trình khắc phục sự cố [kích hoạt](https://aka.ms/SARA-OfficeActivation-Alchemy)
- [Đặt lại trạng thái kích hoạt Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Đặt lại trạng thái kích hoạt Office")
- [Thực hiện sửa chữa trực tuyến của Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

Để biết thêm giải pháp khắc phục sự cố, hãy xem:  

- [Lỗi sản phẩm chưa được cấp phép và kích hoạt trong Office](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- ["Rất tiếc, chúng tôi không thể kết nối với tài khoản của bạn. Xin vui lòng thử lại sau "lỗi" khi bạn kích hoạt Office](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)