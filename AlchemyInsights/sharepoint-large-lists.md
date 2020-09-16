---
title: Danh sách lớn trong SharePoint
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720155"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="208d3-102">Làm việc với các danh sách và thư viện lớn trong SharePoint</span><span class="sxs-lookup"><span data-stu-id="208d3-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="208d3-103">Danh sách và thư viện SharePoint có thể chứa tối đa 30.000.000 mục, nhưng khi có hơn 5.000 mục, bạn có thể thấy lỗi ngưỡng dạng xem danh sách khi bạn tìm cách làm việc với họ.</span><span class="sxs-lookup"><span data-stu-id="208d3-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="208d3-104">Ngưỡng này được đặt tại chỗ để duy trì hiệu suất của dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="208d3-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="208d3-105">Không thể thay đổi nó.</span><span class="sxs-lookup"><span data-stu-id="208d3-105">It can't be changed.</span></span> <span data-ttu-id="208d3-106">Để tránh đánh ngưỡng này:</span><span class="sxs-lookup"><span data-stu-id="208d3-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="208d3-107">**Sử dụng hiện đại**</span><span class="sxs-lookup"><span data-stu-id="208d3-107">**Use modern**</span></span>

<span data-ttu-id="208d3-108">Các dạng xem Hiển thị nhiều mục hoạt động tốt nhất trong trải nghiệm hiện đại.</span><span class="sxs-lookup"><span data-stu-id="208d3-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="208d3-109">[Sử dụng trải nghiệm hiện đại](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) để tránh các lỗi mà bạn có thể thấy trong trải nghiệm cổ điển.</span><span class="sxs-lookup"><span data-stu-id="208d3-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="208d3-110">**Thêm chỉ mục**</span><span class="sxs-lookup"><span data-stu-id="208d3-110">**Add indexes**</span></span>

<span data-ttu-id="208d3-111">Khi bạn lọc hoặc sắp xếp theo một cột không có chỉ mục, bạn có thể thấy thông báo lỗi.</span><span class="sxs-lookup"><span data-stu-id="208d3-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="208d3-112">[Thêm chỉ mục](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) theo cách thủ công từ **thiết đặt danh sách** trong menu thiết đặt, sau đó được **lập chỉ mục cột**.</span><span class="sxs-lookup"><span data-stu-id="208d3-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="208d3-113">**Sửa dạng xem danh sách**</span><span class="sxs-lookup"><span data-stu-id="208d3-113">**Edit the list view**</span></span>

<span data-ttu-id="208d3-114">Nếu lỗi xảy ra khi làm việc với một danh sách lớn, hãy [sửa dạng xem danh sách của bạn](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="208d3-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="208d3-115">Bốn thay đổi sau đây sẽ loại bỏ các lỗi ngưỡng dạng xem danh sách.</span><span class="sxs-lookup"><span data-stu-id="208d3-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="208d3-116">Thực hiện tất cả bốn thay đổi để loại bỏ tất cả các lỗi.</span><span class="sxs-lookup"><span data-stu-id="208d3-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="208d3-117">Nếu bạn vẫn gặp phải lỗi, hãy kiểm tra [quản lý danh sách và thư viện lớn](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="208d3-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="208d3-118">Chọn **không** có từ cả hai **sắp xếp đầu tiên theo cột** và **sau đó sắp xếp theo cột**.</span><span class="sxs-lookup"><span data-stu-id="208d3-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="208d3-119">Chọn **không** có từ cả **nhóm đầu tiên của cột** và **sau đó nhóm theo cột**.</span><span class="sxs-lookup"><span data-stu-id="208d3-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="208d3-120">Chọn **không** cho tất cả các cột trong phần **tổng** .</span><span class="sxs-lookup"><span data-stu-id="208d3-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="208d3-121">Bỏ chọn tất cả nhưng một cột để hiển thị từ phần **cột** .</span><span class="sxs-lookup"><span data-stu-id="208d3-121">Deselect all but one column for display from the **Columns** section.</span></span>

