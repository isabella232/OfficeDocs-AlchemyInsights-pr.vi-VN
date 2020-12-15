---
title: Cho phép quản lý chi phí
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 12/08/2020
ms.locfileid: "49678777"
---
# <a name="enable-cost-management"></a><span data-ttu-id="5a666-102">Cho phép quản lý chi phí</span><span class="sxs-lookup"><span data-stu-id="5a666-102">Enable cost management</span></span>

<span data-ttu-id="5a666-103">**' Chi phí nào bị vô hiệu cho tổ chức của bạn có nghĩa là gì?**</span><span class="sxs-lookup"><span data-stu-id="5a666-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="5a666-104">Các tổ chức sử dụng thỏa thuận doanh nghiệp (EA) hoặc các tài khoản thỏa thuận Microsoft customer (MCA) có thể tắt quyền truy nhập vào thông tin chi phí và thông tin về giá.</span><span class="sxs-lookup"><span data-stu-id="5a666-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="5a666-105">Sau khi đăng nhập vào Azure Portal, họ có thể sử dụng các API thanh toán để lập trình các hóa đơn (sau khi chọn tham gia) và chi tiết về mức sử dụng.</span><span class="sxs-lookup"><span data-stu-id="5a666-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="5a666-106">**Cách để cho phép người dùng bổ sung truy nhập hóa đơn**</span><span class="sxs-lookup"><span data-stu-id="5a666-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="5a666-107">Đi đến **lưỡi đăng ký** trong Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="5a666-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="5a666-108">Chọn hóa **đơn** và sau đó **truy nhập vào hóa đơn**.</span><span class="sxs-lookup"><span data-stu-id="5a666-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="5a666-109">Bật truy nhập, tiếp theo là lưu các thay đổi, để cho phép người dùng trong vai trò đăng ký-phạm vi để tải xuống hóa đơn.</span><span class="sxs-lookup"><span data-stu-id="5a666-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="5a666-110">Người quản trị tài khoản cũng có thể cấu hình để có các hóa đơn được gửi qua email.</span><span class="sxs-lookup"><span data-stu-id="5a666-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="5a666-111">Để tìm hiểu thêm, hãy xem [mục nhận hóa đơn của bạn trong email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="5a666-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="5a666-112">**Cách thêm người dùng vào vai trò bộ đọc thanh toán**</span><span class="sxs-lookup"><span data-stu-id="5a666-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="5a666-113">Đi đến **lưỡi đăng ký** trong Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="5a666-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="5a666-114">Chọn **Access Control (iam)** , rồi bấm **Thêm**.</span><span class="sxs-lookup"><span data-stu-id="5a666-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="5a666-115">Chọn bộ **đọc thanh toán** trong trang **chọn vai trò** .</span><span class="sxs-lookup"><span data-stu-id="5a666-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="5a666-116">Nhập email của người dùng mà bạn muốn mời, rồi bấm **OK** để gửi lời mời.</span><span class="sxs-lookup"><span data-stu-id="5a666-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="5a666-117">Làm theo hướng dẫn được cung cấp trong email mời để đăng nhập với tư cách là bộ đọc thanh toán.</span><span class="sxs-lookup"><span data-stu-id="5a666-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="5a666-118">Để biết thêm thông tin, hãy xem [cấp quyền truy nhập vào thanh toán](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="5a666-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="5a666-119">**Tài liệu được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="5a666-119">**Recommended documents**</span></span>

- [<span data-ttu-id="5a666-120">Kích hoạt các dạng xem DA và AO qua EA Portal</span><span class="sxs-lookup"><span data-stu-id="5a666-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="5a666-121">Chi phí bao gồm trong quản lý chi phí</span><span class="sxs-lookup"><span data-stu-id="5a666-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="5a666-122">Cung cấp Microsoft Azure được hỗ trợ</span><span class="sxs-lookup"><span data-stu-id="5a666-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="5a666-123">Xem lại chi phí trong phân tích chi phí</span><span class="sxs-lookup"><span data-stu-id="5a666-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="5a666-124">Cung cấp quyền truy nhập vào thông tin thanh toán</span><span class="sxs-lookup"><span data-stu-id="5a666-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="5a666-125">Kiểm tra quyền truy nhập vào thỏa thuận khách hàng của Microsoft</span><span class="sxs-lookup"><span data-stu-id="5a666-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






