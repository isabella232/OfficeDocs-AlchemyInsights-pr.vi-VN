---
title: 'Máy quét AIP: cài đặt và cấu hình'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: 75fd61e18503292bd5fa9e48c7cdba7692282925a419b3230d17448eab928ba0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/05/2021
ms.locfileid: "53934279"
---
# <a name="aip-scanner-installation-and-configuration"></a>Máy quét AIP: cài đặt và cấu hình

**Để cài đặt máy quét AIP, hãy làm theo các hướng dẫn được đề xuất:**

1. Nếu bạn đang nâng cấp và không thực hiện cài đặt sạch, vui lòng đảm bảo rằng bạn đã làm theo các hướng dẫn để nâng cấp Trình quét Thông tin [Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) và cho máy khách dán nhãn hợp nhất, hãy xem nâng cấp Trình quét Azure [Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner)
2. Xác minh rằng bạn tuân thủ tất cả các yêu [cầu về Tường lửa và cài đặt cơ sở hạ tầng mạng.](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure)
3. Hãy đảm bảo rằng [chính sách của bạn được](https://docs.microsoft.com/azure/information-protection/configure-policy) đặt thành tự động đánh nhãn hoặc có nhãn mặc định trong chính sách.
4. Hãy đảm bảo rằng loại tệp liên quan được cấu hình cho nhãn/bảo vệ như được mô tả trong các kiểu tệp được hỗ trợ [bởi máy khách Azure Information Protection.](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection) Ngoài ra, nếu bạn muốn thay đổi hành vi mặc định, hãy làm theo các hướng dẫn sau: [Thay đổi mức bảo vệ mặc định của tệp](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Xác minh rằng tài khoản người dùng đã cấu hình để chạy dịch vụ máy quét có quyền truy nhập vào tất cả kho lưu trữ được đặt cấu hình.
6. Nếu bạn vẫn gặp sự cố, vui lòng xuất nhật ký máy quét và thêm vào thẻ hỗ trợ của bạn.

**Xuất nhật ký Azure Information Protection Scanner**

1. Dẫn hướng đến %localappdata%\Microsoft\MSIP trong ngữ cảnh người dùng đang chạy dịch vụ máy quét.
2. Nén tất cả nội dung bên dưới thư mục MSIP.
3. Lưu nhật ký vào lựa chọn của bạn về vị trí và đính kèm nhật ký vào yêu cầu dịch vụ của bạn.
4. Bạn cũng có thể [dùng Export-AIPLogs -OnBehalfOf.](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps)

**Để biết thêm thông tin, hãy xem:**
- [Triển khai trình quét Azure Information Protection để tự động phân loại và bảo vệ tệp](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Xác định và sử dụng tham số Token cho Set-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Chạy chu kỳ khám phá và xem báo cáo cho máy quét](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Xem lại hướng dẫn sử dụng Azure Information Protection](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Yêu cầu đối với Azure Information Protection](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tải xuống máy khách Azure Information Protection](https://www.microsoft.com/download/details.aspx?id=53018)
