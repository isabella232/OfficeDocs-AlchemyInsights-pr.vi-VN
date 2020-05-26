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
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="c37f4-102">Máy quét AIP: cài đặt và cấu hình</span><span class="sxs-lookup"><span data-stu-id="c37f4-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="c37f4-103">**Để cài đặt máy quét AIP, hãy làm theo các nguyên tắc được đề xuất**:</span><span class="sxs-lookup"><span data-stu-id="c37f4-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="c37f4-104">Nếu bạn đang nâng cấp và không thực hiện cài đặt sạch, hãy chắc chắn rằng bạn đã làm theo các hướng dẫn để [nâng cấp máy quét Azure thông tin bảo vệ](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) và cho khách hàng ghi nhãn hợp nhất, hãy xem [nâng cấp máy quét Azure thông tin bảo vệ](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="c37f4-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="c37f4-105">Xác minh rằng bạn tuân thủ tất cả các [yêu cầu cài đặt tường lửa và hạ tầng mạng](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="c37f4-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="c37f4-106">Đảm bảo rằng [chính sách của bạn được đặt thành](https://docs.microsoft.com/azure/information-protection/configure-policy) ghi nhãn tự động hoặc có nhãn mặc định trong chính sách.</span><span class="sxs-lookup"><span data-stu-id="c37f4-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="c37f4-107">Đảm bảo rằng loại tệp có liên quan được cấu hình cho nhãn/bảo vệ như được mô tả trong [các loại tệp được hỗ trợ bởi khách hàng bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="c37f4-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="c37f4-108">Ngoài ra, nếu bạn muốn thay đổi hành vi mặc định, hãy làm theo các nguyên tắc [sau: thay đổi mức độ bảo vệ mặc định của tệp](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="c37f4-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="c37f4-109">Xác minh rằng tài khoản người dùng cấu hình để chạy dịch vụ máy quét có quyền truy cập vào tất cả các kho cấu hình.</span><span class="sxs-lookup"><span data-stu-id="c37f4-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="c37f4-110">Nếu bạn vẫn gặp sự cố, hãy xuất Nhật ký máy quét và thêm chúng vào vé hỗ trợ của bạn.</span><span class="sxs-lookup"><span data-stu-id="c37f4-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="c37f4-111">**Xuất bản ghi Azure thông tin bảo vệ máy quét**</span><span class="sxs-lookup"><span data-stu-id="c37f4-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="c37f4-112">Điều hướng đến%localappdata%\Microsoft\MSIP trong ngữ cảnh người dùng chạy dịch vụ máy quét.</span><span class="sxs-lookup"><span data-stu-id="c37f4-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="c37f4-113">Zip tất cả các nội dung trong thư mục MSIP.</span><span class="sxs-lookup"><span data-stu-id="c37f4-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="c37f4-114">Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ của bạn.</span><span class="sxs-lookup"><span data-stu-id="c37f4-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="c37f4-115">Bạn cũng có thể sử dụng [xuất-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="c37f4-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="c37f4-116">Để biết **thêm thông tin, xem**:</span><span class="sxs-lookup"><span data-stu-id="c37f4-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="c37f4-117">Triển khai máy quét Azure Information Protection để tự động phân loại và bảo vệ tệp</span><span class="sxs-lookup"><span data-stu-id="c37f4-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="c37f4-118">Chỉ định và sử dụng tham số mã thông báo cho thiết lập-AIPAuthentication</span><span class="sxs-lookup"><span data-stu-id="c37f4-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="c37f4-119">Chạy chu trình khám phá và xem báo cáo cho máy quét</span><span class="sxs-lookup"><span data-stu-id="c37f4-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="c37f4-120">Đánh giá tài liệu về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="c37f4-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="c37f4-121">Yêu cầu đối với bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="c37f4-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="c37f4-122">Tải về Azure bảo vệ thông tin khách hàng</span><span class="sxs-lookup"><span data-stu-id="c37f4-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
