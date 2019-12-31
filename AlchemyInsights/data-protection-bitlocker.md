---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: c23a2a2bde240900119382a9c1185a6e02520149
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908731"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="8341a-102">Cho phép mã hóa BitLocker với InTune</span><span class="sxs-lookup"><span data-stu-id="8341a-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="8341a-103">Chính sách bảo vệ điểm cuối InTune có thể được sử dụng để cấu hình cài đặt mã hóa BitLocker cho thiết bị Windows.</span><span class="sxs-lookup"><span data-stu-id="8341a-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="8341a-104">Để biết thêm thông tin, xem [cài đặt Windows 10 (và sau này) để bảo vệ thiết bị bằng cách sử dụng InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="8341a-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="8341a-105">Bạn nên biết rằng nhiều thiết bị mới chạy Windows 10 hỗ trợ mã hóa BitLocker tự động, được kích hoạt mà không có ứng dụng chính sách MDM.</span><span class="sxs-lookup"><span data-stu-id="8341a-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="8341a-106">Điều này có thể ảnh hưởng đến áp dụng chính sách nếu thiết đặt không mặc định được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="8341a-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="8341a-107">Xem FAQ sau đây để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="8341a-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="8341a-108">Để biết thông tin về khắc phục sự cố BitLocker, xem [khắc phục sự cố chính sách BitLocker trong Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="8341a-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="8341a-109">**Faq**</span><span class="sxs-lookup"><span data-stu-id="8341a-109">**FAQ**</span></span>

 <span data-ttu-id="8341a-110">Câu hỏi: Phiên bản nào của Windows hỗ trợ mã hóa thiết bị bằng cách sử dụng chính sách bảo vệ điểm cuối?</span><span class="sxs-lookup"><span data-stu-id="8341a-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="8341a-111">A: cài đặt trong chính sách bảo vệ điểm cuối được thực hiện bằng cách sử dụng [CSP BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="8341a-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="8341a-112">Không phải tất cả các phiên bản hoặc xây dựng Windows hỗ trợ CSP BitLocker.</span><span class="sxs-lookup"><span data-stu-id="8341a-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="8341a-113">Tại thời gian này, các phiên bản Windows sau được hỗ trợ: doanh nghiệp, giáo dục, di động, doanh nghiệp di động và chuyên nghiệp (xây dựng 1809 và mới hơn).</span><span class="sxs-lookup"><span data-stu-id="8341a-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="8341a-114">Câu hỏi: nếu một thiết bị đã được mã hóa bằng BitLocker bằng cách sử dụng các thiết lập mặc định hệ điều hành cho phương pháp mã hóa và cường độ (XTS-AES-128), sẽ áp dụng một chính sách với các cài đặt khác nhau tự động kích hoạt mã hóa lại ổ đĩa với các cài đặt mới?</span><span class="sxs-lookup"><span data-stu-id="8341a-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="8341a-115">A: không.</span><span class="sxs-lookup"><span data-stu-id="8341a-115">A: No.</span></span> <span data-ttu-id="8341a-116">Để áp dụng cài đặt mật mã mới, ổ đĩa trước tiên phải được giải mã.</span><span class="sxs-lookup"><span data-stu-id="8341a-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="8341a-117">**Lưu ý:** Đối với các thiết bị được đăng ký với Autopilot, mã hóa tự động sẽ xảy ra trong OOBE không được kích hoạt cho đến khi chính sách InTune được đánh giá, cho phép các thiết đặt dựa trên chính sách được sử dụng tại chỗ của hệ điều hành mặc định.</span><span class="sxs-lookup"><span data-stu-id="8341a-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="8341a-118">Câu hỏi: nếu thiết bị được mã hóa là kết quả của việc áp dụng chính sách InTune, nó sẽ được giải mã khi chính sách đó bị xóa?</span><span class="sxs-lookup"><span data-stu-id="8341a-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="8341a-119">A: loại bỏ chính sách liên quan đến mã hóa không dẫn đến giải mã ổ đĩa được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="8341a-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="8341a-120">Câu hỏi: tại sao chính sách tuân thủ InTune cho thấy rằng thiết bị của tôi không bật BitLocker, mặc dù nó là?</span><span class="sxs-lookup"><span data-stu-id="8341a-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="8341a-121">A: cài đặt "bật BitLocker" trong chính sách tuân thủ InTune sử dụng máy khách chứng thực tình trạng Windows Device (DHA).</span><span class="sxs-lookup"><span data-stu-id="8341a-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="8341a-122">Máy khách này chỉ đo trạng thái thiết bị vào thời gian khởi động.</span><span class="sxs-lookup"><span data-stu-id="8341a-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="8341a-123">Vì vậy, nếu một thiết bị không được khởi động lại kể từ khi mã hóa BitLocker được hoàn thành, Dịch vụ khách hàng DHA sẽ không báo cáo BitLocker đang hoạt động.</span><span class="sxs-lookup"><span data-stu-id="8341a-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 