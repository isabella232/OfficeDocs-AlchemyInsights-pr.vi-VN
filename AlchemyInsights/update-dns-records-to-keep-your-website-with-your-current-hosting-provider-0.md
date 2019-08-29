---
title: Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện hành
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
ms.sourcegitcommit: b3e55405af384e868fcd32ea794eb15d1356c3fc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/29/2019
ms.locfileid: "36665782"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện hành

1. Trong Trung tâm quản trị Microsoft 365, đi đến **thiết lập** > [tên miền](https://portal.office.com/adminportal/home#/Domains) trang, và trong danh sách các tên miền, chọn tên miền bạn đang sử dụng cho trang web của bạn.

2. Chọn **+ ghi tùy chỉnh mới** và nhập thông tin sau:

  - **DNS** loại nhập: **(địa chỉ)**

  - Đối với **tên máy chủ hoặc bí danh**, gõ như sau:**@**

  - Đối với **Địa chỉ IP**, gõ địa chỉ IP tĩnh cho trang web của bạn nơi mà nó hiện đang được tổ chức (ví dụ, 172.16.140.1).

    Điều này phải có một địa chỉ IP *tĩnh* cho trang web, không phải là một địa chỉ IP *động* . Kiểm tra với các trang web mà trang web của bạn được lưu trữ để đảm bảo rằng bạn có thể nhận được một địa chỉ IP tĩnh cho trang web công cộng của bạn.

3. Chọn **lưu**.

Ngoài ra, bạn có thể tạo bản ghi CNAME để giúp khách hàng tìm thấy trang web của bạn.
  
1. Chọn **+ ghi tùy chỉnh mới** và nhập thông tin sau:

  - **DNS** loại nhập: **CNAME (bí danh)**

  - Đối với **tên máy chủ hoặc bí danh**, gõ như sau: **www**

  - Cho **điểm đến địa chỉ**, hãy nhập tên miền đủ điều kiện (FQDN) cho trang web của bạn (ví dụ: contoso.com).

2. Chọn **lưu**.
