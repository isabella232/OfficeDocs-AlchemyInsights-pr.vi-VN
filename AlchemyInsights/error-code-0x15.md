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
ms.openlocfilehash: ed3770c001461c162ff5bbe24dc400a29380a03b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58316708"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Lỗi trong khi kích Office 2013 trên Dịch vụ Máy tính Từ xa

Nếu bạn đang nhận được lỗi trong khi kích hoạt Office 2013 trên triển khai Dịch vụ Máy tính Từ xa (RDS), hãy cân nhắc việc bật ADAL bằng cách chỉnh sửa sổ đăng ký.
  
|**Khóa đăng ký**|**Nhập**|**Giá trị**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Để biết thêm thông tin, [hãy xem mục Bật Xác thực Hiện đại Office 2013 trên các Windows khác.](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)
  
**Lưu** ý : ADAL được bật theo mặc định Ứng dụng Microsoft 365 dành cho doanh nghiệp lớn và Office 2016. Dịch vụ Máy tính Từ xa (RDS) trước đây được đặt tên là Terminal Services.
  