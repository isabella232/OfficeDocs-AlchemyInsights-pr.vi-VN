---
title: Lỗi đăng nhập OneDrive AADSTS50011
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
- "9003820"
- "6840"
ms.openlocfilehash: 1f906f82e99c322ed953800d54fba5a073eacd10
ms.sourcegitcommit: 534e9217d99336eb471166ff83231c7e408fb1d9
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 11/09/2020
ms.locfileid: "48982551"
---
# <a name="onedrive-login-error-aadsts50011"></a><span data-ttu-id="b300b-102">Lỗi đăng nhập OneDrive AADSTS50011</span><span class="sxs-lookup"><span data-stu-id="b300b-102">OneDrive login error AADSTS50011</span></span>

<span data-ttu-id="b300b-103">Nếu bạn nhận được lỗi "AADSTS50011: URL trả lời được xác định trong yêu cầu không khớp trả lời" khi đăng nhập vào ứng dụng OneDrive, hãy kiểm tra các mục sau:</span><span class="sxs-lookup"><span data-stu-id="b300b-103">If you receive an error "AADSTS50011: The reply URL specified in the request does not match the reply" when signing into the OneDrive app, check for the following:</span></span>

<span data-ttu-id="b300b-104">Phiên bản OneDrive của bạn cần bằng hoặc lớn hơn phiên bản 20.052. XXXX. XXXX.</span><span class="sxs-lookup"><span data-stu-id="b300b-104">Your OneDrive version needs to be equal to or greater than version 20.052.XXXX.XXXX.</span></span> <span data-ttu-id="b300b-105">Để kiểm tra phiên bản của bạn, hãy bấm vào biểu tượng OneDrive màu lam trong khu vực thông báo, chọn **Trợ giúp & thiết đặt > thiết đặt > giới thiệu về**.</span><span class="sxs-lookup"><span data-stu-id="b300b-105">To check your version, click on the blue OneDrive icon in the notification area, select **Help & Settings > Settings > About**.</span></span>

<span data-ttu-id="b300b-106">Mạng của bạn có thể chặn lưu lượng đến **g.Live.com** và **oneclient.SFX.MS**.</span><span class="sxs-lookup"><span data-stu-id="b300b-106">Your network might block traffic to **g.live.com** and **oneclient.sfx.ms**.</span></span> <span data-ttu-id="b300b-107">Nếu lưu lượng đó bị chặn, OneDrive không thể cập nhật chính nó.</span><span class="sxs-lookup"><span data-stu-id="b300b-107">If that traffic is blocked, OneDrive cannot update itself.</span></span> <span data-ttu-id="b300b-108">Làm việc với người quản trị mạng của bạn để đảm bảo bạn có quyền truy nhập vào những URL đó.</span><span class="sxs-lookup"><span data-stu-id="b300b-108">Work with your network administrator to ensure you have access to those URLs.</span></span> <span data-ttu-id="b300b-109">[Những điểm cuối này](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) sẽ có thể truy cập đối với khách hàng bằng cách sử dụng các gói Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="b300b-109">[These endpoints](https://docs.microsoft.com/microsoft-365/enterprise/urls-and-ip-address-ranges?view=o365-worldwide) should be reachable for customers using Microsoft 365 plans.</span></span>

<span data-ttu-id="b300b-110">Nếu bạn cần lấy phiên bản hiện tại của OneDrive, hãy truy nhập [https://aka.ms/getonedrive](https://aka.ms/getonedrive) .</span><span class="sxs-lookup"><span data-stu-id="b300b-110">If you need to manually get a current version of OneDrive, visit [https://aka.ms/getonedrive](https://aka.ms/getonedrive).</span></span>
