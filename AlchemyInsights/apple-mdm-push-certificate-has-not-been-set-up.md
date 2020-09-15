---
title: Chứng chỉ đẩy táo MDM đã không được thiết lập
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5f95c9bee29db44a4153e0de0b8f6fb49b274920
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47716879"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="f524d-102">Chứng chỉ đẩy táo MDM đã không được thiết lập</span><span class="sxs-lookup"><span data-stu-id="f524d-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="f524d-103">Chứng chỉ đẩy của Apple MDM (còn được gọi là chứng chỉ dịch vụ thông báo đẩy táo) chưa được cấu hình cho đăng ký của bạn.</span><span class="sxs-lookup"><span data-stu-id="f524d-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="f524d-104">Nếu không có giấy chứng nhận đẩy táo MDM được cấu hình, bạn sẽ không thể đăng ký và quản lý các thiết bị chạy iOS và Mac OS.</span><span class="sxs-lookup"><span data-stu-id="f524d-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="f524d-105">Sau khi bạn thêm chứng chỉ vào InTune, người dùng có thể cài đặt ứng dụng cổng thông tin công ty để đăng ký thiết bị iOS của họ.</span><span class="sxs-lookup"><span data-stu-id="f524d-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="f524d-106">Chọn **"Tôi đồng ý".**</span><span class="sxs-lookup"><span data-stu-id="f524d-106">Select **"I agree."**</span></span> <span data-ttu-id="f524d-107">để cấp quyền cho Microsoft để gửi dữ liệu sang Apple.</span><span class="sxs-lookup"><span data-stu-id="f524d-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="f524d-108">Chọn **tải xuống** yêu cầu đăng nhập chứng chỉ không điều chỉnh của bạn được yêu cầu để tạo chứng chỉ đẩy MDM của Apple.</span><span class="sxs-lookup"><span data-stu-id="f524d-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="f524d-109">Tệp được dùng để yêu cầu chứng chỉ mối quan hệ tin cậy từ cổng thông tin chứng chỉ đẩy táo.</span><span class="sxs-lookup"><span data-stu-id="f524d-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="f524d-110">Chọn **tạo chứng chỉ đẩy MDM của bạn** để đi đến cổng thông tin chứng chỉ Push của Apple.</span><span class="sxs-lookup"><span data-stu-id="f524d-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="f524d-111">Đăng nhập bằng ID Apple của công ty bạn, rồi chọn **tạo chứng chỉ**.</span><span class="sxs-lookup"><span data-stu-id="f524d-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="f524d-112">Chọn **chọn tệp**, duyệt đến tệp yêu cầu ký chứng chỉ, rồi chọn **tải lên**.</span><span class="sxs-lookup"><span data-stu-id="f524d-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="f524d-113">Trên trang xác nhận, chọn **tải xuống** để tải xuống tệp chứng chỉ (. pem) và lưu tệp cục bộ.</span><span class="sxs-lookup"><span data-stu-id="f524d-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="f524d-114">**Lưu ý**: chứng chỉ được liên kết với Apple ID được sử dụng để tạo ra.</span><span class="sxs-lookup"><span data-stu-id="f524d-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="f524d-115">Với tư cách là tốt nhất, hãy sử dụng một công ty Apple ID cho các tác vụ quản lý và đảm bảo rằng hộp thư được theo dõi bởi nhiều người hoặc bằng cách sử dụng danh sách phân phối.</span><span class="sxs-lookup"><span data-stu-id="f524d-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="f524d-116">Không bao giờ sử dụng ID cá nhân của Apple.</span><span class="sxs-lookup"><span data-stu-id="f524d-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="f524d-117">Sử dụng cùng một ID Apple để gia hạn chứng chỉ đẩy táo mỗi 12 tháng.</span><span class="sxs-lookup"><span data-stu-id="f524d-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="f524d-118">Nhập Apple ID được dùng để tạo chứng chỉ đẩy MDM táo của bạn.</span><span class="sxs-lookup"><span data-stu-id="f524d-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="f524d-119">Ghi lại ID này làm lời nhắc khi bạn cần gia hạn chứng chỉ.</span><span class="sxs-lookup"><span data-stu-id="f524d-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="f524d-120">Đi đến tệp chứng chỉ (. pem), chọn **mở**, rồi chọn **tải lên**.</span><span class="sxs-lookup"><span data-stu-id="f524d-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="f524d-121">Với chứng chỉ đẩy, InTune có thể đăng ký và quản lý các thiết bị của Apple.</span><span class="sxs-lookup"><span data-stu-id="f524d-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>