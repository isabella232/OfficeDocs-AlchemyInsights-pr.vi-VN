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
ms.openlocfilehash: c32f3f10e2e17cf67e73ec8404be293eeefb68a3
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51821685"
---
# <a name="aip-scanner-installation-and-configuration"></a><span data-ttu-id="ef4a5-102">Máy quét AIP: cài đặt và cấu hình</span><span class="sxs-lookup"><span data-stu-id="ef4a5-102">AIP scanner: installation and configuration</span></span>

<span data-ttu-id="ef4a5-103">**Để cài đặt máy quét AIP, hãy làm theo các hướng dẫn được đề** xuất:</span><span class="sxs-lookup"><span data-stu-id="ef4a5-103">**To install the AIP scanner, follow the recommended guidelines**:</span></span>

1. <span data-ttu-id="ef4a5-104">Nếu bạn đang nâng cấp và không thực hiện cài đặt sạch, hãy đảm bảo rằng bạn đã làm theo các hướng dẫn để [nâng cấp máy quét bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) và đối với máy khách gắn nhãn hợp nhất, hãy xem [mục nâng cấp máy quét bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span><span class="sxs-lookup"><span data-stu-id="ef4a5-104">If you are upgrading and not performing a clean installation, please make sure you have followed the guidelines for [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide#upgrading-the-azure-information-protection-scanner) and for unified labeling client, see [upgrading the Azure Information Protection scanner](https://docs.microsoft.com/azure/information-protection/rms-client/clientv2-admin-guide#upgrading-the-azure-information-protection-scanner).</span></span>
2. <span data-ttu-id="ef4a5-105">Xác nhận rằng bạn tuân thủ tất cả các [tường lửa và các yêu cầu thiết đặt hạ tầng mạng](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span><span class="sxs-lookup"><span data-stu-id="ef4a5-105">Verify that you comply with all [Firewalls and network infrastructure settings requirements](https://docs.microsoft.com/azure/information-protection/requirements#firewalls-and-network-infrastructure).</span></span>
3. <span data-ttu-id="ef4a5-106">Đảm bảo các [chính sách của bạn được thiết lập](https://docs.microsoft.com/azure/information-protection/configure-policy) để ghi nhãn tự động hoặc có nhãn mặc định trong chính sách.</span><span class="sxs-lookup"><span data-stu-id="ef4a5-106">Make sure your [policies are set](https://docs.microsoft.com/azure/information-protection/configure-policy) to automatic labeling or have a default label in the policy.</span></span>
4. <span data-ttu-id="ef4a5-107">Hãy đảm bảo rằng loại tệp liên quan được cấu hình cho nhãn/bảo vệ như được mô tả trong các [kiểu tệp được hỗ trợ bởi máy khách bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span><span class="sxs-lookup"><span data-stu-id="ef4a5-107">Make sure that the relevant file type is configured for label/protection as described in [File types supported by the Azure Information Protection client](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#supported-file-types-for-classification-and-protection).</span></span> <span data-ttu-id="ef4a5-108">Ngoài ra, nếu bạn muốn thay đổi hành vi mặc định, hãy làm theo các hướng dẫn sau: [thay đổi mức độ bảo vệ mặc định của tệp](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span><span class="sxs-lookup"><span data-stu-id="ef4a5-108">In addition, if you want to change the default behavior, follow these guidelines: [Changing the default protection level of files](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-file-types#changing-the-default-protection-level-of-files).</span></span>
5. <span data-ttu-id="ef4a5-109">Xác nhận rằng tài khoản người dùng được cấu hình để chạy dịch vụ máy quét có quyền truy nhập tất cả các kho công việc được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="ef4a5-109">Verify that the user account configured to run the scanner service has permissions to access all the configured repositories.</span></span>
6. <span data-ttu-id="ef4a5-110">Nếu bạn vẫn gặp sự cố, vui lòng xuất Nhật ký máy quét và thêm chúng vào phiếu hỗ trợ của bạn.</span><span class="sxs-lookup"><span data-stu-id="ef4a5-110">If you still experience issues, please export the scanner logs and add them to your support ticket.</span></span>

<span data-ttu-id="ef4a5-111">**Xuất Nhật ký máy quét bảo vệ thông tin Azure**</span><span class="sxs-lookup"><span data-stu-id="ef4a5-111">**Export Azure Information Protection Scanner logs**</span></span>

1. <span data-ttu-id="ef4a5-112">Dẫn hướng đến%localappdata%\Microsoft\MSIP bên dưới ngữ cảnh người dùng đang chạy dịch vụ máy quét.</span><span class="sxs-lookup"><span data-stu-id="ef4a5-112">Navigate to %localappdata%\Microsoft\MSIP under the user context running the scanner service.</span></span>
2. <span data-ttu-id="ef4a5-113">Zip tất cả các nội dung bên dưới thư mục MSIP.</span><span class="sxs-lookup"><span data-stu-id="ef4a5-113">Zip all the contents under the MSIP folder.</span></span>
3. <span data-ttu-id="ef4a5-114">Lưu Nhật ký vào lựa chọn vị trí của bạn và đính kèm chúng vào yêu cầu dịch vụ của bạn.</span><span class="sxs-lookup"><span data-stu-id="ef4a5-114">Save the logs to your choice of location, and attach them to your service request.</span></span>
4. <span data-ttu-id="ef4a5-115">Bạn cũng có thể sử dụng [Export-AIPLogs-OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span><span class="sxs-lookup"><span data-stu-id="ef4a5-115">You can also use [Export-AIPLogs -OnBehalfOf](https://docs.microsoft.com/powershell/module/azureinformationprotection/export-aiplogs?view=azureipps).</span></span>

<span data-ttu-id="ef4a5-116">**Để biết thêm thông tin, hãy xem**:</span><span class="sxs-lookup"><span data-stu-id="ef4a5-116">**For additional information, see**:</span></span>
- [<span data-ttu-id="ef4a5-117">Triển khai máy quét bảo vệ thông tin Azure để tự động phân loại và bảo vệ tệp</span><span class="sxs-lookup"><span data-stu-id="ef4a5-117">Deploying the Azure Information Protection scanner to automatically classify and protect files</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner)
- [<span data-ttu-id="ef4a5-118">Xác định và sử dụng tham số mã thông báo cho Set-Aipxác thực</span><span class="sxs-lookup"><span data-stu-id="ef4a5-118">Specify and use the Token parameter for Set-AIPAuthentication</span></span>](https://docs.microsoft.com/azure/information-protection/rms-client/client-admin-guide-powershell#specify-and-use-the-token-parameter-for-set-aipauthentication)
- [<span data-ttu-id="ef4a5-119">Chạy chu kỳ khám phá và xem báo cáo cho máy quét</span><span class="sxs-lookup"><span data-stu-id="ef4a5-119">Run a discovery cycle and view reports for the scanner</span></span>](https://docs.microsoft.com/azure/information-protection/deploy-aip-scanner#run-a-discovery-cycle-and-view-reports-for-the-scanner)
- [<span data-ttu-id="ef4a5-120">Xem lại tài liệu bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="ef4a5-120">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)
- [<span data-ttu-id="ef4a5-121">Các yêu cầu về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="ef4a5-121">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)
- [<span data-ttu-id="ef4a5-122">Tải xuống máy khách bảo vệ thông tin về Azure</span><span class="sxs-lookup"><span data-stu-id="ef4a5-122">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)
