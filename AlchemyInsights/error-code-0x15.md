---
title: Mã lỗi 0x15
ms.author: pebaum
author: pebaum
ms.date: 10/31/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry.
ms.openlocfilehash: 89f9270169e13fd7706f7826c624ef8ae4d47b3f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/15/2019
ms.locfileid: "28320647"
---
Nếu bạn nhận được một lỗi trong khi kích hoạt Office 2013 trên dịch vụ máy tính để bàn từ xa (RDS) triển khai, hãy xem xét cho phép ADAL bằng cách chỉnh sửa registry. 
  
|**Khóa sổ đăng ký**|**Nhập **|**Giá trị**|
|:-----|:-----|:-----|
|HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL  <br/> |REG_DWORD  <br/> |1  <br/> |
   
Để biết thêm chi tiết, hãy xem [Sử xác thực hiện đại cho Office 2013 trên thiết bị Windows](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).
  
> [!NOTE]
>  ADAL được kích hoạt theo mặc định trong Office 365 ProPlus và Office 2016. > Dịch vụ từ xa máy tính để bàn (RDS) trước đây được đặt tên là dịch vụ đầu cuối. 
  

