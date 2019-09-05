---
title: Điều khoản thiếu từ SharePoint Online Term Store
ms.author: pebaum
author: Techwriter40
ms.date: 10/30/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 0f9efe980987c9ffc64fcf9d5d72a67f0a622867
ms.sourcegitcommit: 23772ebd25a86a879ced40b10566a35e76a79eb5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/05/2019
ms.locfileid: "36762103"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="405b3-102">Cho phép mã hóa BitLocker với InTune</span><span class="sxs-lookup"><span data-stu-id="405b3-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="405b3-103">InTune Endpoint Protection chính sách có thể được sử dụng để cấu hình thiết đặt mã hóa Boitlocker cho các thiết bị Windows như được mô tả trong: Windows10 (và sau đó) cài đặt để bảo vệ thiết bị bằng cách sử dụng InTune</span><span class="sxs-lookup"><span data-stu-id="405b3-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="405b3-104">Bạn nên biết rằng nhiều thiết bị mới chạy Windows 10 hỗ trợ mã hóa BitLocker tự động được kích hoạt mà không có ứng dụng chính sách MDM.</span><span class="sxs-lookup"><span data-stu-id="405b3-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="405b3-105">Điều này có thể ảnh hưởng đến áp dụng chính sách nếu không cài đặt mặc định được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="405b3-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="405b3-106">Xem FAQ để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="405b3-106">See FAQ for more detail.</span></span>


<span data-ttu-id="405b3-107">Câu  hỏi thường gặp Q: Phiên bản nào của Windows hỗ trợ mã hóa thiết bị bằng cách sử dụng chính sách bảo vệ điểm cuối?</span><span class="sxs-lookup"><span data-stu-id="405b3-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="405b3-108"> A: cài đặt trong chính sách InTune Endpoint Protection được thực hiện bằng cách sử dụng CSP BitLocker.</span><span class="sxs-lookup"><span data-stu-id="405b3-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="405b3-109">Không phải tất cả các phiên bản cũng không xây dựng Windows hỗ trợ CSP BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="405b3-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="405b3-110">Tại thời gian này phiên bản Windows: Enterprise; Giáo dục, di động, doanh nghiệp di động và chuyên nghiệp (từ xây dựng 1809 trở đi) được hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="405b3-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="405b3-111">Câu hỏi: nếu thiết bị đã được mã hóa bằng BitLocker bằng cách sử dụng các thiết lập mặc định của hệ điều hành cho phương pháp mã hóa và cường độ (XTS-AES-128) sẽ áp dụng một chính sách với các cài đặt khác nhau tự động kích hoạt mã hóa lại ổ đĩa với các thiết đặt mới?</span><span class="sxs-lookup"><span data-stu-id="405b3-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="405b3-112">A: không.</span><span class="sxs-lookup"><span data-stu-id="405b3-112">A: No.</span></span> <span data-ttu-id="405b3-113">Để áp dụng các thiết lập mật mã mới, ổ đĩa đầu tiên phải được giải mã.</span><span class="sxs-lookup"><span data-stu-id="405b3-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="405b3-114">Lưu ý đối với các thiết bị được đăng ký với Autopilot mã hóa tự động sẽ xảy ra trong OOBE không được kích hoạt cho đến khi chính sách InTune được đánh giá cho phép chính sách dựa trên cài đặt được sử dụng ở nơi mặc định hệ điều hành</span><span class="sxs-lookup"><span data-stu-id="405b3-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="405b3-115">Câu hỏi: nếu thiết bị được mã hóa do ứng dụng chính sách InTune sẽ được giải mã khi chính sách đó bị xóa?</span><span class="sxs-lookup"><span data-stu-id="405b3-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="405b3-116">A: loại bỏ chính sách liên quan đến mã hóa không dẫn đến giải mã các ổ đĩa được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="405b3-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="405b3-117">Câu hỏi: tại sao chính sách tuân thủ dành cho thấy rằng thiết bị của tôi không có "đã bật BitLocker" nhưng?</span><span class="sxs-lookup"><span data-stu-id="405b3-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="405b3-118">A: cài đặt "bật BitLocker" trong chính sách tuân thủ InTune sử dụng máy khách chứng thực sự cố Windows Device (DHA).</span><span class="sxs-lookup"><span data-stu-id="405b3-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="405b3-119">Máy khách này chỉ đo trạng thái thiết bị vào thời gian khởi động.</span><span class="sxs-lookup"><span data-stu-id="405b3-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="405b3-120">Vì vậy, nếu một thiết bị không được khởi động lại kể từ khi mã hóa BitLocker đã hoàn thành dịch vụ khách hàng DHA sẽ không báo cáo BitLocker đang hoạt động.</span><span class="sxs-lookup"><span data-stu-id="405b3-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>