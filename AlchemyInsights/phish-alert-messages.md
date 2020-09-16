---
title: 2491 thông báo email từ ' phish Delivered do chính sách đối tượng thuê hoặc ghi đè người dùng
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 5b5faa08542cb5878107f10afb34427f636562ac
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47728633"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="52d50-102">Thông báo tin nhắn email từ ' phish Delivered do chính sách đối tượng thuê hoặc ghi đè người dùng</span><span class="sxs-lookup"><span data-stu-id="52d50-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="52d50-103">Một chính sách cảnh báo mặc định có tên là "phish được chuyển phát do đối tượng thuê hoặc người dùng ghi đè" đã được triển khai cho các đối tượng thuê với Office 365 ATP P1 và P2 giấy phép.</span><span class="sxs-lookup"><span data-stu-id="52d50-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="52d50-104">Nếu bạn nhận được cảnh báo này, sau đây là các bước để điều tra:</span><span class="sxs-lookup"><span data-stu-id="52d50-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="52d50-105">Từ thông báo cảnh báo, hãy bấm **xem cảnh báo** để đi đến trang **cảnh báo** trong trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="52d50-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="52d50-106">Chọn cảnh báo để xem tùy chọn để **xem danh sách thư** hoặc **xem thư trong Explorer**.</span><span class="sxs-lookup"><span data-stu-id="52d50-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="52d50-107">Cả hai tùy chọn này sẽ đưa bạn đến chi tiết của thư, trong đó bao gồm ID thư.</span><span class="sxs-lookup"><span data-stu-id="52d50-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="52d50-108">Lưu ý rằng nối kết mối đe dọa Explorer sẽ tự động lọc các thư khớp với tiêu chí cảnh báo.</span><span class="sxs-lookup"><span data-stu-id="52d50-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="52d50-109">Bạn có thể cần điều chỉnh bộ lọc ngày trong Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="52d50-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="52d50-110">Thư lừa đảo được chuyển phát do ghi đè được cấu hình thủ công:</span><span class="sxs-lookup"><span data-stu-id="52d50-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="52d50-111">Người dùng hoặc tên miền được cho phép.</span><span class="sxs-lookup"><span data-stu-id="52d50-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="52d50-112">Người gửi hoặc tên miền được cho phép do người quản trị thiết lập trong chính sách chống thư rác.</span><span class="sxs-lookup"><span data-stu-id="52d50-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="52d50-113">Một địa chỉ IP được cho phép trong chính sách bộ lọc kết nối.</span><span class="sxs-lookup"><span data-stu-id="52d50-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="52d50-114">Quy tắc dòng thư (còn được gọi là quy tắc truyền dẫn) được cấu hình để cho phép các thư trong đó.</span><span class="sxs-lookup"><span data-stu-id="52d50-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="52d50-115">Nếu bạn tin rằng thư không được đánh dấu là phish, hãy dùng [bổ trợ tin nhắn báo cáo](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) Outlook để gửi mẫu thư vào Microsoft.</span><span class="sxs-lookup"><span data-stu-id="52d50-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
