---
title: Làm việc với các ứng dụng iOS VPP ID quy tắc 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 88a1ef66bf337b3a0094976c122330591aee77ff
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43719979"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="7fa15-102">Làm việc với các ứng dụng iOS VPP</span><span class="sxs-lookup"><span data-stu-id="7fa15-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="7fa15-103">Đọc [cách quản lý các ứng dụng iOS mua thông qua chương trình mua ổ đĩa với Microsoft InTune](https://docs.microsoft.com/intune/vpp-apps-ios) để tìm hiểu về các tính năng, ràng buộc và các bước để sử dụng chương trình mua và hỗ trợ của Apple trong Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="7fa15-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="7fa15-104">**Các vấn đề thường gặp:** "Tôi đã gán một ứng dụng iOS VPP cho người dùng của tôi, nhưng việc cài đặt không thành công."</span><span class="sxs-lookup"><span data-stu-id="7fa15-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="7fa15-105">Điều này có thể xảy ra nếu một mã thông báo VPP duy nhất được sử dụng trên nhiều nhà cung cấp quản lý thiết bị di động.</span><span class="sxs-lookup"><span data-stu-id="7fa15-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="7fa15-106">Thẻ VPP từ Apple chỉ có thể được sử dụng với một nhà cung cấp.</span><span class="sxs-lookup"><span data-stu-id="7fa15-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="7fa15-107">Nếu bạn sử dụng một thẻ VPP với nhiều nhà cung cấp, bạn phải tải lên lại mã thông báo để InTune.</span><span class="sxs-lookup"><span data-stu-id="7fa15-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="7fa15-108">Quá trình cài đặt cũng có thể thất bại nếu tổng số cài đặt vượt quá số lượng giấy phép.</span><span class="sxs-lookup"><span data-stu-id="7fa15-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="7fa15-109">Để xem báo cáo sử dụng cho giấy phép của bạn, hãy chuyển đến trang \> **giấy phép** ứng dụng **dành cho thiết bị di động InTune** .</span><span class="sxs-lookup"><span data-stu-id="7fa15-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="7fa15-110">Để tìm hiểu cách lấy lại giấy phép sử dụng, hãy xem [bài viết này.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="7fa15-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
