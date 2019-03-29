---
title: Hạn chế SharePoint Online để chế độ cổ điển
ms.author: kirks
author: Techwriter40
ms.date: 3/27/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 6e99da1c-e61d-40ba-855e-1a8f346e42fd
ms.openlocfilehash: 6a7c0497243ef7425917f54815e61f1244838c54
ms.sourcegitcommit: b14aa00b42ce4ca9d7dc3aa1fd57e66eae115447
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/28/2019
ms.locfileid: "30953366"
---
# <a name="restrict-sharepoint-online-to-classic-mode"></a><span data-ttu-id="a8be5-102">Hạn chế SharePoint Online để chế độ cổ điển</span><span class="sxs-lookup"><span data-stu-id="a8be5-102">Restrict SharePoint Online to classic mode</span></span>

<span data-ttu-id="a8be5-103">Một số tổ chức vẫn đòi hỏi kinh nghiệm chế độ cổ điển.</span><span class="sxs-lookup"><span data-stu-id="a8be5-103">Some organizations still require the Classic mode experience.</span></span> <span data-ttu-id="a8be5-104">Trong khi không có kế hoạch để loại bỏ các chế độ cổ điển ở một mức độ chi tiết, bắt đầu từ ngày 1,2019, nó sẽ không còn có thể giới hạn một tổ chức toàn bộ (thuê) để chế độ cổ điển cho các danh sách và thư viện.</span><span class="sxs-lookup"><span data-stu-id="a8be5-104">While there are no plans to remove classic mode at a granular level, starting April 1,2019, it will no longer be possible to restrict an entire organization (tenant) to classic mode for lists and libraries.</span></span>

<span data-ttu-id="a8be5-105">Các quản trị viên sẽ có các tùy chọn sau đây để quản lý danh sách cá nhân và thư viện trong chế độ cổ điển bằng cách sử dụng chi tiết lựa chọn thiết bị chuyển mạch mà chúng tôi cung cấp tại các đơn vị sau:</span><span class="sxs-lookup"><span data-stu-id="a8be5-105">The admin will have the following options to manage individual lists and libraries in classic mode using granular opt-out switches that we provide at the following levels:</span></span>

<span data-ttu-id="a8be5-106">--danh sách trang web bộ sưu tập--trang web----thư viện</span><span class="sxs-lookup"><span data-stu-id="a8be5-106">-- site collection -- site -- list -- library</span></span>

<span data-ttu-id="a8be5-107">Ngoài ra, danh sách sử dụng một số tính năng và tùy chỉnh mà không được hỗ trợ bởi hiện đại sẽ vẫn được tự động chuyển sang chế độ cổ điển.</span><span class="sxs-lookup"><span data-stu-id="a8be5-107">Additionally, lists that use certain features and customizations that are not supported by modern will still be automatically switched to classic mode.</span></span>

<span data-ttu-id="a8be5-108">Sau 1 tháng, danh sách và thư viện đang trong chế độ cổ điển là kết quả của người thuê nhà chọn không tham gia sẽ tự động được quản lý ở cấp độ trang web và danh sách cấp.</span><span class="sxs-lookup"><span data-stu-id="a8be5-108">After April 1, lists and libraries that are in classic mode as a result of tenant opt-out will automatically be managed at the site level and list level.</span></span>

<span data-ttu-id="a8be5-109">Nếu bạn yêu cầu chế độ cổ điển xin vui lòng xem thêm thông tin ở đây và PnP Powershell lệnh dưới đây mô tả tùy chọn và các công cụ bạn có thể sử dụng ngày nay để chuẩn bị cho việc loại bỏ người thuê nhà cấp lựa chọn ra ngày 1 tháng 4.</span><span class="sxs-lookup"><span data-stu-id="a8be5-109">If you require classic mode please see more information here and PnP Powershell instruction here that describes options and tools you can use today to prepare for the removal of the tenant level opt-out on April 1.</span></span>
