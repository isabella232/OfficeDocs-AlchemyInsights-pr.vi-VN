---
title: Đặt cấu hình dịch vụ đồng bộ MIM
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
- "8472"
- "9004688"
ms.openlocfilehash: 48e9a0e8c26088b690092bfaedfba641841739f6
ms.sourcegitcommit: 379e132c4d21ecf703d5506484ec96a767fdda39
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482892"
---
# <a name="configure-mim-sync-service"></a><span data-ttu-id="a5373-102">Đặt cấu hình dịch vụ đồng bộ MIM</span><span class="sxs-lookup"><span data-stu-id="a5373-102">Configure MIM Sync service</span></span>

<span data-ttu-id="a5373-103">Dịch vụ đồng bộ hóa Microsoft Identity Manager (MIM) là một thành phần của MIM.</span><span class="sxs-lookup"><span data-stu-id="a5373-103">Microsoft Identity Manager (MIM) Synchronization Service is a component of MIM.</span></span> <span data-ttu-id="a5373-104">Đây là dịch vụ tại cơ sở tập trung lưu trữ và tích hợp thông tin cho các tổ chức có nhiều thư mục và cơ sở dữ liệu tại chỗ.</span><span class="sxs-lookup"><span data-stu-id="a5373-104">It is a centralized on-premises service that stores and integrates information for organizations that have multiple on-premises directories and databases.</span></span> <span data-ttu-id="a5373-105">Bạn có thể giải quyết vấn đề của mình với MIM đồng bộ nếu sự cố này đã được giải quyết trong bản cập nhật gần đây cho MIM hoặc là một trong các vấn đề khác được đề cập trong phần dưới đây.</span><span class="sxs-lookup"><span data-stu-id="a5373-105">You may be able to resolve your problem with MIM Sync if the issue was addressed in a recent update to MIM or is one of the other issues mentioned in the below section.</span></span>

<span data-ttu-id="a5373-106">**Các bước được đề xuất**</span><span class="sxs-lookup"><span data-stu-id="a5373-106">**Recommended steps**</span></span>

1. <span data-ttu-id="a5373-107">Đảm bảo rằng bạn đang sử dụng bản cập nhật gần đây về MIM đồng bộ và kiểm tra [ghi chú bản phát hành MIM Sync](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) để xác định xem vấn đề đã được giải quyết trong bản Cập Nhật hay không.</span><span class="sxs-lookup"><span data-stu-id="a5373-107">Ensure that you are using a recent update of MIM Sync and check the [MIM Sync release notes](https://docs.microsoft.com/microsoft-identity-manager/reference/version-history) to determine if the issue has been resolved in an update.</span></span>
2. <span data-ttu-id="a5373-108">Nếu vấn đề là với LDAP chung, SQL chung chung, Lotus Domino hoặc trình kết nối dịch vụ web, hãy đảm bảo rằng bạn đang sử dụng bản cập nhật gần đây của các đường kết [nối chung](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span><span class="sxs-lookup"><span data-stu-id="a5373-108">If the problem is with the Generic LDAP, Generic SQL, Lotus Domino or Web Services connector, ensure that you are using a recent update of the [generic connectors](https://docs.microsoft.com/microsoft-identity-manager/reference/microsoft-identity-manager-2016-connector-version-history).</span></span>
3. <span data-ttu-id="a5373-109">Nếu điểm dừng đồng bộ chạy MIM với lỗi, hãy tham khảo bảng của các [mã lỗi chạy](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) để xác định các nguyên nhân tiềm ẩn.</span><span class="sxs-lookup"><span data-stu-id="a5373-109">If an MIM Sync-run stops with an error, consult the table of [run error codes](https://docs.microsoft.com/microsoft-identity-manager/reference/maerrorcodes) to determine the potential causes.</span></span>
4. <span data-ttu-id="a5373-110">Nếu các điểm dừng chạy với **phần mở rộng-dll-ngoại lệ**, sau đó bấm vào những từ này để mở cửa sổ **thuộc tính không gian kết nối** , rồi bấm vào theo **dõi stack...** để xem thêm thông tin về nguyên nhân cơ bản, như được mô tả trong [phần mở rộng-dll-ngoại lệ](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span><span class="sxs-lookup"><span data-stu-id="a5373-110">If the run stops with **extension-dll-exception**, then click on those words to open the **Connector Space Object properties** window, and click on **Stack Trace...** to see more information on the underlying cause, as described in [Extension-DLL-Exception](https://social.technet.microsoft.com/wiki/contents/articles/7515.fim-troubleshooting-extension-dll-exception.aspx).</span></span>
5. <span data-ttu-id="a5373-111">Nếu lỗi cấu phần dịch vụ thông báo thay đổi mật khẩu (PCNS), hãy chọn **6025** trong Nhật ký sự kiện khi đồng bộ hóa mật khẩu, đánh dấu phần hướng dẫn khắc phục sự cố [lỗi báo cáo PCNS 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span><span class="sxs-lookup"><span data-stu-id="a5373-111">If the Password Change Notification Service (PCNS) component reports **error 6025** in the event log during password synchronization, check the guide for troubleshooting [PCNS reporting error 6025](https://social.technet.microsoft.com/wiki/contents/articles/4159.pcns-troubleshooting-event-id-6025.aspx).</span></span>
6. <span data-ttu-id="a5373-112">Nếu việc đồng bộ hóa đầy đủ với tác nhân quản lý Dịch vụ FIM là chậm, hãy kiểm tra cài đặt **tự động phát triển** cho TempDB, như được mô tả trong [khắc phục sự cố chậm hoặc treo đồng bộ hóa đầy đủ](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span><span class="sxs-lookup"><span data-stu-id="a5373-112">If full synchronization with the FIM Service Management Agent is slow, check the **auto grow** setting for TempDB, as described in [Troubleshooting slow or hanging full synchronization](https://social.technet.microsoft.com/wiki/contents/articles/14713.troubleshooting-fim-performance-slow-or-hanging-full-synchronization.aspx).</span></span>
7. <span data-ttu-id="a5373-113">Nếu bạn đang gặp phải lỗi dừng máy chủ với không thành công-qua-dịch vụ web bằng cách sử dụng tác nhân quản lý Dịch vụ FIM, hãy xem mục [hỗ trợ-thông tin: không thành công-thông qua-web-dịch vụ](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) để biết tổng quan về các nguyên nhân.</span><span class="sxs-lookup"><span data-stu-id="a5373-113">If you are encountering an error of stopped-server with failed-creation-via-web-services using the FIM Service Management Agent, see [Support-Info: failed-creation-via-web-services](https://docs.microsoft.com/archive/blogs/iamsupport/support-info-fimma-failed-creation-via-web-services) for an overview of causes.</span></span>

