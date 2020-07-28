---
title: Apple MDM Push Certificate chưa được thiết lập
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2634"
- "9000770"
ms.openlocfilehash: 5888eeb9b1dfde0b1ac5e7569f00d812e3d9d1bb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "45440005"
---
# <a name="apple-mdm-push-certificate-has-not-been-set-up"></a><span data-ttu-id="5407e-102">Apple MDM Push Certificate chưa được thiết lập</span><span class="sxs-lookup"><span data-stu-id="5407e-102">Apple MDM Push Certificate has not been set up</span></span>

<span data-ttu-id="5407e-103">Apple MDM Push Certificate (còn được gọi là chứng chỉ Apple Push Notification Service (APNS)) chưa được cấu hình cho đăng ký của bạn.</span><span class="sxs-lookup"><span data-stu-id="5407e-103">An Apple MDM Push Certificate (also known as an Apple Push Notification Service (APNS) certificate) has not been configured for your subscription.</span></span> <span data-ttu-id="5407e-104">Nếu không có một Apple MDM Push Certificate cấu hình, bạn không thể đăng ký và quản lý các thiết bị iOS và Mac OS.</span><span class="sxs-lookup"><span data-stu-id="5407e-104">Without an Apple MDM Push Certificate configured, you are unable to enroll and manage iOS and Mac OS devices.</span></span> <span data-ttu-id="5407e-105">Sau khi bạn thêm chứng chỉ dành cho InTune, người dùng có thể cài đặt ứng dụng cổng thông tin công ty để đăng ký thiết bị iOS của họ.</span><span class="sxs-lookup"><span data-stu-id="5407e-105">After you add the certificate to Intune, users can install the Company Portal app to enroll their iOS devices.</span></span>

1. <span data-ttu-id="5407e-106">Chọn **"Tôi đồng ý".**</span><span class="sxs-lookup"><span data-stu-id="5407e-106">Select **"I agree."**</span></span> <span data-ttu-id="5407e-107">để cho phép Microsoft gửi dữ liệu đến Apple.</span><span class="sxs-lookup"><span data-stu-id="5407e-107">to give Microsoft permission to send data to Apple.</span></span>

2. <span data-ttu-id="5407e-108">Chọn **tải xuống CSR của bạn** yêu cầu đăng ký chứng chỉ cần thiết để tạo một Apple MDM đẩy chứng chỉ.</span><span class="sxs-lookup"><span data-stu-id="5407e-108">Select **Download your CSR** the Intune certificate signing request required to create an Apple MDM push certificate.</span></span> <span data-ttu-id="5407e-109">Tệp được sử dụng để yêu cầu chứng chỉ mối quan hệ tin cậy từ cổng của Apple Push Certificate.</span><span class="sxs-lookup"><span data-stu-id="5407e-109">The file is used to request a trust relationship certificate from the Apple Push Certificates Portal.</span></span>

3. <span data-ttu-id="5407e-110">Chọn **tạo chứng chỉ đẩy MDM của bạn** để đi đến cổng thông tin chứng chỉ Push của Apple.</span><span class="sxs-lookup"><span data-stu-id="5407e-110">Select **Create your MDM push Certificate** to go to the Apple Push Certificates Portal.</span></span> <span data-ttu-id="5407e-111">Đăng nhập bằng ID Apple của công ty, sau đó chọn **tạo chứng chỉ**.</span><span class="sxs-lookup"><span data-stu-id="5407e-111">Sign in with your company Apple ID, and then select **Create a Certificate**.</span></span> <span data-ttu-id="5407e-112">Chọn **chọn tệp**, duyệt đến tệp yêu cầu ký chứng chỉ và sau đó chọn **tải lên**.</span><span class="sxs-lookup"><span data-stu-id="5407e-112">Select **Choose File**, browse to the certificate signing request file, and then choose **Upload**.</span></span> <span data-ttu-id="5407e-113">Trên trang xác nhận, chọn **tải xuống** để tải xuống tệp chứng chỉ (. pem) và lưu tệp cục bộ.</span><span class="sxs-lookup"><span data-stu-id="5407e-113">On the Confirmation page, choose **Download** to download the certificate (.pem) file, and save the file locally.</span></span>
 
<span data-ttu-id="5407e-114">**Lưu ý**: chứng chỉ được liên kết với Apple ID được sử dụng để tạo ra nó.</span><span class="sxs-lookup"><span data-stu-id="5407e-114">**Note**: The certificate is associated with the Apple ID used to create it.</span></span> <span data-ttu-id="5407e-115">Để thực hành tốt nhất, hãy sử dụng Apple ID của công ty cho các tác vụ quản lý và đảm bảo rằng hộp thư được giám sát bởi nhiều người hoặc bằng cách sử dụng danh sách phân phối.</span><span class="sxs-lookup"><span data-stu-id="5407e-115">As a best practice, use a company Apple ID for management tasks, and make sure the mailbox is monitored by more than one person or by using a distribution list.</span></span> <span data-ttu-id="5407e-116">Không bao giờ sử dụng ID Apple cá nhân.</span><span class="sxs-lookup"><span data-stu-id="5407e-116">Never use a personal Apple ID.</span></span> <span data-ttu-id="5407e-117">Sử dụng cùng một Apple ID để gia hạn giấy chứng nhận của Apple Push Certificate mỗi 12 tháng.</span><span class="sxs-lookup"><span data-stu-id="5407e-117">Use the same Apple ID to renew the Apple Push Certificate every 12 months.</span></span>
 
4. <span data-ttu-id="5407e-118">Nhập Apple ID được sử dụng để tạo giấy chứng nhận đẩy Apple MDM của bạn.</span><span class="sxs-lookup"><span data-stu-id="5407e-118">Enter the Apple ID used to create your Apple MDM push certificate.</span></span> <span data-ttu-id="5407e-119">Ghi lại ID này như một lời nhắc nhở khi bạn cần gia hạn chứng chỉ.</span><span class="sxs-lookup"><span data-stu-id="5407e-119">Record this ID as a reminder for when you need to renew the certificate.</span></span>

5. <span data-ttu-id="5407e-120">Đi tới tệp chứng chỉ (. pem), chọn **mở**, sau đó chọn **tải lên**.</span><span class="sxs-lookup"><span data-stu-id="5407e-120">Go to the certificate (.pem) file, choose **Open**, and then choose **Upload**.</span></span> <span data-ttu-id="5407e-121">Với giấy chứng nhận đẩy, InTune có thể đăng ký và quản lý các thiết bị của Apple.</span><span class="sxs-lookup"><span data-stu-id="5407e-121">With the push certificate, Intune can enroll and manage Apple devices.</span></span>