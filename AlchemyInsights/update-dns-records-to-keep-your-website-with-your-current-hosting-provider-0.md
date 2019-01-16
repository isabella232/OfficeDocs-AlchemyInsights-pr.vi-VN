---
title: Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện hành
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 48251355-7383-4fdc-a1e1-9dc2c85a8d29
ms.openlocfilehash: a79302259e294ea5bf3b1d29393a412edb27a388
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320502"
---
# <a name="update-dns-records-to-keep-your-website-with-your-current-hosting-provider"></a>Cập Nhật bản ghi DNS để giữ cho trang web của bạn với nhà cung cấp lưu trữ hiện hành

1. Trên trang [miền](https://portal.office.com/adminportal/home#/Domains) , trong danh sách các tên miền, chọn tên miền bạn đang sử dụng cho trang web của bạn, và sau đó chọn **cài đặt DNS** trong cửa sổ quản lý. 
    
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
    

