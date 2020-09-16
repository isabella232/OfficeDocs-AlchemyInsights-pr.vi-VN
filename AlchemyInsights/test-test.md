---
title: Các thuật ngữ bị thiếu trong lưu trữ thuật ngữ SharePoint Online
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1243"
- "5200021"
ms.openlocfilehash: 06711c289365c0fcdf71cf9cccf3cfc53511495a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47750473"
---
# <a name="enabling-bitlocker-encryption-with-intune"></a><span data-ttu-id="c4709-102">Bật tính năng mã hóa BitLocker bằng InTune</span><span class="sxs-lookup"><span data-stu-id="c4709-102">Enabling Bitlocker Encryption with Intune</span></span>

<span data-ttu-id="c4709-103">Có thể sử dụng chính sách bảo vệ Endpoint trong InTune để cấu hình thiết đặt mã hóa Boitlocker cho các thiết bị Windows như được mô tả trong: Windows10 (và phiên sau) để bảo vệ các thiết bị bằng cách dùng InTune</span><span class="sxs-lookup"><span data-stu-id="c4709-103">Intune Endpoint Protection Policy can be used to configure Boitlocker encryption settings for Windows devices as described in : Windows10 (and later) settings to protect devices using Intune</span></span>

<span data-ttu-id="c4709-104">Bạn nên lưu ý rằng nhiều thiết bị mới chạy Windows 10 hỗ trợ mã hóa BitLocker tự động được kích hoạt mà không cần áp dụng chính sách MDM.</span><span class="sxs-lookup"><span data-stu-id="c4709-104">You should be aware that many newer devices running Windows 10 support automatic bitlocker encryption which is triggered without the application of MDM policy.</span></span> <span data-ttu-id="c4709-105">Việc này có thể tác động đến ứng dụng chính sách nếu thiết đặt mặc định không được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="c4709-105">This may impact application of policy if non default settings are configured.</span></span> <span data-ttu-id="c4709-106">Xem câu hỏi thường gặp về chi tiết hơn.</span><span class="sxs-lookup"><span data-stu-id="c4709-106">See FAQ for more detail.</span></span>


<span data-ttu-id="c4709-107">Câu hỏi thường gặp   hỏi: Phiên bản nào của mã hóa thiết bị hỗ trợ Windows bằng chính sách bảo vệ điểm cuối?</span><span class="sxs-lookup"><span data-stu-id="c4709-107">FAQ  Q: Which editions of Windows support device encryption using the Endpoint Protection Policy?</span></span>
<span data-ttu-id="c4709-108"> A: các thiết đặt trong chính sách bảo vệ điểm cuối trong InTune được thực hiện bằng cách sử dụng CPC BitLocker.</span><span class="sxs-lookup"><span data-stu-id="c4709-108"> A: The settings in Intune Endpoint Protection Policy  are implemented using the Bitlocker CSP.</span></span><span data-ttu-id="c4709-109">Không phải tất cả các phiên bản cũng không phải là bản dựng của Windows hỗ trợ CPC BitLocker. 
     </span><span class="sxs-lookup"><span data-stu-id="c4709-109">  Not all editions nor builds of Windows support the Bitlocker CSP. 
     </span></span> <span data-ttu-id="c4709-110">Tại phiên bản Windows thời gian này: Enterprise; Giáo dục, di động, doanh nghiệp di động và chuyên nghiệp (từ bản dựng 1809 trở đi) được hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="c4709-110">At this time Windows Editions: Enterprise; Education, Mobile, Mobile Enterprise and Professional (from build 1809 onwards) are supported.</span></span>




<span data-ttu-id="c4709-111">Hỏi: nếu thiết bị đã được mã hóa với BitLocker bằng cách dùng thiết đặt mặc định của hệ điều hành cho phương pháp mã hóa và sức mạnh của mật độ (XTS-AES-128) sẽ áp dụng chính sách với các thiết đặt khác nhau sẽ tự động kích hoạt lại mã hóa ổ đĩa với cài đặt mới?</span><span class="sxs-lookup"><span data-stu-id="c4709-111">Q: If a device is already encrypted with Bitlocker using the OS default settings for encryption method and cipher strength (XTS-AES-128)  will applying a policy with different settings automatically trigger re-encryption of the drive with the new settings?</span></span>

<span data-ttu-id="c4709-112">A: không.</span><span class="sxs-lookup"><span data-stu-id="c4709-112">A: No.</span></span> <span data-ttu-id="c4709-113">Để áp dụng các thiết đặt mã hóa mới, trước tiên, bạn phải được giải mã.</span><span class="sxs-lookup"><span data-stu-id="c4709-113">In order to apply the new cipher settings the drive must first be decrypted.</span></span>

<span data-ttu-id="c4709-114">Lưu ý đối với các thiết bị đang được đăng ký với Autopilot mã hóa tự động sẽ xảy ra trong khi OOBE không được kích hoạt cho đến khi chính sách InTune được đánh giá cho phép các thiết đặt dựa trên chính sách sẽ được sử dụng thay cho mặc định của hệ điều hành</span><span class="sxs-lookup"><span data-stu-id="c4709-114">Note For devices being enrolled with Autopilot the automatic encryption that would occur during OOBE is not triggered until Intune policy is evaluated which allows the policy based settings to be used in place of the OS defaults</span></span>




<span data-ttu-id="c4709-115">Hỏi nếu thiết bị được mã hóa là kết quả của việc áp dụng chính sách InTune sẽ được giải mã khi chính sách đó bị loại bỏ?</span><span class="sxs-lookup"><span data-stu-id="c4709-115">Q If a device is encrypted as a result of the  application of Intune policy will it be decrypted when that policy is removed?</span></span>

<span data-ttu-id="c4709-116">A: loại bỏ chính sách liên quan đến mã hóa không dẫn đến việc giải mã các ổ đĩa được cấu hình.</span><span class="sxs-lookup"><span data-stu-id="c4709-116">A: Removal of encryption related policy does NOT result in decryption of the drives which were configured.</span></span>




<span data-ttu-id="c4709-117">Hỏi: tại sao không điều chỉnh chính sách tuân thủ cho biết thiết bị của tôi không có "BitLocker đã bật" nhưng nó là gì?</span><span class="sxs-lookup"><span data-stu-id="c4709-117">Q: Why does intune Compliance policy show that my device does not have "Bitlocker Enabled" but it is?</span></span>

<span data-ttu-id="c4709-118">A: thiết đặt "BitLocker Enabled" trong chính sách tuân thủ InTune sẽ sử dụng máy khách Attestation (DHA) của thiết bị Windows (DHA).</span><span class="sxs-lookup"><span data-stu-id="c4709-118">A: The "Bitlocker enabled" setting in intune compliance policy utilizes the Windows Device Health Attestation  (DHA) client.</span></span> <span data-ttu-id="c4709-119">Máy khách này chỉ đo trạng thái thiết bị tại thời điểm khởi động.</span><span class="sxs-lookup"><span data-stu-id="c4709-119">This client only measures device state at boot time.</span></span> <span data-ttu-id="c4709-120">Vì vậy, nếu thiết bị không được khởi động lại từ khi mã hóa BitLocker đã hoàn tất dịch vụ máy khách DHA sẽ không báo cáo BitLocker khi đang hiện hoạt.</span><span class="sxs-lookup"><span data-stu-id="c4709-120">So if a device has not been rebooted since bitlocker encryption was completed the DHA client service will not report bitlocker as being active.</span></span>