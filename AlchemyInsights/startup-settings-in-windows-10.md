---
title: Cài đặt khởi động trong Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001691"
- "3768"
ms.openlocfilehash: 526b92013f26675b5bf42077271ae7dc7003af31fa8f605d76aea92e0ccabfa1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53909848"
---
# <a name="startup-settings-in-windows-10"></a>Cài đặt khởi động trong Windows 10

**Thay đổi các ứng dụng tự động chạy khi khởi động**

1. Đi tới [Cài đặt > Apps > Startup](ms-settings:startupapps?activationSource=GetHelp).

2. Đảm bảo mọi ứng dụng bạn muốn chạy khi khởi động đều **được Bật**.

**Thêm ứng dụng để chạy tự động khi khởi động**

1. Bấm hoặc nhấn vào **Bắt** đầu và tìm ứng dụng mà bạn muốn chạy khi khởi động.

2. Bấm chuột phải vào ứng dụng, bấm **Thêm**, sau đó bấm **Mở vị trí tệp**. Làm như vậy sẽ mở vị trí lưu lối tắt đến ứng dụng. Nếu không có tùy chọn cho Mở vị trí tệp, nghĩa là ứng dụng không thể chạy khi khởi động.

3. Khi vị trí tệp mở, hãy **nhấn phím Windows logo + R**, type **shell:startup**, sau đó bấm **OK.** Làm như vậy sẽ mở thư mục Khởi động.

4. Sao chép và dán lối tắt đến ứng dụng từ vị trí tệp vào thư mục Khởi động.

**Tùy chọn khởi động nâng cao (bao Két sắt Mode, cài đặt UEFI và khởi động từ thiết bị khác)**

1. Lưu công việc của bạn và đóng mọi tài liệu đang mở, vì các bước này sẽ khởi động lại PC của bạn.

2. Đi tới Cài đặt > [Cập nhật & hồi > hồi](ms-settings:recovery?activationSource=GetHelp).

3. Bên dưới **Khởi động nâng cao,** bấm **vào Khởi động lại ngay**. 

4. Sau khi PC khởi động lại đến màn hình Chọn một tùy chọn:

    - Để khởi động từ một thiết bị như ổ đĩa USB, bấm vào **Sử dụng thiết bị**.

    - To enter the UEFI settings (sometimes called BIOS setup), click **troubleshoot > Advanced options > UEFI Firmware Cài đặt**. 

    - Để vào Chế độ Két sắt thay đổi thiết đặt khởi động nâng cao, hãy bấm Khắc phục sự cố > chọn Nâng cao > **khởi Cài đặt**, sau đó bấm Khởi động **lại.** Bạn có thể được yêu cầu nhập khóa [khôi phục BitLocker.](https://support.microsoft.com/help/4026181/windows-10-find-my-bitlocker-recovery-key) Sau khi PC khởi động lại lần nữa, hãy bấm vào thiết đặt khởi động mà bạn muốn sử dụng.