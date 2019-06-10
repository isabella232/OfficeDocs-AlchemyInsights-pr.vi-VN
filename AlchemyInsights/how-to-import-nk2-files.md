---
title: làm thế nào-to-nhập khẩu-nk2-files
ms.author: daeite
author: daeite
manager: joallard
ms.date: 5/3/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1800027"
- "1267"
ms.assetid: ''
ms.openlocfilehash: 1d1b02527c3b614375cf1f84a7a511d9318689b1
ms.sourcegitcommit: 136b8209c52c2a05d0f2fdaab93b2cd92253fa2c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/07/2019
ms.locfileid: "34770268"
---
# <a name="how-to-import-nk2-files"></a><span data-ttu-id="3ab07-102">Làm thế nào để nhập tệp .nk2</span><span class="sxs-lookup"><span data-stu-id="3ab07-102">How to import .nk2 files</span></span> 

<span data-ttu-id="3ab07-103">Khi bạn khởi động Microsoft Outlook 2013, Outlook 2016, Outlook 2019 hoặc Outlook cho Office 365 Beta dành cho lần đầu tiên, bộ nhớ cache biệt hiệu (được lưu trữ trong tập tin .nk2 *profilename*) được nhập vào một thông điệp ẩn ở cửa hàng tin nhắn mặc định của bạn.</span><span class="sxs-lookup"><span data-stu-id="3ab07-103">When you start Microsoft Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365 for the first time, your nickname cache (stored in the *profilename*.nk2 file) is imported into a hidden message in your default message store.</span></span>

<span data-ttu-id="3ab07-104">Để nhập tệp .nk2 vào Outlook 2013, Outlook 2016, Outlook 2019 hoặc Outlook cho Office 365, hãy chắc chắn rằng tệp .nk2 trong cặp sau: %appdata%\Microsoft\Outlook</span><span class="sxs-lookup"><span data-stu-id="3ab07-104">To import .nk2 files into Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365, make sure that the .nk2 file is in the following folder: %appdata%\Microsoft\Outlook</span></span>

<span data-ttu-id="3ab07-105">**Lưu ý**: tập tin .nk2 phải có cùng tên như tiểu sử hiện tại của bạn Outlook 2013 hoặc Outlook 2016.</span><span class="sxs-lookup"><span data-stu-id="3ab07-105">**Note**: The .nk2 file must have the same name as your current Outlook 2013 or Outlook 2016 profile.</span></span> <span data-ttu-id="3ab07-106">Theo mặc định, tên cấu hình là "Outlook."</span><span class="sxs-lookup"><span data-stu-id="3ab07-106">By default, the profile name is "Outlook."</span></span> <span data-ttu-id="3ab07-107">Để kiểm tra tên tiểu sử, hãy làm theo các bước sau:</span><span class="sxs-lookup"><span data-stu-id="3ab07-107">To check the profile name, follow these steps:</span></span> 
1. <span data-ttu-id="3ab07-108">Nhấp vào **bắt đầu**, và sau đó nhấp vào **Bảng điều khiển**.</span><span class="sxs-lookup"><span data-stu-id="3ab07-108">Click **Start**, and then click **Control Panel**.</span></span>
2. <span data-ttu-id="3ab07-109">Nhấp đúp vào **thư**.</span><span class="sxs-lookup"><span data-stu-id="3ab07-109">Double-click **Mail**.</span></span>
3. <span data-ttu-id="3ab07-110">Trong hộp thoại thiết lập thư, chọn **Hiển thị cấu hình**.</span><span class="sxs-lookup"><span data-stu-id="3ab07-110">In the Mail Setup dialog box, select **Show Profiles**.</span></span>
4. <span data-ttu-id="3ab07-111">Chọn **bắt đầu** > **chạy**.</span><span class="sxs-lookup"><span data-stu-id="3ab07-111">Select **Start** > **Run**.</span></span>
5. <span data-ttu-id="3ab07-112">Trong các **mở** hộp, loại *outlook.exe /importnk2*, và sau đó chọn **OK**.</span><span class="sxs-lookup"><span data-stu-id="3ab07-112">In the **Open** box, type *outlook.exe /importnk2*, and then select **OK**.</span></span> 

<span data-ttu-id="3ab07-113">Sau khi bạn nhập tệp .nk2, nội dung của các tập tin được sáp nhập vào bộ đệm ẩn biệt hiệu hiện có được lưu trữ trong hộp thư của bạn.</span><span class="sxs-lookup"><span data-stu-id="3ab07-113">After you import the .nk2 file, the contents of the file are merged into the existing nickname cache stored in your mailbox.</span></span>

<span data-ttu-id="3ab07-114">**Lưu ý**: tập tin .nk2 đổi tên với một phần mở rộng tên tệp .old thời gian tiếp theo bạn khởi động Outlook 2013, Outlook 2016, Outlook 2019 hoặc Outlook cho Office 365.</span><span class="sxs-lookup"><span data-stu-id="3ab07-114">**Note**: The .nk2 file is renamed with a .old file name extension the next time you start Outlook 2013, Outlook 2016, Outlook 2019 or Outlook for Office 365.</span></span> <span data-ttu-id="3ab07-115">Nếu muốn tái nhập tệp .nk2, loại bỏ phần mở rộng tên tệp .old lần đầu tiên.</span><span class="sxs-lookup"><span data-stu-id="3ab07-115">If want to re-import the .nk2 file, remove the .old file name extension first.</span></span>

<span data-ttu-id="3ab07-116">Để biết thêm chi tiết, hãy xem [nhập hoặc sao chép danh sách Auto-Complete sang máy tính khác](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span><span class="sxs-lookup"><span data-stu-id="3ab07-116">For more information, see [Import or copy the Auto-Complete List to another computer](https://support.microsoft.com/help/2806550/how-to-import-nk2-files-into-outlook%).</span></span>