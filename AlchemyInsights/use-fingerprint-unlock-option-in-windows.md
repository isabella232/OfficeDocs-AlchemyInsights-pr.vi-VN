---
title: Sử dụng tùy chọn mở khóa dấu vân tay trong Windows 10
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
- "9001689"
- "3765"
ms.openlocfilehash: 99f037f62748c06d77b526e35f67b711885c4a1e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47795266"
---
# <a name="use-fingerprint-unlock-option-in-windows-10"></a><span data-ttu-id="2a79b-102">Sử dụng tùy chọn mở khóa dấu vân tay trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="2a79b-102">Use fingerprint unlock option in Windows 10</span></span>

<span data-ttu-id="2a79b-103">**Bật dấu vân tay của Windows Xin chào**</span><span class="sxs-lookup"><span data-stu-id="2a79b-103">**Enable Windows Hello Fingerprint**</span></span>

<span data-ttu-id="2a79b-104">Để mở khóa Windows 10 bằng dấu vân tay của bạn, bạn cần phải thiết lập Windows Hello dấu vân tay bằng cách thêm (cho phép Windows tìm hiểu để nhận dạng) ít nhất một ngón tay.</span><span class="sxs-lookup"><span data-stu-id="2a79b-104">To unlock Windows 10 using your fingerprint, you need to set up Windows Hello Fingerprint by adding (letting Windows learn to recognize) at least one finger.</span></span> 

1. <span data-ttu-id="2a79b-105">Đi đến **cài đặt > tài khoản > các tùy chọn đăng nhập** (hoặc bấm vào [đây](ms-settings:signinoptions?activationSource=GetHelp)).</span><span class="sxs-lookup"><span data-stu-id="2a79b-105">Go to **Settings  > Accounts > Sign-in options** (or click [here](ms-settings:signinoptions?activationSource=GetHelp)).</span></span> <span data-ttu-id="2a79b-106">Các tùy chọn đăng nhập sẵn dùng sẽ được liệt kê.</span><span class="sxs-lookup"><span data-stu-id="2a79b-106">Available sign-in options will be listed.</span></span> <span data-ttu-id="2a79b-107">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="2a79b-107">For example:</span></span>

    ![Các tùy chọn đăng nhập.](media/sign-in-options.png)

2. <span data-ttu-id="2a79b-109">Bấm hoặc nhấn vào dấu **vân tay của Windows Hello**, sau đó bấm **thiết lập**.</span><span class="sxs-lookup"><span data-stu-id="2a79b-109">Click or tap **Windows Hello Fingerprint**, then click **Set up**.</span></span> <span data-ttu-id="2a79b-110">Trong cửa sổ thiết lập Hello của Windows, bấm **bắt đầu**.</span><span class="sxs-lookup"><span data-stu-id="2a79b-110">In the Windows Hello setup window, click **Get started**.</span></span> <span data-ttu-id="2a79b-111">Cảm biến dấu vân tay sẽ kích hoạt và bạn sẽ được yêu cầu đặt ngón tay của bạn trên bộ cảm biến:</span><span class="sxs-lookup"><span data-stu-id="2a79b-111">The fingerprint sensor will activate, and you'll be asked to place your finger on the sensor:</span></span>

   ![Cảm biến dấu vân tay.](media/fingerprint-sensor.png)

3. <span data-ttu-id="2a79b-113">Làm theo các hướng dẫn, mà sẽ yêu cầu bạn liên tục quét ngón tay của bạn.</span><span class="sxs-lookup"><span data-stu-id="2a79b-113">Follow the instructions, which will ask you to repeatedly scan your finger.</span></span> <span data-ttu-id="2a79b-114">Khi hoàn tất, bạn sẽ có tùy chọn thêm các ngón tay khác mà bạn có thể muốn sử dụng để đăng nhập.</span><span class="sxs-lookup"><span data-stu-id="2a79b-114">When this is finished, you'll have the option of adding other fingers you may want to use for sign-in.</span></span> <span data-ttu-id="2a79b-115">Lần sau khi bạn đăng nhập vào Windows 10, bạn sẽ có tùy chọn sử dụng dấu vân tay để làm như vậy.</span><span class="sxs-lookup"><span data-stu-id="2a79b-115">Next time you sign in to Windows 10, you will have the option of using your fingerprint to do so.</span></span>

<span data-ttu-id="2a79b-116">**Dấu vân tay của Windows Xin chào không sẵn dùng như một tùy chọn đăng nhập**</span><span class="sxs-lookup"><span data-stu-id="2a79b-116">**Windows Hello Fingerprint not available as a sign-in option**</span></span>

<span data-ttu-id="2a79b-117">Nếu Windows Xin chào dấu vân tay không được hiển thị như là một tùy chọn trong **tùy chọn đăng nhập**, nó nghĩa là Windows không biết về bất kỳ bộ đọc dấu vân tay/máy quét nào được đính kèm với PC của bạn hoặc chính sách hệ thống sẽ ngăn không cho sử dụng của bạn (nếu ví dụ máy tính của bạn được quản lý bởi nơi làm việc của bạn).</span><span class="sxs-lookup"><span data-stu-id="2a79b-117">If Windows Hello Fingerprint is not shown as an option in **Sign-in options**, it means Windows is not aware of any fingerprint reader/scanner attached to your PC, or that a system policy prevents its use (if for example your PC is managed by your workplace).</span></span> <span data-ttu-id="2a79b-118">Để khắc phục sự cố:</span><span class="sxs-lookup"><span data-stu-id="2a79b-118">To troubleshoot:</span></span> 

1. <span data-ttu-id="2a79b-119">Chọn nút **bắt đầu** trong thanh tác vụ và tìm kiếm **trình quản lý thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="2a79b-119">Select the **Start** button in the Taskbar and search for **Device Manager**.</span></span>

2. <span data-ttu-id="2a79b-120">Bấm hoặc gõ nhẹ để mở **trình quản lý thiết bị**.</span><span class="sxs-lookup"><span data-stu-id="2a79b-120">Click or tap to open **Device Manager**.</span></span>

3. <span data-ttu-id="2a79b-121">Trong trình quản lý thiết bị, hãy bung rộng thiết bị sinh trắc học bằng cách bấm vào Chevron của nó.</span><span class="sxs-lookup"><span data-stu-id="2a79b-121">In Device Manager, expand Biometric devices by clicking its chevron.</span></span>

   ![Thiết bị sinh trắc học.](media/biometric-devices.png)

4. <span data-ttu-id="2a79b-123">Máy quét dấu vân tay của bạn sẽ được liệt kê dưới dạng thiết bị sinh trắc học, chẳng hạn như máy quét máy tính Synapdi WBTICS:</span><span class="sxs-lookup"><span data-stu-id="2a79b-123">Your fingerprint scanner should be listed as a biometric device, such as the Synaptics WBDI scanner:</span></span>

   ![Thiết bị sinh trắc học.](media/biometric-devices-expanded.png)

5. <span data-ttu-id="2a79b-125">Nếu máy quét dấu vân tay của bạn không được hiển thị và máy quét được tích hợp vào PC của bạn, hãy đi đến trang web của nhà sản xuất PC.</span><span class="sxs-lookup"><span data-stu-id="2a79b-125">If your fingerprint scanner is not shown, and the scanner is integrated into your PC, go to the PC manufacturer's website.</span></span> <span data-ttu-id="2a79b-126">Trong phần hỗ trợ kỹ thuật cho mô hình PC của bạn, hãy tìm kiếm một trình điều khiển Windows 10 cho một máy quét mà bạn có thể cài đặt.</span><span class="sxs-lookup"><span data-stu-id="2a79b-126">In the technical support section for your PC model, search for a Windows 10 driver for a scanner that you can install.</span></span>

6. <span data-ttu-id="2a79b-127">Nếu máy quét tách riêng ra khỏi PC (được đính kèm qua USB), hãy đi đến trang web của nhà sản xuất máy quét để tìm và cài đặt phần mềm trình điều khiển thiết bị chạy Windows 10 cho mô hình máy quét mà bạn có.</span><span class="sxs-lookup"><span data-stu-id="2a79b-127">If the scanner is separate from the PC (attached via USB), go to the scanner manufacturer's website to find and install Windows 10 device driver software for the scanner model you have.</span></span>
