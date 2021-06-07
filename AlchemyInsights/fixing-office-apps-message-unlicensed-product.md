---
title: Không thể kích hoạt các Office
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
- "2000023"
- "3509"
ms.openlocfilehash: 81941d84127a096c3bd588dafc61b492ab6d6458
ms.sourcegitcommit: 1eee2412dfb8b1f10a3aa28dd1086a0c589cdba0
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2021
ms.locfileid: "52798702"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="a2ed8-102">Không thể kích hoạt các Office</span><span class="sxs-lookup"><span data-stu-id="a2ed8-102">Unable to activate Office</span></span>

<span data-ttu-id="a2ed8-103">**Lưu** ý: Nếu bạn đang sử dụng phiên bản cũ hơn của Windows (ví dụ: Windows 7), hãy đảm bảo rằng TLS 1.2 được bật làm mặc định.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-103">**Note**: If you are using an older version of Windows (For example, Windows 7), ensure that TLS 1.2 is enabled as the default.</span></span> <span data-ttu-id="a2ed8-104">Để biết thêm thông tin, hãy xem Cập nhật để bật [TLS 1.1 và TLS 1.2](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392)làm giao thức bảo mật mặc định trong WinHTTP trong Windows.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-104">For more information, see [Update to enable TLS 1.1 and TLS 1.2 as default secure protocols in WinHTTP in Windows](https://support.microsoft.com/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392).</span></span>

- <span data-ttu-id="a2ed8-105">Kiểm tra xem trạng thái đăng ký của bạn đã hết hạn chưa.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-105">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="a2ed8-106">Đảm bảo bạn có đăng ký cho phép giấy phép máy khách, chẳng hạn như Office 365 Business hoặc Business Premium, và đảm bảo người dùng có [giấy phép được gán.](/microsoft-365/admin/manage/assign-licenses-to-users)</span><span class="sxs-lookup"><span data-stu-id="a2ed8-106">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](/microsoft-365/admin/manage/assign-licenses-to-users).</span></span>
- <span data-ttu-id="a2ed8-107">Đảm bảo người dùng đăng nhập vào Office bằng chính tài khoản đã được gán giấy phép.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-107">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="a2ed8-108">Hãy kiểm tra [Office 365 Trạng tác Dịch vụ Để](/office365/enterprise/view-service-health) xem liệu có bất kỳ sự cố đã biết nào với dịch vụ này không.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-108">Check the [Office 365 Service Health page](/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="a2ed8-109">Kiểm tra tường lửa, phần mềm chống vi-rút và thiết đặt proxy của bạn để xác nhận rằng họ không chặn Microsoft 365 ứng dụng truy nhập internet.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-109">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="a2ed8-110">Vui lòng [xem Office 365 URL và dải địa chỉ IP mới.](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URL và dải địa chỉ IP")</span><span class="sxs-lookup"><span data-stu-id="a2ed8-110">Please see [Office 365 URLs and IP address ranges](/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="a2ed8-111">**Mẹo** Trên Windows tính, chúng tôi có thể chẩn đoán và tự động khắc phục một số sự cố Office đăng nhập thường gặp cho bạn.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-111">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="a2ed8-112">Tải xuống và chạy Microsoft Công cụ Trợ giúp Phục hồi và Hỗ trợ **[cách sử dụng](https://aka.ms/SaRA-OfficeSignInScenario)** công cụ tự động của chúng tôi.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-112">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="a2ed8-113">Sử dụng các hành động khắc phục sự cố sau đây:</span><span class="sxs-lookup"><span data-stu-id="a2ed8-113">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="a2ed8-114">Mở một tài Ứng dụng Office và đăng xuất [khỏi bất kỳ](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) tài khoản người dùng hiện có nào.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-114">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="a2ed8-115">[Loại](/microsoft-365/admin/manage/remove-licenses-from-users) bỏ [và gán lại giấy](/microsoft-365/admin/manage/assign-licenses-to-users) Office, rồi đăng nhập vào tài [Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) sử dụng tài khoản người dùng bị ảnh hưởng.</span><span class="sxs-lookup"><span data-stu-id="a2ed8-115">[Remove](/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="a2ed8-116">Chạy Trình khắc phục [sự cố Kích hoạt](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="a2ed8-116">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="a2ed8-117">Đặt lại Office thái kích hoạt</span><span class="sxs-lookup"><span data-stu-id="a2ed8-117">Reset Office activation state</span></span>](/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Đặt lại Office thái kích hoạt")
- [<span data-ttu-id="a2ed8-118">Thực hiện Sửa chữa Trực tuyến Office</span><span class="sxs-lookup"><span data-stu-id="a2ed8-118">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="a2ed8-119">Để biết thêm các giải pháp khắc phục sự cố, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="a2ed8-119">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="a2ed8-120">Lỗi Sản phẩm Chưa được cấp phép và kích hoạt trong Office</span><span class="sxs-lookup"><span data-stu-id="a2ed8-120">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="a2ed8-121">"Rất tiếc, chúng tôi không thể kết nối với tài khoản của bạn. Lỗi vui lòng thử lại sau" khi bạn kích hoạt Office</span><span class="sxs-lookup"><span data-stu-id="a2ed8-121">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)