---
title: Trang web hiện đại như là trang web gốc
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid:
- "9000153"
- "1692"
ms.openlocfilehash: 6f55f1c63551027cc5522d296cb3f3f342356d95
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 10/18/2019
ms.locfileid: "36576708"
---
# <a name="modernize-your-classic-sharepoint-site"></a><span data-ttu-id="1574b-102">Hiện đại hoá trang web SharePoint cổ điển của bạn</span><span class="sxs-lookup"><span data-stu-id="1574b-102">Modernize your classic SharePoint site</span></span>

<span data-ttu-id="1574b-103">Để thực hiện chuyển đổi sang giao diện người dùng hiện đại, bạn cần tập trung vào các mục sau:</span><span class="sxs-lookup"><span data-stu-id="1574b-103">To make the switch to a modern user interface, you need to focus on the following:</span></span>

- <span data-ttu-id="1574b-104">Chuyển **danh sách và thư viện** của bạn để sử dụng giao diện người dùng hiện đại (còn được gọi là danh sách hiện đại và trải nghiệm thư viện).</span><span class="sxs-lookup"><span data-stu-id="1574b-104">Transitioning your **lists and libraries** to use the modern user interface (also referred to as the modern list and library experience).</span></span>
- <span data-ttu-id="1574b-105">Chuyển đổi các trang **web** của bạn từ wiki cổ điển và các trang web phần vào trang khách hàng hiện đại-Side.</span><span class="sxs-lookup"><span data-stu-id="1574b-105">Transforming your **site pages** from classic wiki and web part pages into modern client-side pages.</span></span>
- <span data-ttu-id="1574b-106">Tạo **các trang web hiện đại** (trang web nhóm hoặc trang web liên lạc).</span><span class="sxs-lookup"><span data-stu-id="1574b-106">Creating **modern sites** (Team site or Communication Site).</span></span>

<span data-ttu-id="1574b-107">Hiện đại hoá trải nghiệm của bạn bằng:</span><span class="sxs-lookup"><span data-stu-id="1574b-107">Modernize your experience by:</span></span>
- <span data-ttu-id="1574b-108">[Cho phép các danh sách và thư viện Hiển thị trong giao diện người dùng hiện đại](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries) bằng cách thay thế tùy chỉnh, loại bỏ các cột không tương thích khỏi các dạng xem đã sử dụng hoặc (như là một khu nghỉ mát cuối cùng) di chuyển dữ liệu vào một loại danh sách tương thích với giao diện người dùng hiện đại.</span><span class="sxs-lookup"><span data-stu-id="1574b-108">[Enabling lists and libraries to show in the modern user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-lists-and-libraries) by replacing customizations, removing incompatible columns from the used views, or (as a last resort) moving data into a modern user interface-compatible list type.</span></span>
- <span data-ttu-id="1574b-109">[Kết nối trang web của bạn với nhóm Office 365](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group), cung cấp cho trang web của bạn một trang chủ hiện đại và cho phép trang web của bạn sử dụng, ví dụ: hộp thư hoặc Microsoft Planner.</span><span class="sxs-lookup"><span data-stu-id="1574b-109">[Connecting your site to an Office 365 group](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group), which gives your site a modern home page and enables your site to use, for example, a mailbox or Microsoft Planner.</span></span> <span data-ttu-id="1574b-110">Điều này cho phép bạn sử dụng phiên bản hiện đại của lịch và danh sách tác vụ.</span><span class="sxs-lookup"><span data-stu-id="1574b-110">This enables you to use a modern version of a calendar and task list.</span></span>
- <span data-ttu-id="1574b-111">[Tạo các trang hiện đại](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec), là một cách tuyệt vời để chia sẻ ý tưởng bằng cách sử dụng hình ảnh, Excel, Word và PowerPoint tài liệu, video, và nhiều hơn nữa.</span><span class="sxs-lookup"><span data-stu-id="1574b-111">[Creating modern pages](https://support.office.com/article/create-and-use-modern-pages-on-a-sharepoint-site-b3d46deb-27a6-4b1e-87b8-df851e503dec), is a great way to share ideas using images, Excel, Word and PowerPoint documents, video, and more.</span></span>
- <span data-ttu-id="1574b-112">[Tạo các trang khách hàng hiện đại](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages) và cấu hình chúng là "tương tự" với trang wiki cổ điển và phần web của bạn.</span><span class="sxs-lookup"><span data-stu-id="1574b-112">[Creating modern client-side pages](https://docs.microsoft.com/sharepoint/dev/transform/modernize-userinterface-site-pages) and configuring these to be "similar" to your key classic wiki and web part pages.</span></span> <span data-ttu-id="1574b-113">Chương trình chuyển đổi trang phải được thực hiện cho các trang chủ chốt của các trang web của bạn, như biến tất cả các trang là tài nguyên chuyên sâu và thường không cần thiết.</span><span class="sxs-lookup"><span data-stu-id="1574b-113">Programmatic page transformation should be done for the key pages of your sites, as transforming all pages is resource-intensive and often not needed.</span></span> <span data-ttu-id="1574b-114">Để hỗ trợ trong phần ba này, máy quét hiện đại hóa SharePoint có thể cung cấp cho bạn thông tin sử dụng về các trang wiki và web.</span><span class="sxs-lookup"><span data-stu-id="1574b-114">To assist in this triage, the SharePoint Modernization scanner can give you usage information about the current wiki and web part pages.</span></span>
- <span data-ttu-id="1574b-115">[Tạo ra các trang web hiện đại](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="1574b-115">[Creating modern sites](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span> <span data-ttu-id="1574b-116">Tôi có nên tạo một site nhóm hoặc một site liên lạc không?</span><span class="sxs-lookup"><span data-stu-id="1574b-116">Should I create a team site or a communication site?</span></span>

<span data-ttu-id="1574b-117">Thông tin bổ sung:</span><span class="sxs-lookup"><span data-stu-id="1574b-117">Additional Info:</span></span> 
- <span data-ttu-id="1574b-118">Để biết tổng quan từng bước về hiện đại hóa các trang web SharePoint cổ điển của bạn với trải nghiệm Modern, hãy xem tân [trang các site SharePoint cổ điển của](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites)bạn.</span><span class="sxs-lookup"><span data-stu-id="1574b-118">For a step-by-step overview of modernizing your classic SharePoint Sites to the modern experience, see [Modernize your classic SharePoint Sites](https://docs.microsoft.com/sharepoint/dev/transform/modernize-classic-sites).</span></span>
- <span data-ttu-id="1574b-119">Xem hướng dẫn về [trải nghiệm hiện đại](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience).</span><span class="sxs-lookup"><span data-stu-id="1574b-119">See a guide to [Modern Experience](https://docs.microsoft.com/sharepoint/guide-to-sharepoint-modern-experience).</span></span>
- <span data-ttu-id="1574b-120">Xem [trải nghiệm SharePoint Classic và hiện đại](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f).</span><span class="sxs-lookup"><span data-stu-id="1574b-120">See [SharePoint Classic and Modern experiences](https://support.office.com/article/sharepoint-classic-and-modern-experiences-5725c103-505d-4a6e-9350-300d3ec7d73f).</span></span> 




