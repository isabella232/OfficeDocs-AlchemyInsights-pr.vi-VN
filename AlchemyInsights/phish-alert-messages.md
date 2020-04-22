---
title: 2491 thông báo email từ ' phish gửi do thuê hoặc người dùng ghi đè ' chính sách
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 2e4efd504304da757687e697ff23374aeea31851
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 04/22/2020
ms.locfileid: "43758956"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="8c805-102">Cảnh báo email từ ' phish Delivered do thuê hoặc người dùng ghi đè ' chính sách</span><span class="sxs-lookup"><span data-stu-id="8c805-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="8c805-103">Chính sách cảnh báo mặc định có tên "phish gửi do thuê hoặc người dùng ghi đè" đã được tung ra cho thuê với Office 365 ATP P1 và P2 giấy phép.</span><span class="sxs-lookup"><span data-stu-id="8c805-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="8c805-104">Nếu bạn nhận được cảnh báo này, sau đây là các bước để điều tra:</span><span class="sxs-lookup"><span data-stu-id="8c805-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="8c805-105">Từ thông báo cảnh báo, nhấp vào **xem cảnh báo** để chuyển đến trang **cảnh báo** trong trung tâm tuân thủ & bảo mật.</span><span class="sxs-lookup"><span data-stu-id="8c805-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="8c805-106">Chọn cảnh báo để xem tùy chọn để **xem danh sách tin nhắn** hoặc **xem tin nhắn trong Explorer**.</span><span class="sxs-lookup"><span data-stu-id="8c805-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="8c805-107">Cả hai tùy chọn này sẽ đưa bạn đến các chi tiết của thư, bao gồm thông báo ID.</span><span class="sxs-lookup"><span data-stu-id="8c805-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="8c805-108">Lưu ý rằng liên kết Threat Explorer sẽ tự động lọc các thư phù hợp với tiêu chí cảnh báo.</span><span class="sxs-lookup"><span data-stu-id="8c805-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="8c805-109">Bạn có thể cần phải điều chỉnh bộ lọc ngày trong Threat Explorer.</span><span class="sxs-lookup"><span data-stu-id="8c805-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="8c805-110">Thư lừa đảo đã được gửi do ghi đè cấu hình theo cách thủ công:</span><span class="sxs-lookup"><span data-stu-id="8c805-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="8c805-111">Một người gửi hoặc miền được cho phép do người dùng đặt.</span><span class="sxs-lookup"><span data-stu-id="8c805-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="8c805-112">Một người gửi hoặc tên miền được cho phép bởi quản trị viên trong chính sách chống thư rác.</span><span class="sxs-lookup"><span data-stu-id="8c805-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="8c805-113">Một địa chỉ IP được phép trong chính sách lọc kết nối.</span><span class="sxs-lookup"><span data-stu-id="8c805-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="8c805-114">Quy tắc lưu lượng thư (còn được gọi là quy tắc truyền tải) có cấu hình để cho phép thư.</span><span class="sxs-lookup"><span data-stu-id="8c805-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="8c805-115">Nếu bạn tin rằng thông báo không chính xác được đánh dấu là phish, sử dụng Outlook [báo cáo thông báo Add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) để gửi mẫu thư cho Microsoft.</span><span class="sxs-lookup"><span data-stu-id="8c805-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
