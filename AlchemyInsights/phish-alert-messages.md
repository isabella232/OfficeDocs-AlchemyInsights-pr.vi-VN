---
title: 2491 email cảnh báo tin nhắn từ chính sách 'Phish giao hàng do người thuê nhà hoặc người dùng ghi đè
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 2491
ms.assetid: ''
ms.openlocfilehash: 456b186ecea59422c791c79d4df056ad8446bc70
ms.sourcegitcommit: 7c90dcc570d32ebd968e3e4e816a7b482890b3a4
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36391628"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="3f1b3-102">Các thư email cảnh báo từ chính sách 'Phish giao hàng do người thuê nhà hoặc người dùng ghi đè</span><span class="sxs-lookup"><span data-stu-id="3f1b3-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="3f1b3-103">Một chính sách mặc định cảnh báo tên "Phish Delivered do người thuê nhà hoặc người dùng ghi đè" đã được cán cho người thuê nhà với giấy phép Office 365 ATP P1 và P2.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Office 365 ATP P1 and P2 licenses.</span></span> <span data-ttu-id="3f1b3-104">Nếu bạn nhận được thông báo này, dưới đây là các bước điều tra:</span><span class="sxs-lookup"><span data-stu-id="3f1b3-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="3f1b3-105">Từ cảnh báo, hãy nhấp vào **Xem thông báo** để đi đến trang **cảnh báo** an ninh & Trung tâm phù hợp.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="3f1b3-106">Chọn cảnh báo để xem các tùy chọn để **xem thông báo danh sách** hoặc **xem tin nhắn trong Explorer**.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="3f1b3-107">Cả hai các tùy chọn này sẽ đưa bạn đến các chi tiết của thư, bao gồm ID tin nhắn</span><span class="sxs-lookup"><span data-stu-id="3f1b3-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="3f1b3-108">Lưu ý rằng các liên kết mối đe dọa Explorer sẽ tự động lọc thư phù hợp với các tiêu chí cảnh báo.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="3f1b3-109">Bạn có thể cần phải điều chỉnh các bộ lọc ngày trong Explorer mối đe dọa.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="3f1b3-110">Thư lừa đảo đã được chuyển giao bởi vì một ghi đè cấu hình thủ công:</span><span class="sxs-lookup"><span data-stu-id="3f1b3-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="3f1b3-111">Cho phép người gửi hay tên miền thiết lập bởi người dùng.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="3f1b3-112">Cho phép người gửi hay tên miền thiết lập bởi các quản trị viên trong một chính sách chống thư rác.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="3f1b3-113">Một địa chỉ IP được cho phép trong một chính sách lọc kết nối.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="3f1b3-114">Một luồng quy tắc thư (cũng được biết đến như là một quy tắc truyền tải) được cấu hình để cho phép các tin nhắn trong.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="3f1b3-115">Nếu bạn tin rằng thư được đánh dấu không chính xác như phish, sử dụng các Outlook [tin nhắn báo cáo add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) để gửi thông báo mẫu cho Microsoft.</span><span class="sxs-lookup"><span data-stu-id="3f1b3-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
