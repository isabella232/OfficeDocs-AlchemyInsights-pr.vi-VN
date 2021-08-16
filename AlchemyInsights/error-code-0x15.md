---
title: Trình xác định 0x15
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
description: Nếu bạn đang nhận được lỗi trong khi kích hoạt Office 2013 trên triển khai Dịch vụ Máy tính Từ xa (RDS), hãy cân nhắc việc bật ADAL bằng cách chỉnh sửa sổ đăng ký.
ms.openlocfilehash: 247686bf26c11d07ed118bdb1ba190fc718e87cf140b88f79b8aa0b40c827b4d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54100784"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Lỗi trong khi kích Office 2013 trên Dịch vụ Máy tính Từ xa

Nếu bạn đang nhận được lỗi trong khi kích hoạt Office 2013 trên triển khai Dịch vụ Máy tính Từ xa (RDS), hãy cân nhắc việc bật ADAL bằng cách chỉnh sửa sổ đăng ký.
  
|**Khóa đăng ký**|**Nhập**|**Giá trị**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Để biết thêm thông tin, [hãy xem mục Bật Xác thực Hiện đại cho Office 2013 trên Windows cụ thể.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
> [!NOTE]
>  ADAL được bật theo mặc định trong Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn và Office 2016. Dịch vụ Máy tính Từ xa (RDS) trước đây được đặt tên là Terminal Services.
  