---
title: Lấy danh sách các ứng dụng doanh nghiệp
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
- "9004342"
- "9837"
ms.openlocfilehash: f5c1a77e415d4bbaa5718a6668af95934db7e5ae
ms.sourcegitcommit: e5f261f95ffc6074cce89e62ef8c4e9fd519d3ee
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/26/2021
ms.locfileid: "51405507"
---
# <a name="get-a-list-of-enterprise-applications"></a>Lấy danh sách các ứng dụng doanh nghiệp

1. Để **lấy danh sách các ứng dụng doanh nghiệp** (Tất cả các ứng dụng hoặc được lọc theo tên hiển thị, ID, mã định danh Uris, v.v.) thông qua lệnh PowerShell, hãy xem [Get-AzureADApplication (azuread)](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication).
2. Để lấy danh sách các đối tượng chính của dịch vụ (Tất cả đối tượng hoặc lọc theo ID) thông qua lệnh PowerShell, hãy xem [Get-AzureADServicePrincipal (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal).
3. Nếu bạn muốn **lấy danh sách các ứng dụng được cấu hình SAML, sau đây là các script PowerShell** có thể giúp bạn:

    Mỗi ứng dụng có thể là ứng dụng OAuth hoặc SAML (cả bộ sưu tập và ứng dụng không phải là bộ sưu tập) sẽ có hai đối tượng được tạo ra trong khi đăng ký của họ sẽ xảy ra. Một được gọi là đối tượng ứng dụng và đó là đối tượng dịch vụ chính. Khi bạn đổ các thuộc tính của một đối tượng dịch vụ chủ yếu bằng cách sử dụng PowerShell, bạn sẽ thấy rằng mọi ứng dụng đều có một số lượng thẻ nhất định được liên kết với nó như sau:

    - Ứng dụng OAuth sẽ có một thẻ có tên là "**Windowsazureactivedirecstafintegratedapp**"
    - Bộ sưu tập các ứng dụng SAML sẽ có thẻ có tên là "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Ứng dụng không phải là bộ sưu tập SAML sẽ có thẻ có tên "**Windowsazureactivedirectorycustomsinglesignonapplication**"

    Do đó, bạn có thể sử dụng các thẻ này và tìm hiểu xem loại ứng dụng đó là gì. Thẻ "**Windowsazureactivedirectoryintegratedapp**" là chung cho tất cả các loại ứng dụng. Bạn có thể dùng đoạn trích sau đây để liệt kê tất cả các ứng dụng SAML (cả bộ sưu tập và không phải là bộ sưu tập):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Để biết thêm thông tin, hãy xem mục [xác định các ứng dụng SAML cho phép trong AZURE AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Chỉ tìm kiếm và danh sách các ứng dụng web**: dùng lệnh dưới đây để nhận tất cả các ứng dụng Azure AD với loại ứng dụng "Web App/API"

    Get-AzureADApplication-tất cả: $true | Where-Object {$ _. PublicClient-NE $true} | Bình
5. **Tìm và danh sách các ứng dụng gốc một mình**: chạy lệnh sau đây để nhận tất cả các ứng dụng máy khách gốc (thiết bị di động/thiết bị di động).

    Get-AzureADApplication-tất cả: $true | Where-Object {$ _. PublicClient-EQ $true} | Bình
6. **Xuất tất cả các chi tiết ứng dụng AZURE AD đã đăng ký thành CSV**: lệnh dưới đây xuất chuyển tất cả các ứng dụng Azure AD với chi tiết bắt buộc vào tệp CSV:

    - Get-AzureADApplication-tất cả: $true | Select-Object DisplayName, AppID, PublicClient, Availabletootherthuê, trang chủ, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv"-thông tin mã hóa UTF8

7. **Cần xuất danh sách các ứng dụng Azure không sử dụng** – báo cáo kiểm nghiệm

    Azure AD có thể hiển thị Nhật ký ứng dụng chỉ có tối đa 30 ngày cung cấp cho bạn giấy phép Azure AD Premium.
    Bạn có hai tùy chọn để giữ lại dữ liệu trong hơn 30 ngày. Bạn có thể sử dụng [API báo cáo AZURE AD](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) để truy xuất các chương trình dữ liệu và lưu trữ nó trong một cơ sở dữ liệu. Ngoài ra, bạn có thể tích hợp Nhật ký kiểm tra vào một hệ thống SIEM của bên thứ ba.

    Bạn cũng có thể tải xuống danh sách ứng dụng cho tất cả các ứng dụng và các ứng dụng thuộc đối với đăng ký ứng dụng Azure Active Directory>>tải xuống>tất cả các ứng dụng/ứng dụng thuộc sở hữu.

    Để lấy danh sách các ứng dụng thông qua MS graph, hãy xem [ứng dụng danh sách-Microsoft graph v 1.0](https://docs.microsoft.com/graph/api/application-list) và [loại tài nguyên ứng dụng-Microsoft graph v 1.0](https://docs.microsoft.com/graph/api/resources/application).
