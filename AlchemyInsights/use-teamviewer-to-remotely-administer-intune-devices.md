---
title: Sử dụng TeamViewer để quản lý từ xa các thiết bị InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555755"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="8f481-102">Sử dụng TeamViewer để quản lý từ xa các thiết bị InTune</span><span class="sxs-lookup"><span data-stu-id="8f481-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="8f481-103">Thiết bị được quản lý bởi InTune có thể được dùng từ xa bằng cách sử dụng [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="8f481-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="8f481-104">Quản lý InTune bằng cách sử dụng TeamViewer, sử dụng các bước sau:</span><span class="sxs-lookup"><span data-stu-id="8f481-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="8f481-105">Bắt đầu bằng cách lấy thông tin từ TeamViewer để thiết lập kết nối TeamViewer trên InTune.</span><span class="sxs-lookup"><span data-stu-id="8f481-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="8f481-106">Điều này cho phép quản trị viên nhập thông tin đăng nhập trong giao diện người dùng TeamViewer Connector trong thiết bị, thao tác một lần để thiết lập liên kết giữa InTune và dịch vụ TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="8f481-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="8f481-107">**Phần 1: bắt đầu một phiên với một thiết bị từ xa**</span><span class="sxs-lookup"><span data-stu-id="8f481-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="8f481-108">Trong **tất cả các thiết bị**, chọn thiết bị bạn muốn bắt đầu một phiên làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="8f481-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="8f481-109">Từ **... Hơn nữa**, chọn **phiên hỗ trợ từ xa mới**.</span><span class="sxs-lookup"><span data-stu-id="8f481-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="8f481-110">Chọn **có** để thừa nhận bạn muốn thiết lập một phiên làm từ xa.</span><span class="sxs-lookup"><span data-stu-id="8f481-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="8f481-111">Sau khi yêu cầu "bắt đầu phiên làm việc từ xa mới" được công nhận bởi dịch vụ TeamViewer, bạn sẽ thấy một tùy chọn để **khởi động hỗ trợ từ xa** theo chi tiết của ngăn tổng quan (hoặc, Essentials) cho thiết bị.</span><span class="sxs-lookup"><span data-stu-id="8f481-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="8f481-112">Chọn **xem thêm** để mở rộng ngăn và hiển thị trạng thái hỗ trợ từ xa.</span><span class="sxs-lookup"><span data-stu-id="8f481-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="8f481-113">Chọn **khởi động phiên từ xa** để bắt đầu phiên ở phía quản trị.</span><span class="sxs-lookup"><span data-stu-id="8f481-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="8f481-114">Chọn để tải về các nhị phân TeamViewer (Windows), và chọn **Run**.</span><span class="sxs-lookup"><span data-stu-id="8f481-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="8f481-115">**Lưu ý** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở vào trang web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="8f481-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="8f481-116">Thừa nhận yêu cầu cho ứng dụng TeamViewer để thực hiện thay đổi trên thiết bị (chỉ dành cho Windows).</span><span class="sxs-lookup"><span data-stu-id="8f481-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="8f481-117">Ứng dụng TeamViewer khởi động và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="8f481-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="8f481-118">**Phần 2: trên thiết bị đang được nhắm mục tiêu cho một phiên làm việc từ xa**</span><span class="sxs-lookup"><span data-stu-id="8f481-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="8f481-119">Mở cổng công ty InTune.</span><span class="sxs-lookup"><span data-stu-id="8f481-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="8f481-120">Tìm cờ thông báo: "người quản trị CNTT của bạn đang yêu cầu quyền kiểm soát thiết bị này cho phiên hỗ trợ từ xa" và chọn thông báo.</span><span class="sxs-lookup"><span data-stu-id="8f481-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="8f481-121">Chọn để tải xuống ứng dụng TeamViewer hoặc xác nhận tải xuống ứng dụng TeamViewer từ cửa hàng ứng dụng và chọn **chạy**.</span><span class="sxs-lookup"><span data-stu-id="8f481-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="8f481-122">**Lưu ý** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở vào trang web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="8f481-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="8f481-123">Thừa nhận yêu cầu cho ứng dụng TeamViewer để thực hiện thay đổi trên thiết bị (chỉ dành cho Windows).</span><span class="sxs-lookup"><span data-stu-id="8f481-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="8f481-124">Ứng dụng TeamViewer khởi động và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="8f481-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="8f481-125">Một popup sẽ hỏi nếu bạn muốn cho phép phiên để bắt đầu.</span><span class="sxs-lookup"><span data-stu-id="8f481-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="8f481-126">**Lưu ý** Mã phiên được tạo bởi dịch vụ TeamViewer chỉ sử dụng một lần.</span><span class="sxs-lookup"><span data-stu-id="8f481-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="8f481-127">Nếu bạn bị mất kết nối, bạn phải:</span><span class="sxs-lookup"><span data-stu-id="8f481-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="8f481-128">Đóng phiên bản ứng dụng TeamViewer trên thiết bị từ xa và trên trạm làm việc quản trị.</span><span class="sxs-lookup"><span data-stu-id="8f481-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="8f481-129">Đóng cổng công ty trên thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="8f481-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="8f481-130">Khởi tạo mới "phiên hỗ trợ từ xa mới" từ cổng quản trị.</span><span class="sxs-lookup"><span data-stu-id="8f481-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="8f481-131">Mở lại cổng công ty trên thiết bị từ xa để nhận được thông báo mới.</span><span class="sxs-lookup"><span data-stu-id="8f481-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="8f481-132">Tải xuống và mở ứng dụng TeamViewer trên cả thiết bị từ xa và máy trạm quản trị, như trước đây.</span><span class="sxs-lookup"><span data-stu-id="8f481-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>