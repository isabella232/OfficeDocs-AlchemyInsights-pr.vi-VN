---
title: Cập nhật bản ghi DNS để tiếp tục lưu trữ website tại nhà cung cấp lưu trữ hiện tại của bạn
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: f868ce25d68f61da30d2db4de88aa83675c97857b3c1371cf2039e0b03895a64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007704"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Cập nhật bản ghi DNS để tiếp tục lưu trữ website tại nhà cung cấp lưu trữ hiện tại của bạn

1. Trong hộp Trung tâm quản trị Microsoft 365, hãy đến trang Thiết lập Tên miền và trong danh sách tên miền, hãy chọn tên miền mà bạn đang dùng cho  >  [](https://admin.microsoft.com/Adminportal#/Domains) website của bạn.

2. Chọn **+ Bản ghi tùy chỉnh mới,** rồi nhập các mục sau:

  - Đối **với Loại DNS,** nhập: **A (Địa chỉ)**

  - Đối **với Tên máy chủ hoặc Biệt danh**, hãy nhập như sau: **@**

  - Đối **với Địa chỉ IP,** nhập địa chỉ IP tĩnh nơi hiện đang lưu trữ website của bạn (ví dụ: 172.16.140.1).

    Đây phải là một tĩnh  *cho*  website, không phải một  *địa chỉ*  IP động. Hãy kiểm tra với site lưu trữ website của bạn để đảm bảo rằng bạn có thể lấy địa chỉ IP tĩnh cho website công cộng của bạn.

3. Chọn **Lưu**.

Ngoài ra, bạn có thể tạo bản ghi CNAME để giúp khách hàng tìm thấy website của bạn.
  
1. Chọn **+ Bản ghi tùy chỉnh mới,** rồi nhập các mục sau:

  - Đối **với Loại DNS,** hãy nhập: **CNAME (Biệt danh)**

  - Đối **với Tên máy chủ hoặc Biệt danh**, nhập như sau: **www**

  - Đối **với Points to Address**, hãy nhập tên miền đủ điều kiện (FQDN) cho website của bạn (ví dụ, contoso.com).

2. Chọn **Lưu**.
