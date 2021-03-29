---
title: Khắc phục sự cố kết hợp kết nối Azure AD
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401929"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="d3da8-102">Khắc phục sự cố kết hợp kết nối Azure AD</span><span class="sxs-lookup"><span data-stu-id="d3da8-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="d3da8-103">Rất khuyên bạn nên đảm bảo rằng một thiết bị có thể truy nhập các điểm cuối đăng ký thiết bị bên dưới tài khoản hệ thống bằng cách sử dụng [script kết nối đăng ký thiết bị kiểm tra](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="d3da8-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="d3da8-104">Nếu bạn đang thiết lập đăng ký thiết bị lần đầu tiên, hãy đảm bảo bạn xem lại tính[năng quản lý thiết bị trong Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) để tìm hiểu cách tải các thiết bị dưới phần điều khiển của Azure AD.</span><span class="sxs-lookup"><span data-stu-id="d3da8-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="d3da8-105">Nếu bạn đang đăng ký thiết bị vào Azure AD trực tiếp và đăng ký chúng vào InTune, hãy đảm bảo rằng bạn đã [cấu hình InTune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) và có [cấp phép](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) tại chỗ trước.</span><span class="sxs-lookup"><span data-stu-id="d3da8-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="d3da8-106">Đảm bảo rằng bạn được phép thực hiện các hoạt động trong Azure AD và quảng cáo tại cơ sở.</span><span class="sxs-lookup"><span data-stu-id="d3da8-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="d3da8-107">Chỉ có một người quản trị toàn cầu trong Azure AD có thể quản lý thiết đặt cho việc đăng ký thiết bị.</span><span class="sxs-lookup"><span data-stu-id="d3da8-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="d3da8-108">Ngoài ra, nếu bạn đang thiết lập đăng ký tự động trong Active Directory tại chỗ của bạn, bạn sẽ cần phải là người quản trị của Active Directory và AD FS (nếu có).</span><span class="sxs-lookup"><span data-stu-id="d3da8-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="d3da8-109">Để biết thêm chi tiết về cách giải quyết các vấn đề có thể xảy ra với nối kết, hãy xem [khắc phục sự cố gia nhập](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) kết hợp để thiết lập kết hợp Azure và quản lý các thiết bị bằng cách sử dụng cổng thông tin Azure AD, hãy xem [thiết lập kết hợp Azure AD đã tham gia (tại chỗ) thiết bị](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) và [quản lý các thiết bị bằng Azure Portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="d3da8-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="d3da8-110">Để giải quyết các sự cố phổ biến với kết hợp Azure Azure Active Directory (AD), hãy xem [câu hỏi thường gặp về gia nhập AZURE AD](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="d3da8-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
