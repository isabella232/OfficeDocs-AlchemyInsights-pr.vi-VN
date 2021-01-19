---
title: Bộ điều khiển tên miền
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901319"
---
# <a name="domain-controller"></a><span data-ttu-id="a0efa-102">Bộ điều khiển tên miền</span><span class="sxs-lookup"><span data-stu-id="a0efa-102">Domain controller</span></span>

<span data-ttu-id="a0efa-103">**Không thể bật không kích hoạt được-DS hoặc triển khai**</span><span class="sxs-lookup"><span data-stu-id="a0efa-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="a0efa-104">Để giải quyết vấn đề dịch vụ Azure AD Domain (không được bật hoặc không cho phép triển khai, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="a0efa-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="a0efa-105">Nếu bạn đang sử dụng một mạng ảo hiện có, hãy kiểm tra NSG của bạn để quy tắc chặn các cổng cần thiết để đồng bộ hóa trong thiết bị in-DS trong cổng thông tin https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="a0efa-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="a0efa-106">Kiểm tra xem thông báo lỗi của bạn được trả lời trong hướng dẫn khắc phục sự cố này sẵn dùng hay không  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="a0efa-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="a0efa-107">Thử triển khai các dịch vụ tên miền Azure AD trong một mạng ảo mới.</span><span class="sxs-lookup"><span data-stu-id="a0efa-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="a0efa-108">Hãy làm theo hướng dẫn bắt đầu về cách triển khai các phép tiếp tục, vốn sẵn dùng tại mục [hướng dẫn để tạo Dịch vụ AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="a0efa-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="a0efa-109">Nếu bạn đang gặp vấn đề khi triển khai Azure AD Domain Services, hãy xem [khắc phục sự cố dịch vụ AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) để giải quyết các lỗi thường gặp để giúp bạn làm việc cùng một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="a0efa-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="a0efa-110">**Không thể tắt tính năng đọc tiếng Anh**</span><span class="sxs-lookup"><span data-stu-id="a0efa-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="a0efa-111">Không thể tạm dừng không đọc được.</span><span class="sxs-lookup"><span data-stu-id="a0efa-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="a0efa-112">Nếu bạn muốn ngừng sử dụng tên miền được quản lý của mình, nó phải bị xóa bỏ.</span><span class="sxs-lookup"><span data-stu-id="a0efa-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="a0efa-113">Nếu bạn gặp phải sự cố, để giải quyết thông báo lỗi thông thường và đối với các bước khắc phục sự cố liên kết để giúp bạn có thể chạy lại, hãy xem [khắc phục sự cố dịch vụ miền Azure Active Directory](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="a0efa-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
