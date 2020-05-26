---
title: 'Máy quét AIP: cài đặt và cấu hình'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: d059d411aef03ca57662b71fbd7d27aecd3e0e57
ms.sourcegitcommit: c46b8df485edbd13e8bb4d1b2ba1c2821ddc9da0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/23/2020
ms.locfileid: "44358571"
---
# <a name="aip-scanner-installation-and-configuration"></a>Máy quét AIP: cài đặt và cấu hình

**Để cài đặt máy quét AIP, hãy làm theo các nguyên tắc được đề xuất**:

1. Nếu bạn đang nâng cấp và không thực hiện cài đặt sạch, hãy chắc chắn rằng bạn đã làm theo các hướng dẫn để [nâng cấp máy quét Azure thông tin bảo vệ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) và cho khách hàng ghi nhãn hợp nhất, hãy xem [nâng cấp máy quét Azure thông tin bảo vệ](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Xác minh rằng bạn tuân thủ tất cả các [yêu cầu cài đặt tường lửa và hạ tầng mạng](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Đảm bảo rằng [chính sách của bạn được đặt thành](https://docs.microsoft.com/azure/information-protection/configure-policy) ghi nhãn tự động hoặc có nhãn mặc định trong chính sách.
4. Đảm bảo rằng loại tệp có liên quan được cấu hình cho nhãn/bảo vệ như được mô tả trong [các loại tệp được hỗ trợ bởi khách hàng bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Ngoài ra, nếu bạn muốn thay đổi hành vi mặc định, hãy làm theo các nguyên tắc [sau: thay đổi mức độ bảo vệ mặc định của tệp](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Xác minh rằng tài khoản người dùng cấu hình để chạy dịch vụ máy quét có quyền truy cập vào tất cả các kho cấu hình.
6. Nếu bạn vẫn gặp sự cố, hãy xuất Nhật ký máy quét và thêm chúng vào vé hỗ trợ của bạn.

**Xuất bản ghi Azure thông tin bảo vệ máy quét**

1. Điều hướng đến%localappdata%\Microsoft\MSIP trong ngữ cảnh người dùng chạy dịch vụ máy quét.
2. Zip tất cả các nội dung trong thư mục MSIP.
3. Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ của bạn.
4. Bạn cũng có thể sử dụng [xuất-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

Để biết **thêm thông tin, xem**:
- [Triển khai máy quét Azure Information Protection để tự động phân loại và bảo vệ tệp](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Chỉ định và sử dụng tham số mã thông báo cho thiết lập-AIPAuthentication](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Chạy chu trình khám phá và xem báo cáo cho máy quét](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Đánh giá tài liệu về bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Yêu cầu đối với bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tải về Azure bảo vệ thông tin khách hàng](https://www.microsoft.com/download/details.aspx?id=53018)
