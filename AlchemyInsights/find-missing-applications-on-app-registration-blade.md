---
title: Tìm các ứng dụng bị thiếu trên lưỡi Đăng ký Ứng dụng
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004352"
- "9654"
ms.openlocfilehash: 0dee7e44a8701e1df924b9657cce6cf9d90160e58277d667f6069a4cbcf87ce5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54057124"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Tìm các ứng dụng bị thiếu trên lưỡi Đăng ký Ứng dụng

1. Không thể tìm thấy các ứng dụng trên cổng thông tin Đăng ký Ứng dụng.

    Nếu một ứng dụng là ứng dụng nhiều đối tượng thuê và nó đã được đăng ký trong đối tượng thuê khác, nó sẽ không được hiển thị dưới lưỡi Đăng ký Ứng dụng. Tuy nhiên, bạn có thể tìm thấy phần mềm này bên dưới Enterprise Applications blade sau khi đã truy nhập (sau khi được chấp thuận) và tên dịch vụ chính đã được tạo trong đối tượng thuê của bạn. Để biết thêm thông tin, [hãy xem mục & khoản chính của dịch vụ trong Azure AD - Nền tảng định danh Microsoft.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
2. Không thể xem các ứng dụng trong Lưỡi đăng ký Ứng dụng ngay cả khi bạn là người quản trị.

    Vui lòng đảm bảo rằng bạn đang ở đúng thư mục trên cổng thông tin Azure.
3. Ứng dụng của tôi không được liệt kê bên dưới Enterprise Applications blade nhưng sẽ hiển thị khi tôi truy vấn lệnh PowerShell.

    Đôi khi, sau khi bạn xóa ứng dụng khỏi cổng thông tin Azure, ứng dụng sẽ không hiển thị trong cổng thông tin nhưng có thể ứng dụng đó chưa bị xóa hoàn toàn. Để biết thêm thông tin, hãy xem:
    - Bạn có thể truy xuất danh sách các ứng dụng đã xóa trước đó và xem liệu ứng dụng có hiển thị trong danh sách bằng cách sử dụng lệnh Powershell: **Get-AzureADDeletedApplication**. Để tìm hiểu thêm, [hãy xem Get-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication)
    - Nếu bạn muốn loại bỏ hoàn toàn ứng dụng, bạn có thể thử thực hiện như sau trong PowerShell: **Remove-AzureADApplication -ObjectId.** Để tìm hiểu thêm, [hãy xem loại bỏ-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication)
    - Ngoài ra, bạn có thể thử khôi phục ứng dụng đã xóa bằng lệnh Powershell sau: Khôi phục **AzureADDeletedApplication -ObjectId.** Để tìm hiểu thêm, [hãy xem Restore-AzureADDeletedApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication)
4. Không thể tìm thấy danh sách tất cả các ứng dụng doanh nghiệp được cài đặt sẵn trong đối tượng thuê Azure mới của mình.

    Không có ứng dụng doanh nghiệp nào được cài đặt sẵn trong Azure AD theo mặc định. Bạn cần thêm ứng dụng đó theo cách thủ công từ tùy chọn 'Ứng dụng mới' bằng cách duyệt từ bộ sưu tập Azure AD hoặc thêm ứng dụng không phải bộ sưu tập. Để tìm hiểu thêm, hãy [xem Khởi động nhanh: Thêm ứng dụng vào đối tượng thuê Azure Active Directory (Azure AD) của bạn.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal)
    Nếu bạn là người quản trị toàn cầu, bạn có thể dễ dàng truy nhập các ứng dụng của mình [bằng Microsoft 365 khởi động Ứng dụng](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Không thể tìm thấy ứng dụng của tôi từ cổng thông tin Ứng dụng của Tôi.

    Đảm bảo rằng các ứng dụng không bị ẩn trong trang bộ sưu tập Ứng dụng của Tôi. Để tìm hiểu thêm, xem [mục Bộ sưu tập (bản xem trước) trong cổng thông tin Ứng dụng của Tôi - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Để khởi động ứng dụng từ cổng thông tin Ứng dụng của Tôi, hãy xem Xác định & sử dụng ứng dụng trên [cổng thông tin Ứng dụng của Tôi - Azure AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Office 365 Ứng dụng Mover sẽ không hiển thị trên Enterprise Applications blade sau khi cài đặt.

    Ứng dụng "Office 365 Chuyển đổi" là một ứng dụng đa đối số không cần phải được thêm vào AAD bằng cách dùng phần Ứng dụng Bộ sưu tập bên dưới Đăng ký Ứng dụng Doanh nghiệp. Để truy Office 365 dụng Mover, chỉ cần đăng nhập vào ứng dụng và ứng dụng sẽ yêu cầu người dùng chấp thuận các quyền. Sau khi người dùng đưa ra sự chấp thuận, ứng dụng này sẽ tự động được thêm vào đối tượng thuê có id email mà bạn đã đăng nhập.

    Sau khi đăng nhập vào ứng dụng, bạn sẽ có thể tìm thấy mục nhập của ứng dụng này dưới lá của Enterprise Applications trong AAD. Bạn cần tìm kiếm ứng dụng đó bằng cách nhập tên đầy đủ, ví dụ: "Office 365 Mover" hoặc chỉ cần tìm kiếm "office" và bạn sẽ liệt kê ứng dụng. Để tìm hiểu thêm, hãy xem Office 365 Mover cho biết nó đã được cài đặt nhưng nó không được liệt kê trong bộ [sưu tập Ứng dụng Doanh nghiệp](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html).
8. Khởi động nhanh: Xem danh sách các ứng dụng đang sử dụng đối tượng thuê [Azure Active Directory (Azure AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) của bạn để quản lý căn cước cho bạn biết cách xem các ứng dụng, còn được gọi là ứng dụng, đã được thiết lập để sử dụng đối tượng thuê Azure AD của bạn làm Nhà cung cấp Định danh (IdP).
9. [Khắc phục các sự cố thường gặp khi](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) thêm hoặc loại bỏ một ứng dụng vào Azure Active Directory giúp bạn hiểu được những vấn đề chung mà mọi người gặp phải khi xem ứng dụng Azure Active Directory.
