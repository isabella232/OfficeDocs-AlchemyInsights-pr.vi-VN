---
title: 'Máy quét AIP: cài đặt và cấu hình'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5119"
ms.openlocfilehash: be5b63ffccd5bbd83e7802e4ef5aa657ed921ae6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47686664"
---
# <a name="aip-scanner-installation-and-configuration"></a>Máy quét AIP: cài đặt và cấu hình

**Để cài đặt máy quét AIP, hãy làm theo các hướng dẫn được đề** xuất:

1. Nếu bạn đang nâng cấp và không thực hiện cài đặt sạch, hãy đảm bảo rằng bạn đã làm theo các hướng dẫn để [nâng cấp máy quét bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) và đối với máy khách gắn nhãn hợp nhất, hãy xem [mục nâng cấp máy quét bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).
2. Xác nhận rằng bạn tuân thủ tất cả các [tường lửa và các yêu cầu thiết đặt hạ tầng mạng](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).
3. Đảm bảo các [chính sách của bạn được thiết lập](https://docs.microsoft.com/azure/information-protection/configure-policy) để ghi nhãn tự động hoặc có nhãn mặc định trong chính sách.
4. Hãy đảm bảo rằng loại tệp liên quan được cấu hình cho nhãn/bảo vệ như được mô tả trong các [kiểu tệp được hỗ trợ bởi máy khách bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection). Ngoài ra, nếu bạn muốn thay đổi hành vi mặc định, hãy làm theo các hướng dẫn sau: [thay đổi mức độ bảo vệ mặc định của tệp](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).
5. Xác nhận rằng tài khoản người dùng được cấu hình để chạy dịch vụ máy quét có quyền truy nhập tất cả các kho công việc được cấu hình.
6. Nếu bạn vẫn gặp sự cố, vui lòng xuất Nhật ký máy quét và thêm chúng vào phiếu hỗ trợ của bạn.

**Xuất Nhật ký máy quét bảo vệ thông tin Azure**

1. Dẫn hướng đến%localappdata%\Microsoft\MSIP bên dưới ngữ cảnh người dùng đang chạy dịch vụ máy quét.
2. Zip tất cả các nội dung bên dưới thư mục MSIP.
3. Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ của bạn.
4. Bạn cũng có thể sử dụng [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).

**Để biết thêm thông tin, hãy xem**:
- [Triển khai máy quét bảo vệ thông tin Azure để tự động phân loại và bảo vệ tệp](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [Xác định và sử dụng tham số mã thông báo cho Set-Aipxác thực](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [Chạy chu kỳ khám phá và xem báo cáo cho máy quét](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [Xem lại tài liệu bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [Các yêu cầu về bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [Tải xuống máy khách bảo vệ thông tin về Azure](https://www.microsoft.com/download/details.aspx?id=53018)
