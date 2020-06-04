---
title: Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện tại
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "42"
- "43"
- "100002"
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: 7bd36c3954d12d3ee4ac624a2f827d8e5cd88082
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665782"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện tại

1. Trong Trung tâm quản trị Microsoft 365, hãy đi tới trang **thiết lập**  >  [miền](https://portal.office.com/adminportal/home#/Domains) và trong danh sách tên miền, chọn miền bạn đang sử dụng cho trang web của mình.

2. Chọn **+ bản ghi tùy chỉnh mới** và nhập các mục sau:

  - Đối với **loại DNS** nhập: **A (địa chỉ)**

  - **Tên máy chủ hoặc bí danh**, gõ như sau:**@**

  - Đối với **địa chỉ IP**, nhập địa chỉ IP tĩnh cho trang web của bạn nơi hiện đang lưu trữ (ví dụ: 172.16.140.1).

    Điều này phải là một địa chỉ IP *tĩnh* cho các trang web, không một địa chỉ IP *động* . Kiểm tra với trang web nơi trang web của bạn được lưu trữ để đảm bảo bạn có thể nhận được một địa chỉ IP tĩnh cho trang web công cộng của bạn.

3. Chọn **lưu**.

Ngoài ra, bạn có thể tạo bản ghi CNAME để giúp khách hàng tìm thấy trang web của bạn.
  
1. Chọn **+ bản ghi tùy chỉnh mới** và nhập các mục sau:

  - Đối với **loại DNS** nhập: **CNAME (alias)**

  - **Tên máy chủ hoặc bí danh**, gõ như sau: **www**

  - Đối **với điểm đến địa chỉ**, nhập tên miền đủ điều kiện (FQDN) cho trang web của bạn (ví dụ: contoso.com).

2. Chọn **lưu**.
