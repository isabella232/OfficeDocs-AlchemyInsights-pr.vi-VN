---
title: Thay đổi từ máy chủ tên của Microsoft về việc quản lý bản ghi DNS của riêng bạn
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 09/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13988"
- "14"
ms.openlocfilehash: a228bcda1220011ab994de7aa70f19ea092e2142
ms.sourcegitcommit: e9e282be4997b0ee95f1ff4491e0943f8fc52444
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/22/2021
ms.locfileid: "59506978"
---
# <a name="changing-from-microsoft-nameservers-back-to-managing-your-own-dns-records"></a>Thay đổi từ máy chủ tên của Microsoft về việc quản lý bản ghi DNS của riêng bạn

Trước đây bạn đã thay đổi bản ghi NS để trỏ tới Microsoft (ns1.bdm.microsoftonline.com) nhưng bây giờ bạn đã quyết định quản lý bản ghi DNS của riêng mình:

Tại website của nhà đăng ký tên miền của bạn, hãy thay đổi máy chủ tên về thiết đặt trước đó hoặc nhà đăng ký tên miền của bạn. Nếu bạn không quen với DNS, hãy liên hệ với bộ phận hỗ trợ tại nhà đăng ký tên miền. Lưu ý rằng thay đổi máy chủ tên có thể cần tới 48 giờ để phát sinh. 

1. Trong cổng thông Microsoft 365 quản trị viên Của bạn, đi **đến Cài đặt** Domains , chọn hộp kiểm cạnh tên miền  >  [](https://admin.microsoft.com/Adminportal/Home#/Domains)đó và chọn Quản **lý DNS.** 

2. Trong trình hướng dẫn, chọn Thêm **bản ghi DNS của riêng bạn, rồi** hoàn tất trình hướng dẫn. Điều này thay đổi cách quản lý DNS của bạn và sau đó cho phép bạn thêm các bản ghi DNS tùy chỉnh cần thiết để hỗ trợ các dịch vụ đã chọn của bạn.

Ngoài ra, Nếu bạn đã thay đổi bản ghi máy chủ tên của mình thành Microsoft và có website, bạn có thể thêm bản ghi DNS cho website thay vì thay đổi lại các máy chủ tên. Để biết thêm thông tin, hãy xem [Cập nhật bản ghi DNS để duy trì website của bạn tại nhà cung cấp dịch vụ lưu trữ hiện tại của bạn.](https://docs.microsoft.com/microsoft-365/admin/dns/update-dns-records-to-retain-current-hosting-provider)


