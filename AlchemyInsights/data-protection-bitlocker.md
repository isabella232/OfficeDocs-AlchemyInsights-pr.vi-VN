---
title: DataProtection-BitLocker
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1802"
- "9000220"
ms.openlocfilehash: ab28162fcdf0a37060be3bdf15a78aceca7a48b1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47731261"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="cee4b-102">Bật tính năng mã hóa BitLocker bằng InTune</span><span class="sxs-lookup"><span data-stu-id="cee4b-102">Enabling Bitlocker encryption with Intune</span></span>

 <span data-ttu-id="cee4b-103">Có thể sử dụng chính sách bảo vệ Endpoint trong InTune để cấu hình thiết đặt mã hóa BitLocker cho các thiết bị chạy Windows.</span><span class="sxs-lookup"><span data-stu-id="cee4b-103">Intune Endpoint Protection Policy can be used to configure Bitlocker encryption settings for Windows devices.</span></span> <span data-ttu-id="cee4b-104">Để biết thêm thông tin, hãy xem [thiết đặt Windows 10 (và mới hơn) để bảo vệ các thiết bị bằng cách dùng InTune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span><span class="sxs-lookup"><span data-stu-id="cee4b-104">For more information, see [Windows 10 (and later) settings to protect devices using Intune](https://docs.microsoft.com/intune/endpoint-protection-windows-10#windows-encryption).</span></span>
 
<span data-ttu-id="cee4b-105">Bạn nên lưu ý rằng nhiều thiết bị mới chạy Windows 10 hỗ trợ mã hóa BitLocker tự động, được kích hoạt mà không có ứng dụng của chính sách MDM.</span><span class="sxs-lookup"><span data-stu-id="cee4b-105">You should be aware that many newer devices running Windows 10 support automatic Bitlocker encryption, which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="cee4b-106">Điều này có thể tác động đến ứng dụng chính sách nếu thiết đặt không phải mặc định được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="cee4b-106">This may impact application of policy if non-default settings are configured.</span></span> <span data-ttu-id="cee4b-107">Xem câu hỏi thường gặp sau đây để biết thêm chi tiết.</span><span class="sxs-lookup"><span data-stu-id="cee4b-107">See the following FAQ for more detail.</span></span>
 
<span data-ttu-id="cee4b-108">Để biết thông tin về khắc phục sự cố BitLocker, hãy xem [khắc phục sự cố chính sách BitLocker trong Microsoft InTune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span><span class="sxs-lookup"><span data-stu-id="cee4b-108">For information about troubleshooting bitlocker issues, see [Troubleshoot BitLocker policies in Microsoft Intune](https://docs.microsoft.com/intune/protect/troubleshoot-bitlocker-policies).</span></span>
 
 
<span data-ttu-id="cee4b-109">**DIỄN**</span><span class="sxs-lookup"><span data-stu-id="cee4b-109">**FAQ**</span></span>

 <span data-ttu-id="cee4b-110">Hỏi: Phiên bản nào của mã hóa thiết bị hỗ trợ Windows sử dụng chính sách bảo vệ điểm cuối?</span><span class="sxs-lookup"><span data-stu-id="cee4b-110">Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span><br>
 <span data-ttu-id="cee4b-111">A: các thiết đặt trong chính sách bảo vệ điểm cuối trong InTune được thực hiện bằng cách sử dụng [CPC BitLocker](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span><span class="sxs-lookup"><span data-stu-id="cee4b-111">A: The settings in Intune Endpoint Protection Policy  are implemented using the [Bitlocker CSP](https://docs.microsoft.com/windows/client-management/mdm/bitlocker-csp).</span></span> <span data-ttu-id="cee4b-112">Không phải tất cả các phiên bản hoặc bản dựng của Windows hỗ trợ CPC BitLocker.</span><span class="sxs-lookup"><span data-stu-id="cee4b-112">Not all editions or builds of Windows support the Bitlocker CSP.</span></span> <br><br>
      <span data-ttu-id="cee4b-113">Tại thời điểm này, các phiên bản Windows sau đây được hỗ trợ: Enterprise, Education, Mobile, Enterprise và Professional (bản dựng 1809 trở lên).</span><span class="sxs-lookup"><span data-stu-id="cee4b-113">At this time, the following Windows editions are supported: Enterprise, Education, Mobile, Mobile Enterprise, and Professional (build 1809 and later).</span></span>
 
<span data-ttu-id="cee4b-114">Hỏi: nếu thiết bị đã được mã hóa với BitLocker bằng cách dùng thiết đặt mặc định của hệ điều hành cho phương pháp mã hóa và sức mạnh của mật độ (XTS-AES-128), sẽ áp dụng chính sách với các thiết đặt khác nhau sẽ tự động kích hoạt lại mã hóa ổ đĩa với cài đặt mới?</span><span class="sxs-lookup"><span data-stu-id="cee4b-114">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128), will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span><br>
<span data-ttu-id="cee4b-115">A: không.</span><span class="sxs-lookup"><span data-stu-id="cee4b-115">A: No.</span></span> <span data-ttu-id="cee4b-116">Để áp dụng các thiết đặt mã hóa mới, trước tiên, ổ đĩa phải được giải mã.</span><span class="sxs-lookup"><span data-stu-id="cee4b-116">To apply the new cipher settings, the drive must first be decrypted.</span></span><br><br>
<span data-ttu-id="cee4b-117">**Lưu ý:** Đối với các thiết bị đang được đăng ký với Autopilot, mã hóa tự động sẽ xảy ra trong khi OOBE không được kích hoạt cho đến khi chính sách InTune được đánh giá, cho phép các thiết đặt dựa trên chính sách sẽ được sử dụng thay cho mặc định của hệ điều hành.</span><span class="sxs-lookup"><span data-stu-id="cee4b-117">**Note:** For devices being enrolled with Autopilot, the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated, which allows the policy-based settings to be used in place of the OS defaults.</span></span>
 
<span data-ttu-id="cee4b-118">Hỏi: nếu thiết bị được mã hóa là kết quả của việc áp dụng chính sách InTune, nó sẽ được giải mã khi chính sách đó bị loại bỏ?</span><span class="sxs-lookup"><span data-stu-id="cee4b-118">Q: If a device is encrypted as a result of the  application of Intune policy, will it be decrypted when that policy is removed?</span></span><br>
<span data-ttu-id="cee4b-119">A: loại bỏ chính sách liên quan đến mã hóa không dẫn đến việc giải mã các ổ đĩa đã được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="cee4b-119">A: Removal of encryption-related policy does NOT result in decryption of the drives that were configured.</span></span>
 
<span data-ttu-id="cee4b-120">Hỏi: tại sao không điều chỉnh chính sách tuân thủ cho biết thiết bị của tôi không được bật BitLocker, ngay cả khi có hiệu lực đó?</span><span class="sxs-lookup"><span data-stu-id="cee4b-120">Q: Why does Intune Compliance Policy show that my device does not have Bitlocker enabled, even though it is?</span></span><br>
<span data-ttu-id="cee4b-121">A: thiết đặt "BitLocker Enabled" trong chính sách tuân thủ InTune sẽ áp dụng máy khách Attestation (DHA) của thiết bị Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="cee4b-121">A: The "Bitlocker enabled" setting in the Intune Compliance Policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="cee4b-122">Máy khách này chỉ đo trạng thái thiết bị tại thời điểm khởi động.</span><span class="sxs-lookup"><span data-stu-id="cee4b-122">This client only measures device state at boot time.</span></span> <span data-ttu-id="cee4b-123">Vì vậy, nếu thiết bị không được khởi động lại từ khi mã hóa BitLocker đã được hoàn tất, Dịch vụ máy khách DHA sẽ không báo cáo BitLocker khi đang hiện hoạt.</span><span class="sxs-lookup"><span data-stu-id="cee4b-123">So if a device has not been rebooted since Bitlocker encryption was completed, the DHA client service will not report Bitlocker as being active.</span></span>
 
 