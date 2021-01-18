---
title: Cấu hình dịch vụ miền
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885784"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="5fa98-102">Không thể bật không kích hoạt được-DS hoặc triển khai</span><span class="sxs-lookup"><span data-stu-id="5fa98-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="5fa98-103">Để giải quyết vấn đề dịch vụ Azure AD Domain (không được bật hoặc không cho phép triển khai, hãy thực hiện các bước sau đây:</span><span class="sxs-lookup"><span data-stu-id="5fa98-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="5fa98-104">Nếu bạn đang sử dụng một mạng ảo hiện có, hãy kiểm tra NSG của bạn để quy tắc chặn các cổng cần thiết để đồng bộ hóa trong thiết bị in-DS trong cổng thông tin https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="5fa98-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="5fa98-105">Kiểm tra xem thông báo lỗi của bạn được trả lời trong hướng dẫn khắc phục sự cố này sẵn dùng hay không  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="5fa98-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="5fa98-106">Thử triển khai các dịch vụ tên miền Azure AD trong một mạng ảo mới.</span><span class="sxs-lookup"><span data-stu-id="5fa98-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="5fa98-107">Làm theo hướng dẫn bắt đầu về cách triển khai thiết [lập: tạo và đặt cấu hình dịch vụ miền](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance)của bạn.</span><span class="sxs-lookup"><span data-stu-id="5fa98-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="5fa98-108">Nếu bạn đang gặp vấn đề khi triển khai Azure AD Domain Services, hãy xem [khắc phục sự cố dịch vụ AZURE AD Domain](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) để giải quyết các lỗi thường gặp để giúp bạn làm việc cùng một lần nữa.</span><span class="sxs-lookup"><span data-stu-id="5fa98-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="5fa98-109">**Không thể tắt tính năng đọc tiếng Anh**</span><span class="sxs-lookup"><span data-stu-id="5fa98-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="5fa98-110">Không thể tạm dừng không đọc được.</span><span class="sxs-lookup"><span data-stu-id="5fa98-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="5fa98-111">Nếu bạn muốn ngừng sử dụng tên miền được quản lý của mình, nó phải bị xóa bỏ.</span><span class="sxs-lookup"><span data-stu-id="5fa98-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="5fa98-112">Để xóa tên miền được quản lý của bạn, hãy xem [xóa dịch vụ tên miền AAD](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="5fa98-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



