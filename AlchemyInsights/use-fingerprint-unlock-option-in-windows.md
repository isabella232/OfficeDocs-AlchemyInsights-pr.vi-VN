---
title: Sử dụng tùy chọn mở khóa vân tay trong Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001689"
- "3765"
ms.openlocfilehash: 8a5059c722c306ad79811140062cec7f52f31766
ms.sourcegitcommit: 00e4266575438f55bdc18db05ed54aafcb75a3c9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42588337"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="86df7-102">Sử dụng tùy chọn mở khóa vân tay trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="86df7-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="86df7-103">**Kích hoạt Windows Hello Fingerprint**</span><span class="sxs-lookup"><span data-stu-id="86df7-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="86df7-104">Để mở khóa Windows 10 bằng vân tay của bạn, bạn cần phải thiết lập Windows Hello Fingerprint bằng cách thêm (cho phép Windows tìm hiểu để nhận dạng) ít nhất một ngón tay.</span><span class="sxs-lookup"><span data-stu-id="86df7-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="86df7-105">Đi tới **cài đặt > tài khoản > tùy chọn đăng nhập** (hoặc bấm vào [đây](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="86df7-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="86df7-106">Các tùy chọn đăng nhập có sẵn sẽ được liệt kê.</span><span class="sxs-lookup"><span data-stu-id="86df7-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="86df7-107">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="86df7-107">For example:</span></span>

    ![Tùy chọn đăng nhập.](media/sign-in-options.png)

2. <span data-ttu-id="86df7-109">Bấm hoặc chạm vào **Windows Hello Fingerprint**, sau đó nhấp vào **thiết lập**.</span><span class="sxs-lookup"><span data-stu-id="86df7-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="86df7-110">Trong cửa sổ thiết lập Windows hello, hãy nhấp vào bắt **đầu**.</span><span class="sxs-lookup"><span data-stu-id="86df7-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="86df7-111">Cảm biến vân tay sẽ kích hoạt và bạn sẽ được yêu cầu để ngón tay lên cảm biến:</span><span class="sxs-lookup"><span data-stu-id="86df7-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Cảm biến vân tay.](media/fingerprint-sensor.png)

3. <span data-ttu-id="86df7-113">Thực hiện theo các hướng dẫn, sẽ yêu cầu bạn liên tục quét ngón tay của bạn.</span><span class="sxs-lookup"><span data-stu-id="86df7-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="86df7-114">Khi điều này kết thúc, bạn sẽ có tùy chọn thêm các ngón tay khác mà bạn có thể muốn sử dụng để đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="86df7-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="86df7-115">Lần tiếp theo bạn đăng nhập vào Windows 10, bạn sẽ có tùy chọn sử dụng vân tay của mình để làm như vậy.</span><span class="sxs-lookup"><span data-stu-id="86df7-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="86df7-116">**Windows Hello Fingerprint không khả dụng dưới dạng tùy chọn đăng nhập**</span><span class="sxs-lookup"><span data-stu-id="86df7-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="86df7-117">Nếu Windows Hello Fingerprint không được hiển thị dưới dạng tùy chọn trong **tùy chọn đăng nhập**, có nghĩa là Windows không biết bất kỳ trình đọc vân tay/máy quét nào được gắn vào máy tính của bạn hoặc chính sách hệ thống sẽ ngăn việc sử dụng nó (ví dụ: PC của bạn được quản lý bởi công sở của bạn).</span><span class="sxs-lookup"><span data-stu-id="86df7-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="86df7-118">Để khắc phục sự cố:</span><span class="sxs-lookup"><span data-stu-id="86df7-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="86df7-119">Chọn nút **bắt đầu** trong thanh tác vụ và tìm kiếm **trình quản lý thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="86df7-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="86df7-120">Nhấp hoặc nhấn để mở **trình quản lý thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="86df7-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="86df7-121">Trong quản lý thiết bị, mở rộng thiết bị sinh trắc học bằng cách nhấp vào Chevron của nó.</span><span class="sxs-lookup"><span data-stu-id="86df7-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Thiết bị sinh trắc học.](media/biometric-devices.png)

4. <span data-ttu-id="86df7-123">Máy quét vân tay của bạn sẽ được liệt kê dưới dạng thiết bị sinh trắc học, chẳng hạn như máy quét Synaptics WBDI:</span><span class="sxs-lookup"><span data-stu-id="86df7-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Thiết bị sinh trắc học.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="86df7-125">Nếu máy quét vân tay của bạn không được hiển thị và máy quét được tích hợp vào PC của bạn, hãy truy cập trang web của nhà sản xuất PC.</span><span class="sxs-lookup"><span data-stu-id="86df7-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="86df7-126">Trong phần hỗ trợ kỹ thuật cho mô hình máy tính của bạn, hãy tìm kiếm trình điều khiển Windows 10 cho máy quét mà bạn có thể cài đặt.</span><span class="sxs-lookup"><span data-stu-id="86df7-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="86df7-127">Nếu máy quét tách biệt với PC (đính kèm qua USB), hãy truy cập trang web của nhà sản xuất máy quét để tìm và cài đặt phần mềm trình điều khiển thiết bị Windows 10 cho mô hình máy quét mà bạn có.</span><span class="sxs-lookup"><span data-stu-id="86df7-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
