---
title: Các vấn đề liên quan đến VPN
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1545"
- "9000076"
ms.openlocfilehash: 134d78f30216dfd268c5999a5032b7d7ad1d7dd8
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555740"
---
# <a name="vpn-related-issues"></a>Các vấn đề liên quan đến VPN

Thực hiện thành công kết nối VPN cho khách hàng MDM phụ thuộc vào hồ sơ triển khai đúng phản ánh các yêu cầu của cơ sở hạ tầng VPN. Đối với các thiết đặt thích hợp cho các nền tảng máy khách mà bạn đang điều tra, hãy xem: 

[Cài đặt thiết bị Windows 10 và Windows Holographic để thêm các kết nối VPN bằng InTune](https://docs.microsoft.com/intune/vpn-settings-windows-10)  
[Thêm cài đặt VPN trên các thiết bị iOS và iPadOS trong Microsoft InTune](https://docs.microsoft.com/intune/vpn-settings-ios)  
[Cài đặt thiết bị Android để cấu hình VPN trong InTune](https://docs.microsoft.com/intune/vpn-settings-android)  
[Thêm cài đặt VPN trên các thiết bị macOS trong Microsoft InTune](https://docs.microsoft.com/mem/intune/configuration/vpn-settings-macos)

Nếu cấu hình VPN của bạn sử dụng xác thực dựa trên chứng chỉ, hãy đảm bảo rằng chứng chỉ gốc và hồ sơ chứng chỉ xác thực máy khách được liên kết đến cấu hình VPN đang triển khai thành công.

**Các vấn đề thường gặp**

**Tôi đã triển khai một cấu hình VPN đến một thiết bị. InTune Hiển thị rằng nó đã thành công, nhưng thiết bị không kết nối với VPN.**

Trạng thái thành công có nghĩa là InTune đã triển khai thành công hồ sơ dưới dạng cấu hình. Tuy nhiên, các cấu hình có thể không phù hợp với mạng của bạn và/hoặc yêu cầu xác thực. Đánh giá Nhật ký trong cơ sở hạ tầng và dịch vụ xác thực (trên máy chủ VPN và máy chủ NPS/Radius) để biết thêm chi tiết về kết nối cố gắng. Bạn có thể cần phải làm việc với nhóm cơ sở hạ tầng mạng của mình hoặc nhà cung cấp VPN bên thứ ba để thu thập và đánh giá các bản ghi.

**Khi tôi đặt cấu hình VPN tùy chỉnh cho iOS, tính năng VPN cho mỗi ứng dụng không có sẵn.**

Mỗi ứng dụng VPN cho các thiết bị iOS trong InTune hiện có sẵn cho một danh sách cụ thể của các nhà cung cấp và đối tác, những người cũng phải đáp ứng các điều kiện tiên quyết của chứng chỉ trước khi cấu hình một VPN cho mỗi ứng dụng. Để biết thêm thông tin, xem [thiết lập một ứng dụng Virtual Private Network (VPN) cho các thiết bị iOS/iPadOS trong InTune](https://docs.microsoft.com/intune/vpn-setting-configure-per-app). 

Để biết thêm thông tin về tất cả các loại kết nối VPN trong InTune, xem [tạo cấu hình VPN để kết nối với các máy chủ VPN trong InTune](https://docs.microsoft.com/intune/vpn-settings-configure).  

**VPN theo yêu cầu iOS không kích hoạt khi truy cập một miền được cấu hình**

Để kiểm tra cài đặt VPN tự động, hãy đặt các giá trị sau:

Tôi muốn làm như sau: đánh **giá từng nỗ lực kết nối** 

Chọn có kết nối hay không: **kết nối nếu cần**

Khi người dùng truy cập vào các miền này: *tên miền* **đích**

Nếu cấu hình trên không thành công, thêm các yếu tố sau:

Khi URL này không thể truy cập, buộc kết nối VPN: **Badurl**