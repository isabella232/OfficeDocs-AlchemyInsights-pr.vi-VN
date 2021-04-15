---
title: Giải quyết lỗi sản phẩm chưa được cấp phép
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
- "3412"
- "9001428"
ms.openlocfilehash: eebfb7cea7ae97921bf3c3667818400a17b5e52e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51786871"
---
# <a name="suggestions-for-solving-unlicensed-product-errors"></a><span data-ttu-id="6c751-102">Các gợi ý về việc giải quyết lỗi "sản phẩm chưa được cấp phép"</span><span class="sxs-lookup"><span data-stu-id="6c751-102">Suggestions for solving "Unlicensed Product" errors</span></span>

<span data-ttu-id="6c751-103">Để giải quyết các lỗi về "sản phẩm chưa được cấp phép", hãy thử làm như sau:</span><span class="sxs-lookup"><span data-stu-id="6c751-103">To solve errors about an "Unlicensed Product," try the following:</span></span>

- <span data-ttu-id="6c751-104">Kiểm tra xem liệu trạng thái đăng ký của bạn đã hết hạn chưa.</span><span class="sxs-lookup"><span data-stu-id="6c751-104">Check to see if your subscription status has expired.</span></span>
- <span data-ttu-id="6c751-105">Hãy đảm bảo rằng bạn có thuê bao cho phép các giấy phép máy khách, chẳng hạn như ứng dụng Microsoft 365 dành cho doanh nghiệp hoặc doanh nghiệp, đồng [thời, đảm bảo rằng người dùng có giấy phép được gán](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="6c751-105">Make sure you have a subscription that allows client licenses, such as Microsoft 365 Apps for business or Business Premium, and [ensure that the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> 
- <span data-ttu-id="6c751-106">Đảm bảo rằng người dùng đang đăng nhập vào Office bằng cùng tài khoản có giấy phép được gán.</span><span class="sxs-lookup"><span data-stu-id="6c751-106">Make sure the user is signing in to Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="6c751-107">Hãy kiểm tra trang trạng thái [dịch vụ](https://docs.microsoft.com/office365/enterprise/view-service-health) để xem liệu có bất kỳ vấn đề nào đã biết nào với dịch vụ hay không.</span><span class="sxs-lookup"><span data-stu-id="6c751-107">Check the [Service health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="6c751-108">Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy để xác nhận rằng họ không ngăn chặn việc truy nhập ứng dụng Microsoft 365 vào Internet.</span><span class="sxs-lookup"><span data-stu-id="6c751-108">Check your firewall, antivirus software, and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the Internet.</span></span> <span data-ttu-id="6c751-109">Xem [dải URL và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span><span class="sxs-lookup"><span data-stu-id="6c751-109">See [URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).</span></span>

<span data-ttu-id="6c751-110">Bạn cũng có thể thử các hành động khắc phục sự cố sau đây:</span><span class="sxs-lookup"><span data-stu-id="6c751-110">You may also try the following troubleshooting actions:</span></span> 

- <span data-ttu-id="6c751-111">Mở một ứng dụng Office và [đăng xuất khỏi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) mọi tài khoản người dùng hiện có.</span><span class="sxs-lookup"><span data-stu-id="6c751-111">Open an Office app and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="6c751-112">[Loại bỏ](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) và [gán lại](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) giấy phép Office, sau đó [đăng nhập vào Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) bằng tài khoản người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="6c751-112">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) the Office license, and then [sign in to Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="6c751-113">Chạy trình khắc phục sự cố [kích hoạt](https://aka.ms/SARA-OfficeActivation-Alchemy).</span><span class="sxs-lookup"><span data-stu-id="6c751-113">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy).</span></span>
- <span data-ttu-id="6c751-114">[Đặt lại trạng thái kích hoạt Office](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span><span class="sxs-lookup"><span data-stu-id="6c751-114">[Reset the Office activation state](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state).</span></span> 
- <span data-ttu-id="6c751-115">[Thực hiện sửa chữa trực tuyến của Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span><span class="sxs-lookup"><span data-stu-id="6c751-115">[Perform an Online Repair of Office](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b).</span></span>

<span data-ttu-id="6c751-116">Để biết thêm giải pháp khắc phục sự cố, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="6c751-116">For additional troubleshooting solutions, see:</span></span> 

- [<span data-ttu-id="6c751-117">Lỗi sản phẩm chưa được cấp phép và kích hoạt trong Office</span><span class="sxs-lookup"><span data-stu-id="6c751-117">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380)
- [<span data-ttu-id="6c751-118">"Rất tiếc, chúng tôi không thể kết nối với tài khoản của bạn. Xin vui lòng thử lại sau "lỗi" khi bạn kích hoạt Office</span><span class="sxs-lookup"><span data-stu-id="6c751-118">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)