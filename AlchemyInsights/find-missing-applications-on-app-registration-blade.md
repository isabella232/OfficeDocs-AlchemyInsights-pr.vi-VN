---
title: Tìm các ứng dụng bị thiếu trên lưỡi đăng ký ứng dụng
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
ms.openlocfilehash: 00b5821e2edad8b60ff60b1f85264d81c72277e4
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51405226"
---
# <a name="find-missing-applications-on-app-registration-blade"></a>Tìm các ứng dụng bị thiếu trên lưỡi đăng ký ứng dụng

1. Không thể tìm thấy các ứng dụng trên cổng đăng ký ứng dụng.

    Nếu một ứng dụng là một ứng dụng nhiều đối tượng thuê và nó đã được đăng ký tại một đối tượng thuê khác, nó sẽ không được hiển thị bên dưới lưỡi đăng ký ứng dụng. Tuy nhiên, bạn có thể tìm thấy nó trong lưỡi ứng dụng doanh nghiệp sau khi đã được truy nhập (sau khi được đồng ý) và hiệu trưởng dịch vụ đã được tạo ra trong đối tượng thuê của bạn. Để biết thêm thông tin, hãy xem mục các [ứng dụng & hiệu trưởng dịch vụ trong AZURE AD-Microsoft Identity Platform](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
2. Không thể xem các ứng dụng trong lưỡi đăng ký ứng dụng mặc dù bạn là người quản trị.

    Xin vui lòng đảm bảo bạn đang ở trong danh bạ bên phải trên cổng thông tin Azure.
3. Ứng dụng của tôi không được liệt kê trong lưỡi ứng dụng Enterprise nhưng nó sẽ hiển thị khi tôi truy vấn lệnh PowerShell.

    Đôi khi, sau khi bạn xóa ứng dụng khỏi Azure Portal, nó không hiển thị trong cổng thông tin nhưng có thể không bị xóa hoàn toàn. Để biết thêm thông tin, hãy xem:
    - Bạn có thể truy xuất danh sách các ứng dụng đã xóa trước đó và xem liệu ứng dụng này có hiển thị trong danh sách bằng cách sử dụng lệnh PowerShell: **Get-AzureADDeletedApplication**. Để tìm hiểu thêm, hãy xem [Get-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureaddeletedapplication).
    - Nếu bạn muốn loại bỏ hoàn toàn ứng dụng, bạn có thể thử những điều sau trong PowerShell: **loại bỏ-AzureADApplication-ObjectId**. Để tìm hiểu thêm, hãy xem [loại bỏ-AzureADApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplication).
    - Ngoài ra, bạn có thể thử khôi phục ứng dụng đã xóa bằng lệnh PowerShell sau đây: **khôi phục AzureADDeletedApplication-ObjectId**. Để tìm hiểu thêm, hãy xem [khôi phục-AzureADDeletedApplication (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
4. Không thể tìm thấy danh sách tất cả các ứng dụng doanh nghiệp được cài đặt sẵn trong Azure đối tượng thuê mới của tôi.

    Không có ứng dụng doanh nghiệp được cài đặt sẵn trong Azure AD theo mặc định. Bạn cần thêm nó theo cách thủ công từ tùy chọn ' ứng dụng mới ' bằng cách duyệt web từ Azure AD Gallery hoặc thêm ứng dụng không phải là bộ sưu tập. Để tìm hiểu thêm, hãy xem [bắt đầu nhanh: thêm ứng dụng vào đối tượng thuê Azure Active Directory (AZURE AD)](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal).
    Nếu bạn là người quản trị toàn cầu, bạn có thể dễ dàng truy nhập các ứng dụng của mình bằng công cụ khởi động [ứng dụng Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/manage/customize-the-app-launcher).
5. Không thể tìm thấy ứng dụng của tôi từ cổng thông tin ứng dụng của tôi.

    Hãy đảm bảo rằng các ứng dụng không bị ẩn trong trang tuyển tập ứng dụng của tôi. Để tìm hiểu thêm, hãy xem [mục tuyển tập (bản xem trước) trong cổng thông tin ứng dụng của tôi-AZURE AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-user-collections).
6. Để bắt đầu ứng dụng từ cổng thông tin ứng dụng của tôi, hãy xem mục [định vị & sử dụng các ứng dụng trên cổng thông tin ứng dụng của tôi-AZURE AD](https://docs.microsoft.com/azure/active-directory/user-help/my-apps-portal-end-user-access).
7. Ứng dụng Office 365 Mover không hiển thị trên lưỡi ứng dụng doanh nghiệp sau khi cài đặt.

    Ứng dụng "trình hướng dẫn Office 365 là một ứng dụng đa đối tượng thuê không cần được thêm vào AAD bằng cách dùng phần ứng dụng bộ sưu tập bên dưới đăng ký ứng dụng doanh nghiệp. Để truy nhập ứng dụng Mover của Office 365, chỉ cần đăng nhập vào ứng dụng và nó sẽ yêu cầu người dùng chấp thuận cho các quyền. Sau khi người dùng cung cấp sự đồng ý, ứng dụng này sẽ tự động được thêm vào đối tượng thuê với ID email mà bạn đã đăng nhập.

    Sau khi đăng nhập vào ứng dụng, bạn sẽ có thể tìm thấy mục nhập ứng dụng này bên dưới lưỡi ' ứng dụng doanh nghiệp ' trong Bad. Bạn cần tìm kiếm ứng dụng đó bằng cách nhập tên đầy đủ, tức là "mover của Office 365" hoặc chỉ tìm kiếm "Office" và nó sẽ liệt kê ứng dụng. Để tìm hiểu thêm, hãy xem [mục Office 365 Mover nói rằng nó đã được cài đặt nhưng nó không được liệt kê trong bộ sưu tập ứng dụng doanh nghiệp](https://docs.microsoft.com/answers/questions/30186/office-365-mover-says-its-already-installed-but-it.html).
8. [Bắt đầu nhanh: xem danh sách các ứng dụng đang sử dụng đối tượng thuê Azure Active Directory (AZURE AD) của bạn để quản lý định danh](https://docs.microsoft.com/azure/active-directory/manage-apps/view-applications-portal) hướng dẫn bạn cách xem các ứng dụng, còn được gọi là các ứng dụng, vốn đã được thiết lập để sử dụng các đối tượng thuê Azure AD của bạn làm nhà cung cấp danh tính (IDP).
9. [Khắc phục sự cố phổ biến về việc thêm hoặc loại bỏ một ứng dụng vào Azure Active Directory](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-adding-apps) sẽ giúp bạn hiểu được những vấn đề thường gặp về những người đang xem các ứng dụng trong Azure Active Directory.
