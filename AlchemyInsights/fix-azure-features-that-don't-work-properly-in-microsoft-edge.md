---
title: Cần làm gì nếu các tính năng Azure không hoạt động đúng cách trong Microsoft Edge
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
- "9004128"
- "7206"
ms.openlocfilehash: 463236bcd9ff480471604c992aa1ed1ed4ac2987
ms.sourcegitcommit: 2e4a5153e530bf15744a52e982eeb0d99757e9d2
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/04/2020
ms.locfileid: "49583777"
---
# <a name="what-to-do-if-azure-features-dont-work-properly-in-microsoft-edge"></a><span data-ttu-id="58d61-102">Cần làm gì nếu các tính năng Azure không hoạt động đúng cách trong Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="58d61-102">What to do if Azure features don't work properly in Microsoft Edge</span></span>

<span data-ttu-id="58d61-103">Microsoft Edge đã [biết các vấn đề](https://go.microsoft.com/fwlink/?linkid=2140608) liên quan đến các khu bảo mật và có thể ảnh hưởng đến cách Azure người dùng đăng nhập vào Trung tâm quản trị Windows.</span><span class="sxs-lookup"><span data-stu-id="58d61-103">Microsoft Edge has [known issues](https://go.microsoft.com/fwlink/?linkid=2140608) that are related to security zones and might affect how Azure users log in to Windows Admin Center.</span></span> <span data-ttu-id="58d61-104">Nếu bạn đang gặp sự cố khi sử dụng các tính năng Azure với Microsoft Edge, hãy thử các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="58d61-104">If you're having trouble using Azure features with Microsoft Edge, try the following steps:</span></span>

1. <span data-ttu-id="58d61-105">Trong menu **bắt đầu** , hãy tìm kiếm các **tùy chọn Internet** , rồi chọn nó.</span><span class="sxs-lookup"><span data-stu-id="58d61-105">In the **Start** menu, search for **Internet Options** and select it.</span></span>
2. <span data-ttu-id="58d61-106">Trong hộp thoại **thuộc tính Internet** , đi tới tab **bảo mật** .</span><span class="sxs-lookup"><span data-stu-id="58d61-106">In the **Internet Properties** dialog box, go to the **Security** tab.</span></span>
3. <span data-ttu-id="58d61-107">Chọn vùng **site tin cậy** , rồi chọn nút **site** .</span><span class="sxs-lookup"><span data-stu-id="58d61-107">Select the **Trusted sites** zone and then select the **Sites** button.</span></span>
4. <span data-ttu-id="58d61-108">Trong hộp thoại **site tin cậy** , hãy thêm URL cổng kết nối cũng [https://login.microsoftonline.com](https://login.microsoftonline.com) như [https://login.live.com](https://login.live.com) , rồi chọn **đóng**.</span><span class="sxs-lookup"><span data-stu-id="58d61-108">In the **Trusted sites** dialog box, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
5. <span data-ttu-id="58d61-109">Trong hộp thoại **thuộc tính Internet** , hãy đi đến tab **quyền riêng tư** .</span><span class="sxs-lookup"><span data-stu-id="58d61-109">In the **Internet Properties** dialog box, go to the **Privacy** tab.</span></span>
6. <span data-ttu-id="58d61-110">Trong phần **chặn cửa sổ bật lên** , hãy chọn **thiết đặt**.</span><span class="sxs-lookup"><span data-stu-id="58d61-110">In the **Pop-up Blocker** section, select **Settings**.</span></span> <span data-ttu-id="58d61-111">Trong hộp thoại mở ra, hãy thêm URL cổng kết nối cũng như [https://login.microsoftonline.com](https://login.microsoftonline.com) [https://login.live.com](https://login.live.com) , rồi chọn **đóng**.</span><span class="sxs-lookup"><span data-stu-id="58d61-111">In the dialog box that opens, add your gateway URL as well as [https://login.microsoftonline.com](https://login.microsoftonline.com) and [https://login.live.com](https://login.live.com), and then select **Close**.</span></span>
