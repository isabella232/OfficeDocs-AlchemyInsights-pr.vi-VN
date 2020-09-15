---
title: Làm việc với quy tắc ứng dụng iOS VPP 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688968"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="d4669-102">Làm việc với các ứng dụng iOS VPP</span><span class="sxs-lookup"><span data-stu-id="d4669-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="d4669-103">Đọc [cách quản lý các ứng dụng iOS được mua thông qua chương trình mua âm lượng với Microsoft InTune](https://docs.microsoft.com/intune/vpp-apps-ios) để tìm hiểu về các tính năng, ràng buộc và các bước để làm cho việc sử dụng chương trình mua âm lượng của Apple và hỗ trợ cho nó trong Microsoft InTune.</span><span class="sxs-lookup"><span data-stu-id="d4669-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="d4669-104">Các **vấn đề chung:** "Tôi đã gán một ứng dụng iOS VPP cho người dùng của mình, nhưng quá trình cài đặt không thành công."</span><span class="sxs-lookup"><span data-stu-id="d4669-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="d4669-105">Điều này có thể xảy ra nếu một mã thông báo VPP đơn được dùng trên nhiều nhà cung cấp dịch vụ quản lý thiết bị di động.</span><span class="sxs-lookup"><span data-stu-id="d4669-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="d4669-106">Các thẻ VPP từ Apple chỉ có thể sử dụng với một nhà cung cấp.</span><span class="sxs-lookup"><span data-stu-id="d4669-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="d4669-107">Nếu bạn đã sử dụng một mã thông báo VPP với nhiều nhà cung cấp, bạn phải tải lên lại mã thông báo để InTune.</span><span class="sxs-lookup"><span data-stu-id="d4669-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="d4669-108">Quá trình cài đặt cũng có thể không thành công nếu tổng số lượng bản cài đặt vượt quá số lượng giấy phép.</span><span class="sxs-lookup"><span data-stu-id="d4669-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="d4669-109">Để xem báo cáo sử dụng cho giấy phép của bạn, **Intune Mobile apps** hãy đi đến \> trang **giấy phép ứng** dụng InTune trên thiết bị di động.</span><span class="sxs-lookup"><span data-stu-id="d4669-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="d4669-110">Để tìm hiểu cách đòi hỏi giấy phép đang sử dụng, hãy xem [bài viết này.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="d4669-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
