---
title: Chạy Windows chẩn đoán bộ nhớ trong Windows 10
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002959"
- "5661"
ms.openlocfilehash: 3fedc52d02f1f70743429d0313eda0361306c3f3
ms.sourcegitcommit: 18b080c2a5d741af01ec589158effc35ea7cf449
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44358289"
---
# <a name="run-windows-memory-diagnostics-in-windows-10"></a><span data-ttu-id="cbfc6-102">Chạy Windows chẩn đoán bộ nhớ trong Windows 10</span><span class="sxs-lookup"><span data-stu-id="cbfc6-102">Run Windows Memory Diagnostics in Windows 10</span></span>

<span data-ttu-id="cbfc6-103">Nếu Windows và các ứng dụng trên máy tính của bạn bị rơi, đóng băng hoặc hành động một cách không ổn định, bạn có thể gặp sự cố với bộ nhớ (RAM) của PC.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-103">If Windows and apps on your PC are crashing, freezing, or acting in an unstable manner, you may have a problem with the PC’s memory (RAM).</span></span> <span data-ttu-id="cbfc6-104">Bạn có thể chạy các chẩn đoán bộ nhớ Windows để kiểm tra các vấn đề với RAM của máy tính.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-104">You can run the Windows Memory Diagnostic to check for problems with the PC’s RAM.</span></span>

<span data-ttu-id="cbfc6-105">Trong hộp tìm kiếm trên thanh tác vụ của bạn, hãy nhập **chẩn đoán bộ nhớ**, sau đó chọn **chẩn đoán bộ nhớ Windows**.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-105">In the search box on your taskbar, type **memory diagnostic**, and then select **Windows Memory Diagnostic**.</span></span> 

<span data-ttu-id="cbfc6-106">Để chạy chẩn đoán, máy tính cần khởi động lại.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-106">To run the diagnostic, the PC needs to restart.</span></span> <span data-ttu-id="cbfc6-107">Bạn có tùy chọn để khởi động lại ngay lập tức (Hãy lưu công việc của bạn và đóng tài liệu mở và e-mail đầu tiên), hoặc lịch trình chẩn đoán để chạy tự động trong lần tiếp theo máy tính khởi động lại:</span><span class="sxs-lookup"><span data-stu-id="cbfc6-107">You have the option to restart immediately (please save your work and close open documents and e-mails first), or schedule the diagnostic to run automatically the next time the PC restarts:</span></span>

![Chẩn đoán bộ nhớ Windows](media/windows-memory-diagnostic.png)

<span data-ttu-id="cbfc6-109">Khi máy tính khởi động lại, **công cụ chẩn đoán bộ nhớ của Windows** sẽ tự chạy.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-109">When the PC restarts, the **Windows Memory Diagnostics Tool** will run automatically.</span></span> <span data-ttu-id="cbfc6-110">Trạng thái và tiến trình sẽ được hiển thị khi chạy chẩn đoán và bạn có tùy chọn hủy chẩn đoán bằng việc nhấn phím **esc** trên bàn phím.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-110">Status and progress will be displayed as the diagnostics run, and you have the option of cancelling the diagnostics by hitting the **ESC** key on your keyboard.</span></span>

<span data-ttu-id="cbfc6-111">Khi chẩn đoán hoàn tất, Windows sẽ bắt đầu bình thường.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-111">When the diagnostics are complete, Windows will start normally.</span></span>
<span data-ttu-id="cbfc6-112">Ngay sau khi khởi động lại, khi máy tính để bàn xuất hiện, một thông báo sẽ xuất hiện (bên cạnh biểu tượng **Trung tâm hành động** trên thanh tác vụ), để cho biết bất kỳ lỗi bộ nhớ nào được tìm thấy.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-112">Immediately after restart, when the Desktop appears, a notification will appear (next to the **Action Center** icon on the taskbar), to indicate whether any memory errors were found.</span></span> <span data-ttu-id="cbfc6-113">Ví dụ:</span><span class="sxs-lookup"><span data-stu-id="cbfc6-113">For example:</span></span>

<span data-ttu-id="cbfc6-114">Dưới đây là biểu tượng Action Center:</span><span class="sxs-lookup"><span data-stu-id="cbfc6-114">Here's the Action Center icon:</span></span> ![Biểu tượng Trung tâm hành động](media/action-center-icon.png) 

<span data-ttu-id="cbfc6-116">Và một thông báo mẫu:</span><span class="sxs-lookup"><span data-stu-id="cbfc6-116">And a sample notification:</span></span> ![Không có lỗi bộ nhớ](media/no-memory-errors.png)

<span data-ttu-id="cbfc6-118">Nếu bạn bỏ qua thông báo, bạn có thể chọn biểu tượng **Trung tâm hành động** trên thanh tác vụ để hiển thị **Trung tâm hành động** và xem danh sách thông báo có thể cuộn.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-118">If you missed the notification, you can select the **Action Center** icon  on the taskbar to display the **Action Center** and see a scrollable list of notifications.</span></span>

<span data-ttu-id="cbfc6-119">Để xem lại thông tin chi tiết, hãy nhập **sự kiện** vào hộp tìm kiếm trên thanh tác vụ của bạn, sau đó chọn trình chuyển đổi **sự kiện**.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-119">To review detailed information, type **event** into the search box on your taskbar, and then select **Event Viewer**.</span></span> <span data-ttu-id="cbfc6-120">Trong ngăn bên trái của **trình xem sự kiện**, điều hướng đến **nhật ký Windows > hệ thống**.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-120">In the **Event Viewer**’s left-hand pane, navigate to **Windows Logs > System**.</span></span> <span data-ttu-id="cbfc6-121">Trong ngăn bên phải, quét danh sách trong khi nhìn vào cột **nguồn** , cho đến khi bạn thấy sự kiện với nguồn giá trị **memorydiagnostics-kết quả**.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-121">In the right-hand pane, scan down the list while looking at the **Source** column, until you see events with Source value **MemoryDiagnostics-Results**.</span></span> <span data-ttu-id="cbfc6-122">Làm nổi bật mỗi sự kiện như vậy và xem thông tin kết quả trong hộp dưới tab **chung** bên dưới danh sách.</span><span class="sxs-lookup"><span data-stu-id="cbfc6-122">Highlight each such event and see the result information in the box under the **General** tab below the list.</span></span>
