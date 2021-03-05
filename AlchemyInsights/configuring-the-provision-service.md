---
title: Cấu hình dịch vụ cung cấp
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
- "9004687"
- "8468"
ms.openlocfilehash: fd272f8d554d73c87b832443815c25ebb2acc3eb
ms.sourcegitcommit: b71e5981b7f30ef2bce4e695118d03aa68a5be4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/05/2021
ms.locfileid: "50484049"
---
# <a name="configuring-the-provision-service"></a><span data-ttu-id="98dda-102">Cấu hình dịch vụ cung cấp</span><span class="sxs-lookup"><span data-stu-id="98dda-102">Configuring the Provision service</span></span>

<span data-ttu-id="98dda-103">Để cung cấp cho người dùng tự động hoạt động, Azure AD yêu cầu chứng danh hợp lệ cho phép nó kết nối với API dịch vụ web ngày làm việc.</span><span class="sxs-lookup"><span data-stu-id="98dda-103">For automated user provisioning to work, Azure AD requires valid credentials that allow it to connect to Workday Web Services API.</span></span> <span data-ttu-id="98dda-104">Ngoài ra, nút kết nối kiểm tra trong ngày làm việc đến ứng dụng cung cấp người dùng quảng cáo cũng xác nhận nếu có thể kết nối với đại diện cung cấp kết nối Azure AD được liên kết với tên miền quảng cáo.</span><span class="sxs-lookup"><span data-stu-id="98dda-104">Further, the Test Connection button on the Workday to AD User Provisioning app also validates if it is able to connect to the Azure AD Connect Provisioning Agent associated with the AD Domain.</span></span>

<span data-ttu-id="98dda-105">Nếu cổng Azure sẽ trả về lỗi khi lưu chứng danh, hãy làm theo các bước được đề xuất dưới đây:</span><span class="sxs-lookup"><span data-stu-id="98dda-105">If the Azure portal is returning an error upon saving the credentials, follow the recommended steps below:</span></span>

1. <span data-ttu-id="98dda-106">Xác nhận rằng bạn đã cấu hình tài khoản người dùng hệ thống tích hợp workday như đã nêu trong phần hướng dẫn [cấu hình người dùng hệ thống tích hợp trong ngày](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)làm việc.</span><span class="sxs-lookup"><span data-stu-id="98dda-106">Confirm that you have configured Workday Integration System User account as stated in the tutorial section [Configure integration system user in Workday](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
2. <span data-ttu-id="98dda-107">Xác nhận rằng dịch vụ đại diện cung cấp Azure AD kết nối đang được thiết lập và chạy trên Windows Server tại cơ sở của bạn bằng cách sử dụng bảng điều khiển quản lý Dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="98dda-107">Confirm that the Azure AD Connect Provisioning Agent Service is up and running on your on-premises Windows server using the Services Management Console.</span></span> <span data-ttu-id="98dda-108">Bạn cũng có thể kiểm tra trạng thái của đại diện trong cổng thông tin Azure bằng cách bấm vào nút xem các đại diện tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="98dda-108">You can also check the status of the agent in the Azure portal by clicking the View on-premises agents button.</span></span>
3. <span data-ttu-id="98dda-109">Đảm bảo rằng bạn đang nhập giá trị cho trường "username Day Username" bằng cách dùng định dạng username@workday-đối tượng thuê.</span><span class="sxs-lookup"><span data-stu-id="98dda-109">Ensure that you are entering the value for "Workday Username" field using the format username@workday-tenant-name.</span></span> <span data-ttu-id="98dda-110">Nếu thiếu tên đối tượng thuê ngày làm việc, xác thực ngày làm việc không thành công.</span><span class="sxs-lookup"><span data-stu-id="98dda-110">If the workday-tenant-name is missing, Workday authentication fails.</span></span>
4. <span data-ttu-id="98dda-111">Nếu bạn đang cấu hình tích hợp với đối tượng thuê thực thi ngày làm việc, hãy lưu ý những giờ thời gian ngừng hoạt động của đối tượng thuê ngày làm việc của bạn.</span><span class="sxs-lookup"><span data-stu-id="98dda-111">If you are configuring the integration with Workday implementation tenant, note the scheduled downtime hours of your Workday tenant.</span></span> <span data-ttu-id="98dda-112">Ngày làm việc đã lên lịch đã lên lịch cho người thuê thực thi của mình qua các ngày cuối tuần (thường là từ tối thứ sáu đến buổi sáng thứ bảy) và lỗi kết nối trong cửa sổ downtime này là một vấn đề đã biết tự động giải quyết ngay khi các thuê bao triển khai đang trở lại trực tuyến.</span><span class="sxs-lookup"><span data-stu-id="98dda-112">Workday has scheduled down time for its implementation tenants over weekends (usually from Friday evening to Saturday morning) and connectivity failures during this downtime window is a known issue that auto-resolves as soon as the implementation tenants are back online.</span></span>
5. <span data-ttu-id="98dda-113">Trong các trường hợp hiếm, bạn cũng có thể thấy lỗi này nếu mật khẩu của người dùng hệ thống tích hợp đã thay đổi do làm mới của đối tượng thuê hoặc nếu tài khoản trong trạng thái bị khóa hoặc đã hết hạn.</span><span class="sxs-lookup"><span data-stu-id="98dda-113">In rare cases, you may also see this error if the password of the Integration System User changed due to tenant refresh or if the account is in locked or expired state.</span></span> <span data-ttu-id="98dda-114">Vui lòng kiểm tra trạng thái của người dùng hệ thống tích hợp với người quản trị ngày làm việc của bạn.</span><span class="sxs-lookup"><span data-stu-id="98dda-114">Please check the status of the Integration System user with your Workday administrator.</span></span>

<span data-ttu-id="98dda-115">Để biết thêm chi tiết về cách đặt cấu hình ngày làm việc cho tính năng cung cấp tự động, hãy xem [hướng dẫn: cấu hình ngày làm việc cho người dùng tự động cung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)cấp.</span><span class="sxs-lookup"><span data-stu-id="98dda-115">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>
