---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn nhận được lỗi trong khi kích hoạt Office 2013 về triển khai dịch vụ trên máy tính từ xa (RDS), hãy cân nhắc việc bật ADAL bằng cách chỉnh sửa sổ đăng ký.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709209"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Lỗi trong khi kích hoạt Office 2013 trên máy tính từ xa dịch vụ

Nếu bạn nhận được lỗi trong khi kích hoạt Office 2013 về triển khai dịch vụ trên máy tính từ xa (RDS), hãy cân nhắc việc bật ADAL bằng cách chỉnh sửa sổ đăng ký.
  
|**Khóa sổ đăng ký**|**Kiểu**|**Đáng**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Để biết thêm thông tin, hãy xem [bật xác thực hiện đại cho Office 2013 trên các thiết bị chạy Windows](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL được bật theo mặc định trong các ứng dụng Microsoft 365 dành cho doanh nghiệp và Office 2016. Dịch vụ trên máy tính từ xa (RDS) trước đây đã có tên là dịch vụ Terminal.
  