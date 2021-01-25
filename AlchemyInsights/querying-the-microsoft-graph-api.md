---
title: Truy vấn API của Microsoft graph
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
- "9004345"
- "7846"
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974691"
---
# <a name="querying-the-microsoft-graph-api"></a><span data-ttu-id="70392-102">Truy vấn API của Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-102">Querying the Microsoft Graph API</span></span>

<span data-ttu-id="70392-103">Chủ đề này cũng có thể áp dụng cho các nhà phát triển vẫn sử dụng API đồ thị Azure AD.</span><span class="sxs-lookup"><span data-stu-id="70392-103">This topic may also apply to developers still using Azure AD Graph API.</span></span> <span data-ttu-id="70392-104">Tuy nhiên, chúng **tôi khuyên bạn nên sử** dụng Microsoft graph cho tất cả các kịch bản, danh tính và tình huống quản lý truy nhập của bạn.</span><span class="sxs-lookup"><span data-stu-id="70392-104">However, it is **strongly** recommended that you use Microsoft Graph for all your directory, identity, and access management scenarios.</span></span>

<span data-ttu-id="70392-105">**Các vấn đề về xác thực hoặc ủy quyền**</span><span class="sxs-lookup"><span data-stu-id="70392-105">**Authentication or authorization issues**</span></span>

- <span data-ttu-id="70392-106">Nếu ứng dụng của bạn **không thể** có được thẻ để gọi tới Microsoft graph, hãy chọn **vấn đề với thể loại mã thông báo Access (xác thực)** Microsoft graph để biết thêm trợ giúp và hỗ trợ cụ thể về chủ đề này.</span><span class="sxs-lookup"><span data-stu-id="70392-106">If your app is **unable to acquire tokens** to call Microsoft Graph, pick **Problem with getting an access token (Authentication)** Microsoft Graph category to get more specific help and support on this topic.</span></span>
- <span data-ttu-id="70392-107">Nếu ứng dụng của bạn nhận được các **lỗi ủy quyền 401 hoặc 403** khi gọi cho Microsoft graph, hãy chọn thể loại **nhận được một lỗi truy nhập bị từ chối (ủy quyền)** Microsoft graph API để biết thêm trợ giúp và hỗ trợ cụ thể về chủ đề này.</span><span class="sxs-lookup"><span data-stu-id="70392-107">If your app is **receiving 401 or 403 authorization errors** when calling Microsoft Graph, pick the **Getting an access denied error (Authorization)** Microsoft Graph API category to get more specific help and support on this topic.</span></span>

<span data-ttu-id="70392-108">**Tôi muốn sử dụng Microsoft graph, nhưng không chắc chắn bắt đầu từ đâu**</span><span class="sxs-lookup"><span data-stu-id="70392-108">**I want to use Microsoft Graph, but not sure where to start**</span></span>

<span data-ttu-id="70392-109">Để tìm hiểu thêm về Microsoft graph, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="70392-109">To learn more about Microsoft Graph, see:</span></span>

- [<span data-ttu-id="70392-110">Tổng quan về Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-110">Overview of Microsoft Graph</span></span>](https://docs.microsoft.com/graph/overview)
- [<span data-ttu-id="70392-111">Tổng quan về danh tính và quản lý Access trong Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-111">Overview of Identity and Access Management in Microsoft Graph</span></span>](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [<span data-ttu-id="70392-112">Bước bắt đầu xây dựng ứng dụng Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-112">Getting started building Microsoft Graph apps</span></span>](https://docs.microsoft.com/graph/)
- <span data-ttu-id="70392-113">**Microsoft graph Explorer** -kiểm tra API của Microsoft graph trong đối tượng thuê của bạn hoặc đối tượng thuê giới thiệu</span><span class="sxs-lookup"><span data-stu-id="70392-113">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant</span></span>

<span data-ttu-id="70392-114">**Tôi muốn sử dụng Microsoft graph nhưng nó hỗ trợ các API của v 1,0 Directory tôi cần?**</span><span class="sxs-lookup"><span data-stu-id="70392-114">**I want to use Microsoft Graph, but does it support the v1.0 directory APIs I need?**</span></span>

<span data-ttu-id="70392-115">Microsoft graph là API được đề xuất cho thư mục, danh tính và quản lý Access.</span><span class="sxs-lookup"><span data-stu-id="70392-115">Microsoft Graph is the recommended API for directory, identity, and access management.</span></span> <span data-ttu-id="70392-116">Tuy nhiên, vẫn có một vài khoảng trống giữa những gì có thể có trong Azure AD graph và Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="70392-116">However, there are still a few gaps between what is possible in Azure AD Graph and Microsoft Graph.</span></span> <span data-ttu-id="70392-117">Xem lại các bài viết sau đây, trong đó sẽ tô sáng các điểm khác biệt Cập Nhật nhất để hỗ trợ trong lựa chọn của bạn:</span><span class="sxs-lookup"><span data-stu-id="70392-117">Review the following articles, which highlight the most up-to-date differences to assist in your choice:</span></span>

- [<span data-ttu-id="70392-118">Sự khác biệt về kiểu tài nguyên giữa Azure AD graph và Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-118">Resource type differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [<span data-ttu-id="70392-119">Sự khác biệt về tài sản giữa Azure AD graph và Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-119">Property differences between Azure AD Graph and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [<span data-ttu-id="70392-120">Sự khác biệt về phương pháp giữa Azure AD và đồ thị Microsoft</span><span class="sxs-lookup"><span data-stu-id="70392-120">Method differences between Azure AD and Microsoft Graph</span></span>](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

<span data-ttu-id="70392-121">**Khi tôi truy vấn đối tượng *người dùng* , nhiều thuộc tính của nó bị thiếu**</span><span class="sxs-lookup"><span data-stu-id="70392-121">**When I query the *user* object, many of its properties are missing**</span></span>

<span data-ttu-id="70392-122">`GET https://graph.microsoft.com/v1.0/users` chỉ trả về 11 thuộc tính, dưới dạng Microsoft graph tự động chọn một bộ thuộc tính *người dùng* mặc định để trả về.</span><span class="sxs-lookup"><span data-stu-id="70392-122">`GET https://graph.microsoft.com/v1.0/users` only returns 11 properties, as Microsoft Graph auto-selects a default set of *user* properties to return.</span></span> <span data-ttu-id="70392-123">Nếu bạn cần thuộc tính *người dùng* khác, hãy sử dụng $Select để chọn các thuộc tính nhu cầu ứng dụng của bạn.</span><span class="sxs-lookup"><span data-stu-id="70392-123">If you need other *user* properties, use $select to pick the properties your application needs.</span></span> <span data-ttu-id="70392-124">Dùng thử trong **Microsoft graph Explorer** trước tiên.</span><span class="sxs-lookup"><span data-stu-id="70392-124">Try it out in **Microsoft Graph Explorer** first.</span></span>

<span data-ttu-id="70392-125">**Một số giá trị thuộc tính của người dùng là *null* ngay cả khi tôi biết chúng được đặt**</span><span class="sxs-lookup"><span data-stu-id="70392-125">**Some user property values are *null* even though I know they are set**</span></span>

<span data-ttu-id="70392-126">Giải thích có khả năng nhất là ứng dụng đã được cấp cho *người dùng. ReadBasic. tất cả* quyền.</span><span class="sxs-lookup"><span data-stu-id="70392-126">The most likely explanation is that the application had been granted the *User.ReadBasic.All* permission.</span></span> <span data-ttu-id="70392-127">Điều này cho phép ứng dụng đọc một tập hợp các thuộc tính người dùng hạn chế, trả về tất cả các thuộc tính khác là NULL ngay cả khi họ đã thiết lập trước đó.</span><span class="sxs-lookup"><span data-stu-id="70392-127">This allows the application to read a limited set of user properties, returning all other properties as null even if they have been previously set.</span></span> <span data-ttu-id="70392-128">Hãy thử cấp cho *người dùng ứng dụng. đọc. tất cả* quyền thay thế.</span><span class="sxs-lookup"><span data-stu-id="70392-128">Try granting the application *User.Read.All* permission instead.</span></span>

<span data-ttu-id="70392-129">Để biết thêm thông tin, hãy xem quyền đối với [người dùng của Microsoft graph](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span><span class="sxs-lookup"><span data-stu-id="70392-129">For more information, see [Microsoft Graph user permissions](https://docs.microsoft.com/graph/permissions-reference#user-permissions).</span></span>

<span data-ttu-id="70392-130">**Tôi đang gặp sự cố khi sử dụng các tham số truy vấn OData để lọc dữ liệu trong yêu cầu của tôi**</span><span class="sxs-lookup"><span data-stu-id="70392-130">**I'm having trouble using OData query parameters to filter data in my requests**</span></span>

<span data-ttu-id="70392-131">Trong khi Microsoft graph hỗ trợ một phạm vi rộng của các tham số truy vấn OData, nhiều tham số trong số đó không được hỗ trợ đầy đủ bởi dịch vụ thư mục (các tài nguyên kế thừa từ *Directoryobject*) trong Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="70392-131">While Microsoft Graph supports a wide range of the OData query parameters, many of those parameters are not fully supported by directory services (resources that inherit from *directoryObject*) in Microsoft Graph.</span></span> <span data-ttu-id="70392-132">Những giới hạn tương tự được trình bày trong Azure AD graph vẫn tồn tại đối với hầu hết các phần trong Microsoft graph:</span><span class="sxs-lookup"><span data-stu-id="70392-132">The same limitations that were present in Azure AD Graph persist for the most part in Microsoft Graph:</span></span>

1. <span data-ttu-id="70392-133">**Không được hỗ trợ**: $count, $search và $Filter trên các giá trị *null* hoặc *không phải là NULL*</span><span class="sxs-lookup"><span data-stu-id="70392-133">**Not supported**: $count, $search, and $filter on *null* or *not null* values</span></span>
2. <span data-ttu-id="70392-134">**Không được hỗ trợ**: $Filter trên các thuộc tính nhất định (xem chủ đề tài nguyên mà bạn có thể lọc các thuộc tính nào)</span><span class="sxs-lookup"><span data-stu-id="70392-134">**Not supported**: $filter on certain properties (see resource topics on which properties are filterable)</span></span>
3. <span data-ttu-id="70392-135">**Không được hỗ trợ**: hoán trang, lọc và sắp xếp cùng lúc</span><span class="sxs-lookup"><span data-stu-id="70392-135">**Not supported**: paging, filtering, and sorting at the same time</span></span>
4. <span data-ttu-id="70392-136">**Không được hỗ trợ**: lọc trên mối quan hệ.</span><span class="sxs-lookup"><span data-stu-id="70392-136">**Not supported**: filtering on a relationship.</span></span> <span data-ttu-id="70392-137">Ví dụ-tìm tất cả các thành viên của nhóm kỹ thuật ở Vương Quốc Anh.</span><span class="sxs-lookup"><span data-stu-id="70392-137">For example - find all members of the engineering group that are in the UK.</span></span>
5. <span data-ttu-id="70392-138">**Hỗ trợ một phần**: $orderby trên *người dùng* (DisplayName và userPrincipalName chỉ) và *nhóm*</span><span class="sxs-lookup"><span data-stu-id="70392-138">**Partial support**: $orderby on *user* (displayName and userPrincipalName only) and *group*</span></span>
6. <span data-ttu-id="70392-139">**Hỗ trợ một phần**: $Filter (chỉ hỗ trợ các *EQ*, *Startswith*, *or* *và và* giới hạn *nào*) hỗ trợ, $Expand (mở rộng mối quan hệ của một đối tượng trả về tất cả mối quan hệ, nhưng mở rộng tập hợp mối quan hệ của đối tượng được giới hạn)</span><span class="sxs-lookup"><span data-stu-id="70392-139">**Partial support**: $filter (supports only *eq*, *startswith*, *or*, *and*, and limited *any*) support, $expand (expanding a single object's relationships returns all relationships, but expanding a collection of objects' relationships is limited)</span></span>

<span data-ttu-id="70392-140">Để biết thêm thông tin, hãy xem [tùy chỉnh phản hồi với tham số truy vấn](https://docs.microsoft.com/graph/query-parameters).</span><span class="sxs-lookup"><span data-stu-id="70392-140">For more information, see [Customize responses with query parameters](https://docs.microsoft.com/graph/query-parameters).</span></span>

<span data-ttu-id="70392-141">**API tôi đang gọi không hoạt động-tôi có thể làm việc kiểm tra khác ở đâu?**</span><span class="sxs-lookup"><span data-stu-id="70392-141">**The API I'm calling doesn't work - where can I do more testing?**</span></span>

<span data-ttu-id="70392-142">**Microsoft graph Explorer** -kiểm tra API đồ thị Microsoft trong đối tượng thuê của bạn hoặc đối tượng thuê giới thiệu và cũng có thể xem các **truy vấn mẫu** trong Microsoft graph Explorer.</span><span class="sxs-lookup"><span data-stu-id="70392-142">**Microsoft Graph Explorer** - Test Microsoft Graph APIs in your tenant or a demo tenant and also check out the **sample queries** in Microsoft Graph Explorer.</span></span>

<span data-ttu-id="70392-143">**Khi tôi truy vấn dữ liệu có vẻ như tôi nhận được thiết lập dữ liệu không đầy đủ**</span><span class="sxs-lookup"><span data-stu-id="70392-143">**When I query for data it seems like I get an incomplete data set back**</span></span>

<span data-ttu-id="70392-144">Nếu bạn đang truy vấn một tuyển tập (như *người dùng*), Microsoft graph sẽ sử dụng giới hạn trang phía máy chủ để kết quả luôn được trả về bằng một kích cỡ trang mặc định.</span><span class="sxs-lookup"><span data-stu-id="70392-144">If you are querying a collection (like *users*), Microsoft Graph uses server-side page limits so results are always returned with a default page-size.</span></span> <span data-ttu-id="70392-145">Ứng dụng của bạn sẽ luôn mong đợi đến trang thông qua các bộ sưu tập trả về từ dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="70392-145">Your app should always expect to page through collections returned from the service.</span></span>

<span data-ttu-id="70392-146">Để biết thêm thông tin, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="70392-146">For more information, see:</span></span>

- [<span data-ttu-id="70392-147">Các biện pháp tốt nhất của Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-147">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="70392-148">Dữ liệu biểu đồ Microsoft phân trang trong ứng dụng của bạn</span><span class="sxs-lookup"><span data-stu-id="70392-148">Paging Microsoft Graph data in your app</span></span>](https://docs.microsoft.com/graph/paging)

<span data-ttu-id="70392-149">**Ứng dụng của tôi quá chậm và cũng đang nhận được Throttled. Tôi có thể thực hiện những cải thiện nào?**</span><span class="sxs-lookup"><span data-stu-id="70392-149">**My app is too slow and is also getting throttled. What improvements can I make?**</span></span>

<span data-ttu-id="70392-150">Tùy thuộc vào tình huống của bạn, có nhiều tùy chọn khác nhau trong việc xử lý của bạn để làm cho ứng dụng của bạn thêm performant, và trong một số trường hợp, ít dễ bị hơn là Throttled bởi dịch vụ (khi bạn đang thực hiện quá nhiều cuộc gọi).</span><span class="sxs-lookup"><span data-stu-id="70392-150">Depending on your scenario, there are a variety of different options at your disposal to make your application more performant, and in some cases, less prone to being throttled by the service (when you are making too many calls).</span></span>

<span data-ttu-id="70392-151">Để tìm hiểu thêm, hãy xem:</span><span class="sxs-lookup"><span data-stu-id="70392-151">To learn more, see:</span></span>

- [<span data-ttu-id="70392-152">Các biện pháp tốt nhất của Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-152">Microsoft Graph best practices</span></span>](https://docs.microsoft.com/graph/best-practices-concept)
- [<span data-ttu-id="70392-153">Các yêu cầu về định lượng</span><span class="sxs-lookup"><span data-stu-id="70392-153">Batching requests</span></span>](https://docs.microsoft.com/graph/json-batching)
- [<span data-ttu-id="70392-154">Theo dõi thay đổi thông qua truy vấn đồng bằng</span><span class="sxs-lookup"><span data-stu-id="70392-154">Track changes through delta query</span></span>](https://docs.microsoft.com/graph/delta-query-overview)
- [<span data-ttu-id="70392-155">Nhận thông báo về các thay đổi thông qua webhooks</span><span class="sxs-lookup"><span data-stu-id="70392-155">Get notified of changes through webhooks</span></span>](https://docs.microsoft.com/graph/webhooks)
- [<span data-ttu-id="70392-156">Hướng dẫn throttling</span><span class="sxs-lookup"><span data-stu-id="70392-156">Throttling guidance</span></span>](https://docs.microsoft.com/graph/throttling)

<span data-ttu-id="70392-157">**Tôi có thể tìm thêm thông tin về các lỗi và các vấn đề đã biết ở đâu?**</span><span class="sxs-lookup"><span data-stu-id="70392-157">**Where can I find more information on errors and known issues?**</span></span>

- [<span data-ttu-id="70392-158">Thông tin phản hồi về lỗi của Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-158">Microsoft Graph error response information</span></span>](https://docs.microsoft.com/graph/errors)
- [<span data-ttu-id="70392-159">Các vấn đề đã biết với Microsoft graph</span><span class="sxs-lookup"><span data-stu-id="70392-159">Known issues with Microsoft Graph</span></span>](https://docs.microsoft.com/graph/known-issues)

<span data-ttu-id="70392-160">**Tôi có thể kiểm tra trạng thái sẵn dùng và khả năng kết nối của dịch vụ ở đâu?**</span><span class="sxs-lookup"><span data-stu-id="70392-160">**Where can I check status of service availability and connectivity?**</span></span>

<span data-ttu-id="70392-161">Tính khả dụng của dịch vụ và kết nối của các dịch vụ cơ bản có thể được truy nhập thông qua Microsoft graph có thể ảnh hưởng đến tính khả dụng tổng thể và hiệu suất của Microsoft graph.</span><span class="sxs-lookup"><span data-stu-id="70392-161">The service availability and connectivity of the underlying services that can be accessed through Microsoft Graph can impact the overall availability and performance of Microsoft Graph.</span></span>

- <span data-ttu-id="70392-162">Đối với dịch vụ Azure Active Directory Health, hãy kiểm tra trạng thái của dịch vụ **danh tính + bảo mật** được liệt kê trong [trang trạng thái Azure](https://azure.microsoft.com/status/).</span><span class="sxs-lookup"><span data-stu-id="70392-162">For Azure Active Directory service health, check the status of **Security + Identity** services listed in the [Azure status page](https://azure.microsoft.com/status/).</span></span>
- <span data-ttu-id="70392-163">Đối với các dịch vụ Office đóng góp vào Microsoft graph, hãy kiểm tra trạng thái các dịch vụ được liệt kê trong bảng điều khiển trạng thái [dịch vụ Office](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="70392-163">For Office services that contribute to Microsoft Graph, check the status of services listed in the [Office Service Health Dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>
