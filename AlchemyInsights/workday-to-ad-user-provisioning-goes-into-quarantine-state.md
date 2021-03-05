---
title: Ngày làm việc của người dùng quảng cáo đi sâu vào trạng thái cách ly
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8471"
- "9004687"
ms.openlocfilehash: 0fc519c8170de498c9bcb1fc41a76116bda48b1f
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482909"
---
# <a name="workday-to-ad-user-provisioning-goes-into-quarantine-state"></a><span data-ttu-id="62215-102">Ngày làm việc của người dùng quảng cáo đi sâu vào trạng thái cách ly</span><span class="sxs-lookup"><span data-stu-id="62215-102">Workday to AD User Provisioning goes into quarantine state</span></span>

<span data-ttu-id="62215-103">**Ngày làm việc đến cấp phép người dùng quảng cáo đi sâu vào trạng thái kiểm soát và không người nào được tạo trong AD**</span><span class="sxs-lookup"><span data-stu-id="62215-103">**Workday to AD User Provisioning goes into quarantine state and no users are created in AD**</span></span>

<span data-ttu-id="62215-104">Ngày làm việc cho người dùng quảng cáo cung cấp công việc đã đi vào trạng thái cách ly và Nhật ký kiểm tra Hiển thị các sự kiện lỗi xuất hiện với lỗi thông báo lỗi **: OperationsError-SvcErr: một lỗi thao tác xảy ra. Không có tham chiếu vượt trội nào đã được cấu hình cho dịch vụ thư mục. Dịch vụ thư mục do đó không thể phát hiện các đối tượng được giới thiệu bên ngoài rừng này**.</span><span class="sxs-lookup"><span data-stu-id="62215-104">The Workday to AD User Provisioning job has gone into quarantine state and the audit logs show export failure events with the error message **Error: OperationsError-SvcErr: An operation error occurred. No superior reference has been configured for the directory service. The directory service is therefore unable to issue referrals to objects outside this forest**.</span></span> <span data-ttu-id="62215-105">Lỗi này thường hiển thị nếu bộ chứa Active Directory OU không được đặt đúng hoặc nếu có vấn đề với ánh xạ biểu thức được sử dụng cho **Parentused Shedname**.</span><span class="sxs-lookup"><span data-stu-id="62215-105">This error usually shows up if the Active Directory Container OU is not set correctly or if there are issues with the Expression Mapping used for **parentDistinguishedName**.</span></span>

<span data-ttu-id="62215-106">Chọn tham số OU mặc định cho **người dùng mới** cho lỗi chính tả.</span><span class="sxs-lookup"><span data-stu-id="62215-106">Check the Default OU for **New Users** parameter for typos.</span></span> <span data-ttu-id="62215-107">Đảm bảo rằng OU đã xác định đã tồn tại trong quảng cáo của bạn.</span><span class="sxs-lookup"><span data-stu-id="62215-107">Ensure that the specified OU already exists in your AD.</span></span> <span data-ttu-id="62215-108">Nếu bạn đang sử dụng **Parentscn shedname** trong ánh xạ thuộc tính, hãy đảm bảo rằng nó luôn được đánh giá là một bộ chứa đã biết trong tên miền quảng cáo.</span><span class="sxs-lookup"><span data-stu-id="62215-108">If you are using **parentDistinguishedName** in the attribute mapping, ensure that it always evaluates to a known container within the AD domain.</span></span> <span data-ttu-id="62215-109">Kiểm tra sự kiện xuất trong Nhật ký kiểm nghiệm để xem giá trị được tạo ra.</span><span class="sxs-lookup"><span data-stu-id="62215-109">Check the Export event in the audit logs to see the generated value.</span></span>

<span data-ttu-id="62215-110">Để biết thêm chi tiết về cách đặt cấu hình ngày làm việc cho tính năng cung cấp tự động, hãy xem [hướng dẫn: cấu hình ngày làm việc cho người dùng tự động cung](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial)cấp.</span><span class="sxs-lookup"><span data-stu-id="62215-110">For more details on configuring workday for automated provisioning, see [Tutorial: Configure Workday for automatic user provisioning](https://docs.microsoft.com/azure/active-directory/saas-apps/workday-inbound-tutorial).</span></span>

