---
title: Cấu hình điểm kết nối dịch vụ (SCP)
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9732"
- "9003244"
ms.openlocfilehash: 9d733a1a0a3b8d92bdd5477a8978b6fbeede9653
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/19/2021
ms.locfileid: "51037294"
---
# <a name="configure-service-connection-point-scp"></a>Cấu hình điểm kết nối dịch vụ (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Lý do**: không thể đọc được đối tượng SCP và nhận được thông tin về người thuê Azure AD
- **Giải** Pháp: tham khảo phần [cấu hình điểm kết nối dịch vụ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Kế hoạch hành động**

- Kiểm tra xem thiết bị đã nhận được GPO để xác thực được kiểm soát hay không.
- Đảm bảo rằng GPO đã tạo khóa đăng ký.
- Đảm bảo rằng bạn có 2 phím được tạo bằng ID thư mục và tên miền onmicrosoft của bạn.

**Cấu hình thiết đặt sổ đăng ký phía máy khách cho SCP**

Dùng ví dụ sau đây để tạo một đối tượng chính sách Nhóm (GPO) để triển khai thiết đặt sổ đăng ký cấu hình một mục nhập SCP trong sổ đăng ký thiết bị của bạn.

1. Mở bảng điều khiển quản lý chính sách nhóm và tạo một GPO mới trong tên miền của bạn.
     - Cung cấp một tên mới được tạo là GPO của bạn (ví dụ: ClientSideSCP)

2. Sửa GPO và định vị đường dẫn sau đây: **cấu hình máy tính > tùy chọn > thiết đặt Windows > sổ đăng ký**.

3. Bấm chuột phải vào **sổ đăng ký** và chọn **> mục đăng ký mới**.

4. Trên tab **chung** , hãy cấu hình các mục sau:
  
- **Hành động**: Cập Nhật
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Đường dẫn chính**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Giá trị tên**: tenantid
    
- **Loại giá trị**: REG_SZ
    
- **Dữ liệu giá trị**: GUID hoặc ID thư mục của mẫu Azure AD của bạn (giá trị này có thể được tìm thấy trong **Azure Portal > azure Active Directory > thuộc tính > ID thư mục**)
 
- Bấm **OK**.
 
5. Bấm chuột phải vào **sổ đăng ký** và chọn **> mục đăng ký mới**.

6. Trên tab **chung** , hãy cấu hình các mục sau:
  
- **Hành động**: Cập Nhật
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Đường dẫn chính**: Software\microsoft\windows\currentversion\cdj\aad
    
- **Giá trị tên**: tenantname
    
- **Loại giá trị**: REG_SZ
    
- **Dữ liệu giá trị**: tên miền đã xác nhận nếu bạn đang sử dụng môi trường liên kết chẳng hạn như AD FS. Tên miền đã xác nhận của bạn hoặc tên miền onmicrosoft.com của bạn (ví dụ: contoso. onmicrosoft). com nếu bạn đang sử dụng môi trường được quản lý

- Bấm **OK**.

7. Đóng trình soạn thảo cho GPO mới được tạo.

8. Nối kết các máy tính có thể tham gia vào trình phát triển tên miền của bạn.

Để biết thêm thông tin, hãy xem kiểm soát xác thực của kết hợp kết nối [AZURE AD-AZURE AD | ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) Tài liệu Microsoft và  [khắc phục sự cố kết hợp Azure Active Directory đã tham gia thiết bị | ](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current)Tài liệu Microsoft.









