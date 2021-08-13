---
title: Cấu hình Điểm Kết nối Dịch vụ (SCP)
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
ms.openlocfilehash: 5ccb55996ccef4b55c8d80de6e35f4ba27e3dfa18dfcaeaf6f6ad1c54b6bb376
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53965987"
---
# <a name="configure-service-connection-point-scp"></a>Đặt cấu hình Điểm kết nối dịch vụ (SCP)

**DSREG_AUTOJOIN_ADCONFIG_READ_FAILED (0x801c001d/-2145648611)**

- **Lý** do: Không thể đọc đối tượng SCP và nhận thông tin đối tượng thuê Azure AD
- **Giải pháp**: Tham khảo phần Đặt [cấu hình điểm kết nối dịch vụ](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-federated-domains#configure-hybrid-azure-ad-join)


**Kế hoạch hành động**

- Kiểm tra xem thiết bị đã nhận được GPO để xác thực có được kiểm soát hay không.
- Đảm bảo rằng GPO đã tạo khóa đăng ký.
- Đảm bảo rằng bạn đã tạo 2 khóa bằng ID Thư mục và miền onmicrosoft.

**Cấu hình thiết đặt sổ đăng ký phía máy khách cho SCP**

Sử dụng ví dụ sau đây để tạo Đối tượng Chính sách Nhóm (GPO) để triển khai thiết đặt sổ đăng ký đặt cấu hình một mục nhập SCP trong sổ đăng ký thiết bị của bạn.

1. Mở một bảng điều khiển Quản lý Chính sách Nhóm và tạo một GPO mới trong miền của bạn.
     - Cung cấp tên GPO mới tạo của bạn (ví dụ: ClientSideSCP)

2. Sửa GPO và định vị đường dẫn sau đây: **Cấu hình Máy tính > chọn > Windows Cài đặt > ký.**

3. Bấm chuột phải vào Sổ **đăng ký,** rồi **chọn Mục > ký Mới.**

4. Trên tab **Chung,** hãy cấu hình như sau:
  
- **Hành động**: Cập nhật
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Đường dẫn** Khóa : SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Tên giá trị**: TenantId
    
- **Loại giá trị**: REG_SZ
    
- **Dữ liệu giá** trị : GUID hoặc ID Thư mục của phiên bản Azure AD của bạn (Bạn có thể tìm thấy giá trị này trong cổng thông tin **Azure > Azure Active Directory > thuộc tính > ID Thư mục**)
 
- Bấm **OK**.
 
5. Bấm chuột phải vào Sổ **đăng ký,** rồi **chọn Mục > ký Mới.**

6. Trên tab **Chung,** hãy cấu hình như sau:
  
- **Hành động**: Cập nhật
    
- **Hive**: HKEY_LOCAL_MACHINE
    
- **Đường dẫn** Khóa : SOFTWARE\Microsoft\Windows\CurrentVersion\CDJ\AAD
    
- **Tên giá trị**: TenantName
    
- **Loại giá trị**: REG_SZ
    
- **Dữ liệu giá** trị : Tên miền đã xác minh của bạn nếu bạn đang sử dụng môi trường liên kết, chẳng hạn như AD FS. Tên miền đã xác minh hoặc tên miền onmicrosoft.com của bạn (ví dụ: contoso.onmicrosoft).com nếu bạn đang sử dụng môi trường được quản lý

- Bấm **OK**.

7. Đóng trình soạn thảo cho GPO mới được tạo.

8. Nối kết GPO mới được tạo với OU mong muốn có chứa các máy tính nối với tên miền thuộc tổng thể triển khai được kiểm soát của bạn.

Để biết thêm thông tin, hãy [xem mục Xác thực có kiểm soát kết hợp Azure AD kết hợp - Azure AD | Tài liệu Microsoft và](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-control) Khắc [phục sự cố kết hợp Azure Active Directory nối với các thiết | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current).









