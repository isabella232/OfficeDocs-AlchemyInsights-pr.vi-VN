---
title: Nhật ký và báo cáo
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
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036102"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="ce1af-102">Nhật ký và báo cáo</span><span class="sxs-lookup"><span data-stu-id="ce1af-102">Logs and Reporting</span></span>

<span data-ttu-id="ce1af-103">Câu hỏi [thường gặp về Azure Active Directory](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) câu hỏi thường gặp về báo cáo Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="ce1af-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="ce1af-104">Để biết thêm thông tin, hãy xem [báo cáo Azure Active Directory](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span><span class="sxs-lookup"><span data-stu-id="ce1af-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="ce1af-105">**Khắc phục sự cố về kiểm tra**</span><span class="sxs-lookup"><span data-stu-id="ce1af-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="ce1af-106">Nếu bạn đang gặp vấn đề khi thấy một số hoạt động kiểm nghiệm và hoạt động bị thiếu nằm trong [danh sách](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities)này, vui lòng gửi một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="ce1af-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="ce1af-107">Nếu bạn đang gặp vấn đề khi thấy bất kỳ Nhật ký kiểm tra nào trong đối tượng thuê của mình, vui lòng gửi một vé hỗ trợ.</span><span class="sxs-lookup"><span data-stu-id="ce1af-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="ce1af-108">Nếu các hoạt động kiểm nghiệm của bạn không hiển thị ngay lập tức trong cổng thông tin Azure, hãy xem [thông tin về độ trễ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) của chúng tôi và gửi một vé hỗ trợ nếu sự chậm trễ vượt quá độ trễ của tài liệu.</span><span class="sxs-lookup"><span data-stu-id="ce1af-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="ce1af-109">Duy trì ghi nhật ký hoạt động Azure AD</span><span class="sxs-lookup"><span data-stu-id="ce1af-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="ce1af-110">Nếu bạn không nhìn thấy tất cả kiểm nghiệm cho phạm vi ngày bạn đã chọn, bạn có thể tải lên đến 250K hàng (được sắp xếp theo gần đây nhất) của các đăng nhập từ Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ce1af-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="ce1af-111">Để biết thêm thông tin, hãy xem [tải xuống các hoạt động kiểm](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report)nghiệm.</span><span class="sxs-lookup"><span data-stu-id="ce1af-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="ce1af-112">**Khắc phục sự cố với đăng nhập**</span><span class="sxs-lookup"><span data-stu-id="ce1af-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="ce1af-113">Bạn chỉ có thể nhìn thấy 30 ngày cuối cùng của dữ liệu nếu bạn có giấy phép Azure AD Premium (P1 hoặc P2) cho đối tượng thuê của bạn.</span><span class="sxs-lookup"><span data-stu-id="ce1af-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="ce1af-114">Đăng nhập chỉ khả dụng cho các đối tượng thuê Azure AD Premium.</span><span class="sxs-lookup"><span data-stu-id="ce1af-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="ce1af-115">Nó không sẵn dùng đối với người thuê cơ bản miễn phí hoặc được cấp phép.</span><span class="sxs-lookup"><span data-stu-id="ce1af-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="ce1af-116">Nếu đối tượng thuê của bạn có giấy phép P1 Premium và bạn không nhìn thấy các đăng nhập, hãy kiểm tra [thông tin về độ trễ](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) của chúng tôi và gửi một vé hỗ trợ nếu sự chậm trễ vượt quá độ trễ tài liệu.</span><span class="sxs-lookup"><span data-stu-id="ce1af-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="ce1af-117">Nếu bạn không nhìn thấy tất cả các đăng nhập cho phạm vi ngày bạn đã chọn, hãy lưu ý rằng bạn có thể tải lên đến 250K hàng (được sắp xếp theo gần đây nhất) của các đăng nhập từ Azure Portal.</span><span class="sxs-lookup"><span data-stu-id="ce1af-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="ce1af-118">Để biết thêm thông tin, hãy xem [tải xuống các hoạt động đăng nhập](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="ce1af-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="ce1af-119">**Khắc phục sự cố báo cáo bảo mật (người dùng gắn cờ có nguy cơ, đăng nhập rủi ro)**</span><span class="sxs-lookup"><span data-stu-id="ce1af-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="ce1af-120">Người dùng gắn cờ cho báo cáo bảo mật rủi ro</span><span class="sxs-lookup"><span data-stu-id="ce1af-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="ce1af-121">Báo cáo đăng nhập rủi ro trong cổng thông tin Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="ce1af-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="ce1af-122">Sự kiện rủi ro trong Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="ce1af-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
