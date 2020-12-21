---
title: Quản lý nhóm ứng dụng bằng cách dùng cổng thông tin Azure cho Windows Virtual trên máy tính
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003956"
- "7013"
ms.openlocfilehash: 0dd08d04ad6328e7afa158b36517839fc31a8566
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/18/2020
ms.locfileid: "49722050"
---
# <a name="manage-app-groups-by-using-the-azure-portal-for-windows-virtual-desktop"></a><span data-ttu-id="2a2ce-102">Quản lý nhóm ứng dụng bằng cách dùng cổng thông tin Azure cho Windows Virtual trên máy tính</span><span class="sxs-lookup"><span data-stu-id="2a2ce-102">Manage app groups by using the Azure portal for Windows Virtual Desktop</span></span>

<span data-ttu-id="2a2ce-103">Nhóm ứng dụng mặc định được tạo cho một hồ bơi Windows Virtual Desktop host mới cũng phát hành đầy đủ màn hình nền.</span><span class="sxs-lookup"><span data-stu-id="2a2ce-103">The default app group created for a new Windows Virtual Desktop host pool also publishes the full desktop.</span></span> <span data-ttu-id="2a2ce-104">Ngoài ra, bằng cách sử dụng Azure Portal cho phép bạn tạo một hoặc nhiều nhóm ứng dụng RemoteApp cho hồ bơi host.</span><span class="sxs-lookup"><span data-stu-id="2a2ce-104">In addition, using the Azure portal lets you create one or more RemoteApp app groups for the host pool.</span></span>

<span data-ttu-id="2a2ce-105">Quy trình triển khai sẽ thực hiện như sau:</span><span class="sxs-lookup"><span data-stu-id="2a2ce-105">The deployment process will do the following:</span></span>

1. <span data-ttu-id="2a2ce-106">Tạo nhóm ứng dụng RemoteApp.</span><span class="sxs-lookup"><span data-stu-id="2a2ce-106">Create the RemoteApp app group.</span></span>
2. <span data-ttu-id="2a2ce-107">Thêm ứng dụng đã chọn của bạn vào nhóm ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="2a2ce-107">Add your selected apps to the app group.</span></span>
3. <span data-ttu-id="2a2ce-108">Phát hành cá nhân người dùng hoặc nhóm người dùng vào nhóm ứng dụng.</span><span class="sxs-lookup"><span data-stu-id="2a2ce-108">Publish individual users or user groups to the app group.</span></span>
4. <span data-ttu-id="2a2ce-109">Đăng ký nhóm ứng dụng, nếu bạn chọn làm như vậy.</span><span class="sxs-lookup"><span data-stu-id="2a2ce-109">Register the app group, if you choose to do so.</span></span>
5. <span data-ttu-id="2a2ce-110">Tạo một nối kết đến mẫu quản lý tài nguyên Azure theo cấu hình của bạn, mà bạn có thể tải xuống và lưu.</span><span class="sxs-lookup"><span data-stu-id="2a2ce-110">Create a link to an Azure Resource Manager template according to your configuration, which you can download and save.</span></span>

<span data-ttu-id="2a2ce-111">Để tạo nhóm RemoteApp cho Windows Virtual trên máy tính, hãy làm theo các hướng dẫn trong việc [quản lý nhóm ứng dụng với cổng thông tin Azure](https://go.microsoft.com/fwlink/?linkid=2129550).</span><span class="sxs-lookup"><span data-stu-id="2a2ce-111">To create a RemoteApp group for Windows Virtual Desktop, follow the instructions in [Manage app groups with the Azure portal](https://go.microsoft.com/fwlink/?linkid=2129550).</span></span>
