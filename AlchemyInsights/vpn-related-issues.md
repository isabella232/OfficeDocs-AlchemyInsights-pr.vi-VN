---
title: Các vấn đề liên quan đến VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 3c031725c92f5d7af7c0dd0c37ea34fecf4792c8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47726135"
---
# <a name="vpn-related-issues"></a>Các vấn đề liên quan đến VPN

Việc thực hiện thành công các kết nối VPN cho máy khách MDM tùy thuộc vào một hồ sơ đã triển khai phản ánh chính xác các yêu cầu của cơ sở hạ tầng VPN. Đối với các cài đặt phù hợp cho nền tảng máy khách mà bạn đang điều tra, hãy xem: 

[Thiết đặt thiết bị trong Windows 10 và Windows Holographic để thêm kết nối VPN bằng cách dùng InTune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Thêm các thiết đặt VPN trên các thiết bị iOS và iPadOS trong Microsoft InTune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Thiết đặt thiết bị Android để cấu hình VPN trong InTune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Thêm các thiết đặt VPN trên thiết bị macOS trong Microsoft InTune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Nếu hồ sơ VPN của bạn sử dụng xác thực dựa trên chứng chỉ, hãy đảm bảo rằng các hồ sơ chứng nhận chứng chỉ gốc và xác thực máy khách được nối kết với hồ sơ VPN được triển khai thành công.

**Các sự cố phổ biến**

**Tôi đã triển khai hồ sơ VPN vào một thiết bị. InTune Hiển thị rằng nó đã thành công, nhưng thiết bị không được kết nối với VPN.**

Trạng thái thành công nghĩa là InTune đã triển khai thành công hồ sơ như được cấu hình. Tuy nhiên, các cấu hình này có thể không khớp với mạng của bạn và/hoặc các yêu cầu xác thực. Xem lại Nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên máy chủ VPN và NPS/Radius) để biết thêm chi tiết về kết nối đã thử. Bạn có thể cần làm việc với nhóm cơ sở hạ tầng mạng của bạn hoặc nhà cung cấp VPN bên thứ ba, để thu thập và xem lại Nhật ký.

**Khi tôi cấu hình một VPN tùy chỉnh cho iOS, tính năng trên mỗi ứng dụng VPN không được tạo sẵn.**

VPN mỗi ứng dụng dành cho thiết bị iOS trong InTune hiện sẵn dùng cho một danh sách các nhà cung cấp và đối tác cụ thể, những người cũng phải đáp ứng các điều kiện tiên quyết chứng chỉ trước khi cấu hình VPN cho mỗi ứng dụng. Để biết thêm thông tin, hãy xem [thiết lập mạng riêng ảo trên mỗi ứng dụng (VPN) cho các thiết bị iOS/iPadOS trong InTune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Để biết thêm thông tin về tất cả các loại kết nối VPN trong InTune, hãy xem [tạo hồ sơ VPN để kết nối với các máy chủ VPN trong InTune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN on-Demand VPN không được kích hoạt khi tên miền được đặt cấu hình được truy nhập**

Để kiểm tra các thiết đặt VPN tự động, hãy đặt các giá trị sau đây:

Tôi muốn thực hiện các thao tác sau: **đánh giá mỗi lần thử kết nối** 

Chọn xem có kết nối không: **kết nối nếu cần thiết**

Khi người dùng truy nhập các tên miền này: *tên miền* **đích**

Nếu cấu hình trên không thành công, hãy thêm thành phần sau đây:

Khi URL này không thể truy cập, lực lượng kết nối VPN: **Badurl**