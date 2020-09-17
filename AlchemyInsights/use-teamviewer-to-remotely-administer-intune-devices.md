---
title: Sử dụng TeamViewer để quản lý từ xa các thiết bị InTune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: e931b2092ab049bc01c600344cbd4702848abcd7
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "47798470"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="875f4-102">Sử dụng TeamViewer để quản lý từ xa các thiết bị InTune</span><span class="sxs-lookup"><span data-stu-id="875f4-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="875f4-103">Các thiết bị được quản lý bởi InTune có thể được quản lý từ xa bằng cách sử dụng [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="875f4-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="875f4-104">Để quản lý InTune bằng cách dùng TeamViewer, hãy sử dụng các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="875f4-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="875f4-105">Bắt đầu bằng cách thu thập thông tin xác thực từ TeamViewer để thiết lập trình kết nối TeamViewer trên InTune.</span><span class="sxs-lookup"><span data-stu-id="875f4-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="875f4-106">Điều này cho phép người quản trị nhập chứng danh trong giao diện người dùng trình xem TeamViewer bên dưới thiết bị, thao tác một lần để thiết lập liên kết giữa InTune và dịch vụ TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="875f4-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="875f4-107">**Phần 1: bắt đầu một phiên với thiết bị từ xa**</span><span class="sxs-lookup"><span data-stu-id="875f4-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="875f4-108">Bên dưới **tất cả thiết bị**, chọn thiết bị mà bạn muốn bắt đầu một phiên từ xa.</span><span class="sxs-lookup"><span data-stu-id="875f4-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="875f4-109">Từ  **... Xem thêm**, chọn **phiên mới hỗ trợ từ xa**.</span><span class="sxs-lookup"><span data-stu-id="875f4-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="875f4-110">Chọn **có** để xác nhận bạn muốn thiết lập một phiên làm việc từ xa.</span><span class="sxs-lookup"><span data-stu-id="875f4-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="875f4-111">Sau khi "bắt đầu một phiên làm việc từ xa mới" được dịch vụ TeamViewer nhận ra, bạn sẽ thấy một tùy chọn để **khởi động hỗ trợ từ xa** dưới phần chi tiết của Tổng quan (hoặc, Essentials) cho thiết bị.</span><span class="sxs-lookup"><span data-stu-id="875f4-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="875f4-112">Chọn **xem thêm** để bung rộng ngăn và hiển thị trạng thái hỗ trợ từ xa.</span><span class="sxs-lookup"><span data-stu-id="875f4-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="875f4-113">Chọn **bắt đầu phiên từ xa** để bắt đầu phiên ở bên quản trị.</span><span class="sxs-lookup"><span data-stu-id="875f4-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="875f4-114">Chọn tải xuống nhị phân TeamViewer (Windows), rồi chọn **chạy**.</span><span class="sxs-lookup"><span data-stu-id="875f4-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="875f4-115">**Ghi chú** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở đến trang web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="875f4-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="875f4-116">Xác nhận yêu cầu ứng dụng TeamViewer sẽ thực hiện các thay đổi trên thiết bị (chỉ dành cho Windows).</span><span class="sxs-lookup"><span data-stu-id="875f4-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="875f4-117">Ứng dụng TeamViewer bắt đầu và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="875f4-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="875f4-118">**Phần 2: trên thiết bị đang được nhắm đến phiên làm việc từ xa**</span><span class="sxs-lookup"><span data-stu-id="875f4-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="875f4-119">Mở cổng thông tin công ty InTune.</span><span class="sxs-lookup"><span data-stu-id="875f4-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="875f4-120">Tìm cờ thông báo: "người quản trị CNTT của bạn đang yêu cầu điều khiển thiết bị này cho một phiên hỗ trợ từ xa", rồi chọn thông báo.</span><span class="sxs-lookup"><span data-stu-id="875f4-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="875f4-121">Chọn tải xuống ứng dụng TeamViewer hoặc xác nhận tải xuống ứng dụng TeamViewer từ App Store, rồi chọn **chạy**.</span><span class="sxs-lookup"><span data-stu-id="875f4-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="875f4-122">**Ghi chú** Bạn có thể bỏ qua bất kỳ trang trình duyệt web nào được mở đến trang web TeamViewer.</span><span class="sxs-lookup"><span data-stu-id="875f4-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="875f4-123">Xác nhận yêu cầu ứng dụng TeamViewer sẽ thực hiện các thay đổi trên thiết bị (chỉ dành cho Windows).</span><span class="sxs-lookup"><span data-stu-id="875f4-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="875f4-124">Ứng dụng TeamViewer bắt đầu và bao gồm mã phiên để xác thực kết nối với thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="875f4-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="875f4-125">Bật lên sẽ hỏi bạn có muốn cho phép phiên bắt đầu hay không.</span><span class="sxs-lookup"><span data-stu-id="875f4-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="875f4-126">**Ghi chú** Các mã phiên được tạo bởi dịch vụ TeamViewer chỉ được sử dụng một lần.</span><span class="sxs-lookup"><span data-stu-id="875f4-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="875f4-127">Nếu bạn bị mất kết nối, bạn phải:</span><span class="sxs-lookup"><span data-stu-id="875f4-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="875f4-128">Đóng phiên bản của ứng dụng TeamViewer trên thiết bị từ xa và trên máy trạm quản trị.</span><span class="sxs-lookup"><span data-stu-id="875f4-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="875f4-129">Đóng cổng thông tin công ty trên thiết bị từ xa.</span><span class="sxs-lookup"><span data-stu-id="875f4-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="875f4-130">Khởi tạo một phiên mới "hỗ trợ từ xa mới" từ cổng thông tin quản trị.</span><span class="sxs-lookup"><span data-stu-id="875f4-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="875f4-131">Mở lại cổng thông tin công ty trên thiết bị từ xa để nhận được thông báo mới.</span><span class="sxs-lookup"><span data-stu-id="875f4-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="875f4-132">Tải xuống và mở ứng dụng TeamViewer trên cả thiết bị từ xa và máy trạm quản trị, như trước đây.</span><span class="sxs-lookup"><span data-stu-id="875f4-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>