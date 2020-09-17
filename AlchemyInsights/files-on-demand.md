---
title: Các tệp theo yêu cầu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6432"
- "9003530"
ms.openlocfilehash: e0ba83778179abefe3ac4fe3e8ab0303d65ad929
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47804379"
---
# <a name="configure-files-on-demand"></a><span data-ttu-id="3811d-102">Cấu hình các tệp theo yêu cầu</span><span class="sxs-lookup"><span data-stu-id="3811d-102">Configure Files On-Demand</span></span>

<span data-ttu-id="3811d-103">Tệp OneDrive theo yêu cầu sẽ giúp bạn truy nhập tất cả các tệp trong OneDrive mà không cần phải tải xuống tất cả chúng và sử dụng dung lượng lưu trữ trên thiết bị của bạn.</span><span class="sxs-lookup"><span data-stu-id="3811d-103">OneDrive Files On-Demand helps you access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

<span data-ttu-id="3811d-104">Để cấu hình các tệp theo yêu cầu trên PC của bạn:</span><span class="sxs-lookup"><span data-stu-id="3811d-104">To configure Files On-Demand on your PC:</span></span>

1. <span data-ttu-id="3811d-105">Chọn biểu tượng đám mây **Onedrive** màu trắng hoặc màu lam trong khu vực thông báo trên thanh tác vụ Windows.</span><span class="sxs-lookup"><span data-stu-id="3811d-105">Select the white or blue **OneDrive** cloud icon in the Windows taskbar notification area.</span></span> <span data-ttu-id="3811d-106">Chọn **thiết đặt**> **Trợ giúp & thiết đặt** bánh răng.</span><span class="sxs-lookup"><span data-stu-id="3811d-106">Select the **Help & Settings** gear icon > **Settings**.</span></span>
2. <span data-ttu-id="3811d-107">Trên tab **thiết đặt** , hãy chọn **dung lượng lưu và tải xuống các tệp khi bạn sử dụng** hộp thư.</span><span class="sxs-lookup"><span data-stu-id="3811d-107">On the **Settings** tab, select the **Save space and download files as you use them** box.</span></span>  

<span data-ttu-id="3811d-108">Bạn cũng có thể cấu hình các tệp theo yêu cầu bằng cách sử dụng sổ đăng ký.</span><span class="sxs-lookup"><span data-stu-id="3811d-108">You can also configure Files On-Demand using the registry.</span></span>

<span data-ttu-id="3811d-109">Nếu bạn vô hiệu hóa thiết đặt này, người dùng Windows 10 có cùng một hành vi đồng bộ với những người dùng của các phiên bản trước của Windows và không thể bật các tệp theo yêu cầu.</span><span class="sxs-lookup"><span data-stu-id="3811d-109">If you disable this setting, Windows 10 users have the same sync behavior as users of previous versions of Windows, and aren't able to turn on Files On-Demand.</span></span> <span data-ttu-id="3811d-110">Nếu bạn không cấu hình thiết đặt này, người dùng có thể bật hoặc tắt các tệp theo yêu cầu.</span><span class="sxs-lookup"><span data-stu-id="3811d-110">If you do not configure this setting, users can turn Files On-Demand on or off.</span></span>

<span data-ttu-id="3811d-111">Cho phép chính sách này đặt giá trị khóa đăng ký sau đây thành 1.</span><span class="sxs-lookup"><span data-stu-id="3811d-111">Enabling this policy sets the following registry key value to 1.</span></span> <span data-ttu-id="3811d-112">Vô hiệu hóa chính sách này đặt giá trị khóa đăng ký sau đây thành 0.</span><span class="sxs-lookup"><span data-stu-id="3811d-112">Disabling this policy sets the following registry key value to 0.</span></span>

`[HKLM\SOFTWARE\Policies\Microsoft\OneDrive]"FilesOnDemandEnabled"="dword:00000001"`

<span data-ttu-id="3811d-113">Nếu bạn không nhìn thấy tùy chọn tệp theo yêu cầu trong "thiết đặt", hãy đảm bảo rằng "kiểu trình điều khiển bộ lọc tệp của Windows Cloud" được đặt là 2 (AUTO_START).</span><span class="sxs-lookup"><span data-stu-id="3811d-113">If you can't see the Files On-Demand option in "Settings," make sure the service "Windows Cloud Files Filter Driver" start type is set to 2 (AUTO_START).</span></span> <span data-ttu-id="3811d-114">Cho phép tính năng này đặt giá trị khóa đăng ký sau đây thành 2.</span><span class="sxs-lookup"><span data-stu-id="3811d-114">Enabling this feature sets the following registry key value to 2.</span></span>

`[HKLM\SYSTEM\CurrentControlSet\Services\CldFlt]"Start"="dword:00000002"`