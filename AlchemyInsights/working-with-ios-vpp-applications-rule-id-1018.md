---
title: Làm việc với iOS VPP ứng dụng quy tắc Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 5bcfb6dd7222bd102ff2620c19bfb943e7bd9591
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29497151"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="d0a98-102">Làm việc với iOS VPP ứng dụng</span><span class="sxs-lookup"><span data-stu-id="d0a98-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="d0a98-103">Đọc [làm thế nào để quản lý các ứng dụng iOS mua thông qua một chương trình mua hàng khối lượng với Microsoft dành](https://docs.microsoft.com/intune/vpp-apps-ios) để tìm hiểu về tính năng, những hạn chế, và các bước để làm cho việc sử dụng chương trình mua khối lượng của Apple và hỗ trợ cho nó trong Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d0a98-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="d0a98-104">**Những vấn đề chung:** "Tôi chỉ định một ứng dụng VPP iOS để người dùng của tôi, nhưng tiến trình cài đặt thất bại."</span><span class="sxs-lookup"><span data-stu-id="d0a98-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="d0a98-p101">Điều này có thể xảy ra nếu một mã thông báo VPP duy nhất được sử dụng trên nhiều thiết bị di động quản lý nhà cung cấp. VPP thẻ từ Apple chỉ có thể được sử dụng với một trong những nhà cung cấp. Nếu bạn đã sử dụng một mã thông báo VPP với nhiều nhà cung cấp, bạn lại phải tải lên mã thông báo để dành.</span><span class="sxs-lookup"><span data-stu-id="d0a98-p101">This can happen if a single VPP token is used across multiple mobile device management providers. VPP tokens from Apple may only be used with one provider. If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="d0a98-p102">Việc cài đặt có thể cũng không thành công nếu tổng số cài đặt vượt quá số lượng giấy phép. Để xem báo cáo sử dụng cho các giấy phép của bạn, hãy vào **ứng dụng điện thoại di động dành** \> **giấy phép ứng dụng** trang. Để tìm hiểu làm thế nào để thu hồi giấy phép sử dụng, hãy xem [bài viết này.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="d0a98-p102">The installation can also fail if the total number of installations exceed the number of licenses. To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page. To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

