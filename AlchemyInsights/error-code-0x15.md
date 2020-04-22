---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn gặp lỗi khi kích hoạt Office 2013 trên các triển khai dịch vụ máy tính để bàn từ xa (RDS), hãy xem xét cho phép ADAL bằng cách chỉnh sửa sổ đăng ký.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703160"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a>Lỗi khi kích hoạt Office 2013 trên máy tính để bàn từ xa dịch vụ

Nếu bạn gặp lỗi khi kích hoạt Office 2013 trên các triển khai dịch vụ máy tính để bàn từ xa (RDS), hãy xem xét cho phép ADAL bằng cách chỉnh sửa sổ đăng ký.
  
|**Khoá đăng ký**|**Loại**|**Đáng giá tiền**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |

Để biết thêm thông tin, xem [kích hoạt xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL được bật theo mặc định trong Microsoft 365 ứng dụng cho doanh nghiệp và Office 2016. Dịch vụ máy tính để bàn từ xa (RDS) trước đây có tên là dịch vụ đầu cuối.
  