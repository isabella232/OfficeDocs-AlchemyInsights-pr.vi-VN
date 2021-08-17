---
title: Tải danh sách các Ứng dụng Doanh nghiệp
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
ms.openlocfilehash: 99e4f7e676610103355736ce847930c6c5d2d7532c4756ac4551a8d9b3020176
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54116750"
---
# <a name="get-a-list-of-enterprise-applications"></a>Tải danh sách các Ứng dụng Doanh nghiệp

1. Để có danh sách các ứng dụng doanh nghiệp **(tất** cả các ứng dụng hoặc được lọc theo Tên hiển thị, ID, IS Mã định danh, v.v.) thông qua lệnh Powershell, hãy xem [Get-AzureADApplication (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadapplication)
2. Để có danh sách các đối tượng chính của dịch vụ (tất cả các đối tượng hoặc được lọc bằng ID) thông qua lệnh Powershell, hãy xem [Get-AzureADServicePrincipal (AzureAD).](https://docs.microsoft.com/powershell/module/azuread/get-azureadserviceprincipal)
3. Nếu bạn muốn có danh **sách các ứng dụng được đặt cấu hình SAML,** thì những tập lệnh PowerShell sau đây có thể giúp bạn:

    Mỗi ứng dụng đều là một ứng dụng OAuth hoặc ứng dụng SAML (cả bộ sưu tập lẫn ứng dụng không phải bộ sưu tập) sẽ có hai đối tượng được tạo trong AAD khi việc đăng ký của chúng diễn ra. Một đối tượng được gọi là Đối tượng Ứng dụng và đối tượng còn lại được gọi là đối tượng Chính của Dịch vụ. Khi bạn kết xuất các thuộc tính của Đối tượng Chính của Dịch vụ bằng PowerShell, bạn sẽ thấy rằng mọi ứng dụng có một số lượng Thẻ nhất định liên kết với đối tượng đó, chẳng hạn như:

    - Các ứng dụng OAuth sẽ có thẻ có tên "**WindowsAzureActiveDirectoryIntegratedApp**"
    - Gallery SAML Apps would have a tag called "**WindowsAzureActiveDirectoryGalleryApplicationPrimaryV1**"
    - Ứng dụng SAML Không phải Thư viện sẽ có một thẻ có tên là "**WindowsAzureActiveDirectoryCustomSingleSignOnApplication**"

    Do đó, bạn có thể sử dụng các thẻ này và tìm hiểu loại ứng dụng đó. Thẻ "**WindowsAzureActiveDirectoryIntegratedApp**" phổ biến với tất cả các loại ứng dụng. Bạn có thể sử dụng các đoạn mã sau đây để liệt kê tất cả các ứng dụng SAML (cả bộ sưu tập lẫn không phải bộ sưu tập):

    `$type = "SAML APP"`

    `Get-AzureADServicePrincipal -All true | Where-Object {(.Tags -contains "WindowsAzureActiveDirectoryGalleryApplicationNonPrimaryV1") -or (_.Tags -contains "WindowsAzureActiveDirectoryCustomSingleSignOnApplication")} | Select DisplayName, @{Name="AppType"; Expression={type}}_.`

    Để biết thêm thông tin, [hãy xem mục Xác định các ứng dụng hỗ trợ SAML trong Azure AD](https://docs.microsoft.com/answers/questions/24259/identify-saml-enabled-apps-in-azure-ad.html).

4. **Chỉ tìm và chỉ liệt kê các ứng** dụng Web : Sử dụng lệnh dưới đây để nhận được tất cả các ứng dụng Azure AD với loại ứng dụng "Ứng dụng web/API"

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -ne $true } | FT
5. **Tìm và liệt kê riêng các ứng dụng gốc**: Chạy lệnh sau đây để tải tất cả ứng dụng máy khách gốc (máy tính để bàn/thiết bị di động).

    Get-AzureADApplication -All:$true | Where-Object { $_. PublicClient -eq $true } | FT
6. Xuất Tất cả Chi tiết Ứng dụng Azure AD đã Đăng ký sang **CSV:** Lệnh dưới đây sẽ xuất tất cả các ứng dụng Azure AD với các chi tiết bắt buộc sang tệp csv:

    - Get-AzureADApplication -All:$true | Select-Object DisplayName, AppID, PublicClient, AvailableToOtherTenants, HomePage, LogoutUrl |
    - Export-Csv "C:\AzureADApps.csv" -NoTypeInformation -Encoding UTF8

7. **Cần xuất danh sách các ứng dụng Azure không sử dụng tới –** Báo cáo kiểm tra

    Azure AD có thể hiển thị nhật ký ứng dụng chỉ trong tối đa 30 ngày, miễn là bạn có giấy phép Azure AD Premium phép.
    Bạn có hai tùy chọn để lưu giữ dữ liệu trong thời gian hơn 30 ngày. Bạn có thể sử dụng [API Báo cáo Azure AD để truy xuất](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-reporting-api) dữ liệu theo chương trình và lưu trữ dữ liệu trong cơ sở dữ liệu. Ngoài ra, bạn có thể tích hợp nhật ký kiểm tra vào hệ thống SIEM của bên thứ ba.

    Bạn cũng có thể tải xuống danh sách ứng dụng cho mọi ứng dụng và ứng dụng sở hữu bên dưới Đăng ký Ứng dụng Azure Active directory>>Tải xuống>cả ứng dụng/Ứng dụng đã sở hữu.

    Để có danh sách các ứng dụng thông qua MS Graph, hãy xem mục Liệt kê các ứng dụng [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-list) và loại tài nguyên ứng dụng [- Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/resources/application).
