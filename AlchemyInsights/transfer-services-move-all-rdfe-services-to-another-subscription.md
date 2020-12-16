---
title: Dịch vụ chuyển-di chuyển tất cả các dịch vụ RDFE sang một đăng ký khác
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692426"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="a1e03-102">Dịch vụ chuyển-di chuyển tất cả các dịch vụ RDFE sang một đăng ký khác</span><span class="sxs-lookup"><span data-stu-id="a1e03-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="a1e03-103">**Di chuyển tài nguyên**</span><span class="sxs-lookup"><span data-stu-id="a1e03-103">**Move resources**</span></span>

<span data-ttu-id="a1e03-104">Tài nguyên Azure có thể được di chuyển đến một thuê bao Azure hoặc nhóm tài nguyên khác dưới cùng một thuê bao bằng Azure Portal, Azure PowerShell, Azure CLI, hoặc API REST để di chuyển tài nguyên.</span><span class="sxs-lookup"><span data-stu-id="a1e03-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="a1e03-105">Trước khi bạn có thể di chuyển tài nguyên, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="a1e03-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="a1e03-106">Danh sách kiểm tra trước khi di chuyển tài nguyên</span><span class="sxs-lookup"><span data-stu-id="a1e03-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="a1e03-107">Các dịch vụ có thể được di chuyển</span><span class="sxs-lookup"><span data-stu-id="a1e03-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="a1e03-108">Cách thức xác thực việc di chuyển</span><span class="sxs-lookup"><span data-stu-id="a1e03-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="a1e03-109">Di chuyển hướng dẫn cho các dịch vụ</span><span class="sxs-lookup"><span data-stu-id="a1e03-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="a1e03-110">Để di chuyển các tài nguyên hiện có sang một nhóm tài nguyên khác hoặc đăng ký, bạn có thể sử dụng:</span><span class="sxs-lookup"><span data-stu-id="a1e03-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="a1e03-111">Cổng thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="a1e03-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="a1e03-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="a1e03-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="a1e03-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="a1e03-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="a1e03-114">API REST</span><span class="sxs-lookup"><span data-stu-id="a1e03-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="a1e03-115">Hướng dẫn: [di chuyển các tài nguyên Azure đến một nhóm tài nguyên hoặc đăng ký khác](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="a1e03-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="a1e03-116">**Khắc phục sự cố lỗi với Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="a1e03-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="a1e03-117">Tham khảo các bài viết dưới đây để tìm hiểu về một số lỗi triển khai Azure thông thường và nhận thông tin để giải quyết chúng.</span><span class="sxs-lookup"><span data-stu-id="a1e03-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="a1e03-118">Nếu bạn không thể tìm thấy mã lỗi cho lỗi triển khai của mình, hãy xem [Tìm mã lỗi](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="a1e03-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="a1e03-119">Khắc phục sự cố lỗi triển khai</span><span class="sxs-lookup"><span data-stu-id="a1e03-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="a1e03-120">Khắc phục sự cố di chuyển tài nguyên Azure sang nhóm tài nguyên mới hoặc đăng ký</span><span class="sxs-lookup"><span data-stu-id="a1e03-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="a1e03-121">Lưu ý rằng nếu bạn muốn nâng cấp đăng ký Azure của mình, chẳng hạn như chuyển từ miễn phí sang thanh toán-như-bạn-đi, bạn sẽ cần phải chuyển đổi đăng ký của mình.</span><span class="sxs-lookup"><span data-stu-id="a1e03-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="a1e03-122">Để nâng cấp bản dùng thử miễn phí, hãy xem [nâng cấp bản dùng thử miễn phí hoặc Microsoft sẽ tưởng tượng đăng ký Azure để thanh toán-như-bạn-đi](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="a1e03-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="a1e03-123">Để thay đổi một tài khoản thanh toán-như-bạn-đi, hãy xem mục [thay đổi đăng ký Azure Pay-as-You-Go của bạn sang một ưu đãi khác nhau](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="a1e03-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="a1e03-124">**Để thêm hoặc liên kết một thuê bao Azure vào đối tượng thuê Azure Active Directory của bạn:**</span><span class="sxs-lookup"><span data-stu-id="a1e03-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="a1e03-125">Đăng nhập và chọn đăng ký mà bạn muốn sử dụng từ [trang đăng ký trong Azure Portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="a1e03-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="a1e03-126">Chọn **thay đổi thư mục**.</span><span class="sxs-lookup"><span data-stu-id="a1e03-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="a1e03-127">Xem lại mọi cảnh báo xuất hiện, rồi chọn **thay đổi**.</span><span class="sxs-lookup"><span data-stu-id="a1e03-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="a1e03-128">Thư mục được thay đổi cho đăng ký và bạn sẽ nhận được thông báo thành công.</span><span class="sxs-lookup"><span data-stu-id="a1e03-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="a1e03-129">Sử dụng nút *thư mục* để đi đến thư mục mới của bạn.</span><span class="sxs-lookup"><span data-stu-id="a1e03-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="a1e03-130">Có thể mất tối đa 10 phút để mọi thứ Hiển thị đúng cách.</span><span class="sxs-lookup"><span data-stu-id="a1e03-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="a1e03-131">**Tài liệu được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="a1e03-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="a1e03-132">Chuyển quyền sở hữu của một thuê bao Azure</span><span class="sxs-lookup"><span data-stu-id="a1e03-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="a1e03-133">Di chuyển tài nguyên đến nhóm tài nguyên mới hoặc thuê bao</span><span class="sxs-lookup"><span data-stu-id="a1e03-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="a1e03-134">Quản lý tài nguyên bằng Azure Portal</span><span class="sxs-lookup"><span data-stu-id="a1e03-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
