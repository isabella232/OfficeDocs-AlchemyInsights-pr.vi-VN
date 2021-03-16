---
title: Loại bỏ dịch vụ nền cho tìm kiếm Microsoft trong Bing
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/12/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9214"
- "9005302"
ms.openlocfilehash: 6447137fca9b2d48508f4e240a438c7f851c103c
ms.sourcegitcommit: 3fb39a080cc8680d960b8468ac9355389a3e2df4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50816343"
---
# <a name="remove-the-background-service-for-microsoft-search-in-bing"></a><span data-ttu-id="579a6-102">Loại bỏ dịch vụ nền cho tìm kiếm Microsoft trong Bing</span><span class="sxs-lookup"><span data-stu-id="579a6-102">Remove the background service for Microsoft Search in Bing</span></span>

<span data-ttu-id="579a6-103">Để loại bỏ dịch vụ nền cho Microsoft Search trong Bing, bạn có thể thử các biện pháp sau đây:</span><span class="sxs-lookup"><span data-stu-id="579a6-103">To remove the background service for Microsoft Search in Bing, you can try the following remedies:</span></span>

1. <span data-ttu-id="579a6-104">Để trở về thiết đặt công cụ tìm kiếm ban đầu, hãy thực hiện các thao tác sau:</span><span class="sxs-lookup"><span data-stu-id="579a6-104">To revert to the original search engine settings, do the following things:</span></span>

    <span data-ttu-id="579a6-105">một.</span><span class="sxs-lookup"><span data-stu-id="579a6-105">a.</span></span> <span data-ttu-id="579a6-106">Chuyển đổi **sử dụng Bing làm công cụ tìm [kiếm](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) mặc định của bạn tắt**.</span><span class="sxs-lookup"><span data-stu-id="579a6-106">Switch the **Use Bing as your default search engine [toggle](https://docs.microsoft.com/deployoffice/microsoft-search-bing#change-whether-bing-is-the-default-search-engine-for-google-chrome) Off**.</span></span>

    <span data-ttu-id="579a6-107">b.</span><span class="sxs-lookup"><span data-stu-id="579a6-107">b.</span></span> <span data-ttu-id="579a6-108">[Đi đến Trung tâm quản trị Microsoft 365](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) và xóa các thiết đặt ảnh hưởng đến tất cả người dùng trong tổ chức của bạn.</span><span class="sxs-lookup"><span data-stu-id="579a6-108">[Go to the Microsoft 365 admin center](https://docs.microsoft.com/deployoffice/microsoft-search-bing#configure-the-setting-in-the-microsoft-365-admin-center-to-allow-the-extension-to-be-installed) and clear the setting that affects all users in your organization.</span></span>

2. <span data-ttu-id="579a6-109">Để loại bỏ dịch vụ nền khỏi thiết bị riêng lẻ, hãy thực hiện các tác vụ sau đây:</span><span class="sxs-lookup"><span data-stu-id="579a6-109">To remove the background service from an individual device, do the following tasks:</span></span>

    <span data-ttu-id="579a6-110">một.</span><span class="sxs-lookup"><span data-stu-id="579a6-110">a.</span></span> <span data-ttu-id="579a6-111">Chọn **Pa-nen điều khiển > chương trình > các chương trình và tính năng**.</span><span class="sxs-lookup"><span data-stu-id="579a6-111">Choose **Control Panel > Programs > Programs and Features**.</span></span>

    <span data-ttu-id="579a6-112">b.</span><span class="sxs-lookup"><span data-stu-id="579a6-112">b.</span></span> <span data-ttu-id="579a6-113">Bấm chuột phải vào **Microsoft Search trong Bing** bên dưới danh sách các chương trình đã cài đặt, rồi bấm vào **gỡ cài đặt**.</span><span class="sxs-lookup"><span data-stu-id="579a6-113">Right-click **Microsoft Search in Bing** under the list of installed programs, and then click **Uninstall**.</span></span>

3. <span data-ttu-id="579a6-114">Để loại bỏ dịch vụ nền khỏi nhiều thiết bị trong tổ chức của bạn, hãy đăng nhập với tư cách là người quản trị và chạy lệnh sau đây trong một tập lệnh:</span><span class="sxs-lookup"><span data-stu-id="579a6-114">To remove the background service from multiple devices in your organization, log in as an administrator and run the following command in a script:</span></span> 

`"%ProgramFiles(x86)%\Microsoft\DefaultPackMSI\MainBootStrap.exe" uninstallAll`
