---
title: Chạy chẩn đoán bộ nhớ Windows trong Windows 10
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: ff8f80b3df4e3809e844195128f4d99cbc4667be
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826689"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="c20b2-102">Chạy chẩn đoán bộ nhớ Windows trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="c20b2-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="c20b2-103">Nếu Windows và ứng dụng trên PC của bạn bị rơi, đóng băng hoặc làm việc theo cách không ổn định, bạn có thể gặp phải sự cố với bộ nhớ của PC (RAM).</span><span class="sxs-lookup"><span data-stu-id="c20b2-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="c20b2-104">Bạn có thể chạy chẩn đoán bộ nhớ Windows để kiểm tra các vấn đề với RAM của PC.</span><span class="sxs-lookup"><span data-stu-id="c20b2-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="c20b2-105">Trong hộp tìm kiếm trên thanh tác vụ, nhập **chẩn đoán bộ nhớ**, rồi chọn **chẩn đoán bộ nhớ Windows**.</span><span class="sxs-lookup"><span data-stu-id="c20b2-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="c20b2-106">Để chạy chẩn đoán, PC cần phải khởi động lại.</span><span class="sxs-lookup"><span data-stu-id="c20b2-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="c20b2-107">Bạn có tùy chọn khởi động lại ngay lập tức (vui lòng lưu công việc của bạn và đóng tài liệu mở và email đầu tiên) hoặc lên lịch chẩn đoán để chạy tự động lần sau khi PC khởi động lại:</span><span class="sxs-lookup"><span data-stu-id="c20b2-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Chẩn đoán bộ nhớ Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="c20b2-109">Khi PC khởi động lại, **công cụ chẩn đoán bộ nhớ Windows** sẽ chạy tự động.</span><span class="sxs-lookup"><span data-stu-id="c20b2-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="c20b2-110">Trạng thái và tiến độ sẽ được hiển thị ở dạng chạy chẩn đoán và bạn có tùy chọn hủy bỏ chẩn đoán bằng cách nhấn phím **esc** trên bàn phím của bạn.</span><span class="sxs-lookup"><span data-stu-id="c20b2-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="c20b2-111">Khi chẩn đoán hoàn tất, Windows sẽ bắt đầu bình thường.</span><span class="sxs-lookup"><span data-stu-id="c20b2-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="c20b2-112">Ngay sau khi khởi động lại, khi máy tính của bạn xuất hiện, một thông báo sẽ xuất hiện (bên cạnh biểu tượng **Trung tâm hành động** trên thanh tác vụ), để cho biết liệu mọi lỗi đã tìm thấy bộ nhớ.</span><span class="sxs-lookup"><span data-stu-id="c20b2-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="c20b2-113">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="c20b2-113">For example:</span></span>

<span data-ttu-id="c20b2-114">Sau đây là biểu tượng Trung tâm hành động:</span><span class="sxs-lookup"><span data-stu-id="c20b2-114">Here's the Action Center icon:</span></span> ![Biểu tượng Trung tâm hành động](media/action-center-icon.png) 

<span data-ttu-id="c20b2-116">Và thông báo mẫu:</span><span class="sxs-lookup"><span data-stu-id="c20b2-116">And a sample notification:</span></span> ![Không có lỗi bộ nhớ](media/no-memory-errors.png)

<span data-ttu-id="c20b2-118">Nếu bạn bị nhỡ thông báo, bạn có thể chọn biểu tượng **Trung tâm hành động** trên thanh tác vụ để hiển thị **Trung tâm hành động** và xem danh sách thông báo có thể cuộn.</span><span class="sxs-lookup"><span data-stu-id="c20b2-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="c20b2-119">Để xem lại thông tin chi tiết, hãy nhập **sự kiện** vào hộp tìm kiếm trên thanh tác vụ của bạn, rồi chọn **trình xem sự kiện**.</span><span class="sxs-lookup"><span data-stu-id="c20b2-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="c20b2-120">Trong ngăn bàn tay trái của **trình xem sự kiện**, dẫn hướng đến **hệ thống > Nhật ký** của bạn.</span><span class="sxs-lookup"><span data-stu-id="c20b2-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="c20b2-121">Trong ngăn bên phải, hãy quét xuống danh sách trong khi đang xem cột **nguồn** , cho đến khi bạn thấy các sự kiện với **memorydiagnostics giá trị nguồn-kết quả**.</span><span class="sxs-lookup"><span data-stu-id="c20b2-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="c20b2-122">Tô sáng từng sự kiện đó và xem thông tin kết quả trong hộp bên dưới tab **chung** bên dưới danh sách.</span><span class="sxs-lookup"><span data-stu-id="c20b2-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
