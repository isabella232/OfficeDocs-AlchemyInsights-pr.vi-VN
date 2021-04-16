---
title: Mở tệp chỉ đọc
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 39748581-d319-403c-8501-9b785e4a0ed8
ms.custom:
- "765"
- "2200014"
ms.openlocfilehash: e478572ea82e5ea11bac9fd7eacafb833253235d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813206"
---
# <a name="file-open-read-only"></a><span data-ttu-id="18f4c-102">Mở tệp chỉ đọc</span><span class="sxs-lookup"><span data-stu-id="18f4c-102">File open read-only</span></span>

<span data-ttu-id="18f4c-103">Bạn có thể thấy rằng khi mở tệp, chúng sẽ mở dưới dạng chỉ đọc.</span><span class="sxs-lookup"><span data-stu-id="18f4c-103">You may find that when you are opening files, they open as read-only.</span></span> <span data-ttu-id="18f4c-104">Trong một số trường hợp, điều này là để bảo mật thêm, chẳng hạn như khi bạn đang mở tệp từ Internet và các thời điểm khác, có thể là do một thiết đặt có thể thay đổi.</span><span class="sxs-lookup"><span data-stu-id="18f4c-104">In some cases, this is for added security, such as when you are opening files from the internet, and other times, it can be due to a setting that can be changed.</span></span> <span data-ttu-id="18f4c-105">Dưới đây là một số tình huống mà tệp mở ra chỉ đọc và một số bước bạn có thể thực hiện để thay đổi.</span><span class="sxs-lookup"><span data-stu-id="18f4c-105">Here are some scenarios where a file opens read-only and some steps you can take to change that.</span></span>
  
 <span data-ttu-id="18f4c-106">**Chống vi-rút của tôi đang khiến họ mở ra chỉ đọc**</span><span class="sxs-lookup"><span data-stu-id="18f4c-106">**My antivirus is causing them to open read-only**</span></span>
  
<span data-ttu-id="18f4c-107">Một số chương trình chống vi-rút có thể bảo vệ bạn khỏi các tệp có khả năng không an toàn bằng cách mở chúng chỉ đọc.</span><span class="sxs-lookup"><span data-stu-id="18f4c-107">Some antivirus programs may protect you from potentially unsafe files by opening them read-only.</span></span> <span data-ttu-id="18f4c-108">Bạn có thể cần phải kiểm tra với nhà cung cấp dịch vụ chống vi-rút để tìm hiểu cách điều chỉnh các thiết đặt này.</span><span class="sxs-lookup"><span data-stu-id="18f4c-108">You may need to check with your antivirus provider to learn how to adjust these settings.</span></span> <span data-ttu-id="18f4c-109">BitDefender, ví dụ, có nội dung về việc thêm loại trừ áp dụng ở đây: [làm thế nào để thêm ứng dụng hoặc xử lý các loại trừ trong Trung tâm điều khiển BitDefender](https://aka.ms/AA6098i).</span><span class="sxs-lookup"><span data-stu-id="18f4c-109">BitDefender, for example, has content on adding application exclusions here: [How to add application or process exclusions in Bitdefender Control Center](https://aka.ms/AA6098i).</span></span>
  
 <span data-ttu-id="18f4c-110">**Là các thuộc tính tệp được đặt thành chỉ đọc?**</span><span class="sxs-lookup"><span data-stu-id="18f4c-110">**Are the file properties set to read-only?**</span></span>
  
<span data-ttu-id="18f4c-111">Bạn có thể kiểm tra các thuộc tính tệp bằng cách bấm chuột phải vào tệp và chọn thuộc tính.</span><span class="sxs-lookup"><span data-stu-id="18f4c-111">You can check the file properties by right-clicking on the file and choosing Properties.</span></span> <span data-ttu-id="18f4c-112">Nếu đã chọn thuộc tính chỉ đọc, bạn có thể bỏ chọn và bấm OK.</span><span class="sxs-lookup"><span data-stu-id="18f4c-112">If the Read-only attribute is checked, you can uncheck it and click OK.</span></span>
  
 <span data-ttu-id="18f4c-113">**Nội dung nằm trong dạng xem được bảo vệ**</span><span class="sxs-lookup"><span data-stu-id="18f4c-113">**The content is in protected view**</span></span>
  
<span data-ttu-id="18f4c-114">Các tệp từ Internet và từ các vị trí không an toàn tiềm ẩn khác có thể chứa vi-rút, giun hoặc các loại phần mềm độc hại khác có thể làm hại máy tính của bạn.</span><span class="sxs-lookup"><span data-stu-id="18f4c-114">Files from the Internet and from other potentially unsafe locations can contain viruses, worms, or other kinds of malware that can harm your computer.</span></span> <span data-ttu-id="18f4c-115">Điều này cũng thường là trường hợp với phần đính kèm email hoặc tệp bạn đã tải xuống.</span><span class="sxs-lookup"><span data-stu-id="18f4c-115">This is also commonly the case with email attachments or files you've downloaded.</span></span> <span data-ttu-id="18f4c-116">Để giúp bảo vệ máy tính của bạn, các tệp từ các vị trí không an toàn tiềm ẩn này được mở trong dạng xem được bảo vệ.</span><span class="sxs-lookup"><span data-stu-id="18f4c-116">To help protect your computer, files from these potentially unsafe locations are opened in Protected View.</span></span> <span data-ttu-id="18f4c-117">Bằng cách dùng dạng xem được bảo vệ, bạn có thể đọc một tệp và xem nội dung của nó trong khi giảm bớt rủi ro.</span><span class="sxs-lookup"><span data-stu-id="18f4c-117">By using Protected View, you can read a file and see its contents while reducing the risks.</span></span> <span data-ttu-id="18f4c-118">Để biết thêm thông tin về dạng xem được bảo vệ và cách thay đổi thiết đặt, hãy xem bài viết này: [dạng xem được bảo vệ là gì?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span><span class="sxs-lookup"><span data-stu-id="18f4c-118">For more information on Protected view and how to change settings, see this article: [What is Protected View?](https://support.office.com/article/d6f09ac7-e6b9-4495-8e43-2bbcdbcb6653)</span></span>
  
 <span data-ttu-id="18f4c-119">**OneDrive có đầy đủ không?**</span><span class="sxs-lookup"><span data-stu-id="18f4c-119">**Is OneDrive full?**</span></span>
  
<span data-ttu-id="18f4c-120">Nếu tệp được lưu trữ trên OneDrive và dung lượng lưu trữ OneDrive của bạn đầy đủ thì bạn sẽ không thể lưu tài liệu cho đến khi bạn ở bên dưới dung lượng được phân bổ của mình.</span><span class="sxs-lookup"><span data-stu-id="18f4c-120">If the file is stored on OneDrive and your OneDrive storage space is full, you will be unable to save the document until you are under your allotted space.</span></span> <span data-ttu-id="18f4c-121">Bạn có thể kiểm tra dung lượng trống trên OneDrive bằng cách bấm vào biểu tượng OneDrive trong Trung tâm thông báo và chọn quản lý lưu trữ, hoặc bạn có thể đến [https://onedrive.live.com](https://onedrive.live.com) , đăng nhập và ghi chú số lượng không gian được sử dụng ở phía dưới bên trái của màn hình.</span><span class="sxs-lookup"><span data-stu-id="18f4c-121">You can check your free space on OneDrive by clicking the OneDrive icon in the notification center and choosing Manage storage, or you can go to [https://onedrive.live.com](https://onedrive.live.com), sign in, and note the amount of used space in the lower left of the screen.</span></span>
  
 <span data-ttu-id="18f4c-122">**Office có được kích hoạt không?**</span><span class="sxs-lookup"><span data-stu-id="18f4c-122">**Is Office activated?**</span></span>
  
<span data-ttu-id="18f4c-123">Nếu Office không được kích hoạt hoặc nếu thuê bao của bạn đã hết hạn, bạn có thể ở chế độ tính năng chỉ đọc.</span><span class="sxs-lookup"><span data-stu-id="18f4c-123">If Office is not activated, or if your subscription has expired, you could be in read-only Reduced Functionality Mode.</span></span> <span data-ttu-id="18f4c-124">Để biết thêm thông tin về cách kích hoạt Office, hãy xem: [lỗi sản phẩm chưa được cấp phép và kích hoạt trong Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span><span class="sxs-lookup"><span data-stu-id="18f4c-124">For information on how to Activate Office, see: [Unlicensed Product and activation errors in Office](https://support.office.com/article/0d23d3c0-c19c-4b2f-9845-5344fedc4380).</span></span>
  
 <span data-ttu-id="18f4c-125">**Nếu vẫn không thành công...**</span><span class="sxs-lookup"><span data-stu-id="18f4c-125">**If all else fails...**</span></span>
  
- <span data-ttu-id="18f4c-126">Thử khởi động lại máy tính</span><span class="sxs-lookup"><span data-stu-id="18f4c-126">Try restarting the computer</span></span>
    
- <span data-ttu-id="18f4c-127">Cài đặt các bản Cập Nhật Office</span><span class="sxs-lookup"><span data-stu-id="18f4c-127">Install Office updates</span></span>
    
- <span data-ttu-id="18f4c-128">Thực hiện sửa chữa trực tuyến của Office</span><span class="sxs-lookup"><span data-stu-id="18f4c-128">Perform an Online repair of Office</span></span>
    

