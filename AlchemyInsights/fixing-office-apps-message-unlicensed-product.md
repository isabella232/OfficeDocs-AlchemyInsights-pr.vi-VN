---
title: Không thể kích hoạt Office
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
- "2000023"
- "3509"
ms.openlocfilehash: e052c18eae035ff05c70a223f6d8a2eab875b2c9
ms.sourcegitcommit: 57102d7daf32f370cab84dba342819a1ad5cb261
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/23/2020
ms.locfileid: "48236111"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="15a22-102">Không thể kích hoạt Office</span><span class="sxs-lookup"><span data-stu-id="15a22-102">Unable to activate Office</span></span>

- <span data-ttu-id="15a22-103">Kiểm tra xem trạng thái đăng ký của bạn đã hết hạn chưa.</span><span class="sxs-lookup"><span data-stu-id="15a22-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="15a22-104">Đảm bảo bạn có thuê bao cho phép các giấy phép máy khách, chẳng hạn như Office 365 Business hoặc Business Premium và [đảm bảo người dùng có giấy phép được gán](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).</span><span class="sxs-lookup"><span data-stu-id="15a22-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/subscriptions-and-billing/assign-licenses-to-users).</span></span>
- <span data-ttu-id="15a22-105">Đảm bảo người dùng đăng nhập vào Office bằng cùng tài khoản có giấy phép được gán.</span><span class="sxs-lookup"><span data-stu-id="15a22-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="15a22-106">Hãy kiểm tra trang trạng thái [dịch vụ của Office 365](https://docs.microsoft.com/office365/enterprise/view-service-health) để xem liệu có bất kỳ vấn đề nào đã biết với dịch vụ hay không.</span><span class="sxs-lookup"><span data-stu-id="15a22-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="15a22-107">Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy để xác nhận rằng họ không ngăn chặn việc truy nhập ứng dụng Microsoft 365 vào Internet.</span><span class="sxs-lookup"><span data-stu-id="15a22-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="15a22-108">Vui lòng xem các [URL của Office 365 và dải địa chỉ IP](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "URL và dải địa chỉ IP của Office 365").</span><span class="sxs-lookup"><span data-stu-id="15a22-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="15a22-109">**Mẹo** Trên máy Windows, chúng tôi có thể chẩn đoán và tự động khắc phục một số vấn đề đăng nhập Office thông thường cho bạn.</span><span class="sxs-lookup"><span data-stu-id="15a22-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="15a22-110">Tải xuống và chạy trình trợ  **[giúp phục hồi và hỗ trợ của Microsoft](https://aka.ms/SaRA-OfficeSignInScenario)** để sử dụng công cụ tự động của chúng tôi.</span><span class="sxs-lookup"><span data-stu-id="15a22-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="15a22-111">Sử dụng các hành động khắc phục sự cố sau đây:</span><span class="sxs-lookup"><span data-stu-id="15a22-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="15a22-112">Mở một ứng dụng Office và [đăng xuất khỏi](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) bất kỳ tài khoản người dùng hiện có nào.</span><span class="sxs-lookup"><span data-stu-id="15a22-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="15a22-113">[Loại bỏ](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) và [gán lại](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) giấy phép Office, sau đó [đăng nhập vào Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) bằng tài khoản người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="15a22-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="15a22-114">Chạy trình khắc phục sự cố [kích hoạt](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="15a22-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="15a22-115">Đặt lại trạng thái kích hoạt Office</span><span class="sxs-lookup"><span data-stu-id="15a22-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Đặt lại trạng thái kích hoạt Office")
- [<span data-ttu-id="15a22-116">Thực hiện sửa chữa trực tuyến của Office</span><span class="sxs-lookup"><span data-stu-id="15a22-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="15a22-117">Để biết thêm giải pháp khắc phục sự cố, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="15a22-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="15a22-118">Lỗi sản phẩm chưa được cấp phép và kích hoạt trong Office</span><span class="sxs-lookup"><span data-stu-id="15a22-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="15a22-119">"Rất tiếc, chúng tôi không thể kết nối với tài khoản của bạn. Xin vui lòng thử lại sau "lỗi" khi bạn kích hoạt Office</span><span class="sxs-lookup"><span data-stu-id="15a22-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)