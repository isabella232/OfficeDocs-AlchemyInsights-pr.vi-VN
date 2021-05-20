---
title: 2491 Cảnh báo thư email từ chính sách 'Chuyển phát qua mạng do đối tượng thuê hoặc người dùng ghi đè'
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
ms.openlocfilehash: 2b373423cf3e63b76a62465dd62076c023580e94
ms.sourcegitcommit: f4866e94918c7b591ad0cd3b58169d340bcc7f00
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 05/19/2021
ms.locfileid: "52544600"
---
# <a name="alert-email-messages-from-the-phish-delivered-due-to-tenant-or-user-override-policy"></a><span data-ttu-id="d76e2-102">Cảnh báo email từ chính sách 'Chuyển phát thư lừa đảo do đối tượng thuê hoặc người dùng ghi đè'</span><span class="sxs-lookup"><span data-stu-id="d76e2-102">Alert email messages from the 'Phish Delivered due to tenant or user override' policy</span></span>

<span data-ttu-id="d76e2-103">Chính sách cảnh báo mặc định có tên "Giao hàng qua mạng do đối tượng thuê hoặc người dùng ghi đè" đã được triển khai cho các đối tượng thuê có giấy phép Microsoft Defender dành cho Office 365 P1 và P2.</span><span class="sxs-lookup"><span data-stu-id="d76e2-103">A default alert policy named "Phish Delivered due to tenant or user override" has been rolled out to tenants with Microsoft Defender for Office 365 P1 and P2 licenses.</span></span> <span data-ttu-id="d76e2-104">Nếu bạn nhận được cảnh báo này, dưới đây là các bước để điều tra:</span><span class="sxs-lookup"><span data-stu-id="d76e2-104">If you received this alert, here are the steps to investigate:</span></span>

1. <span data-ttu-id="d76e2-105">Từ thông báo cảnh báo, hãy **bấm Xem Cảnh** báo để đến trang Cảnh báo **trong** Trung tâm Tuân & Chính sách Bảo mật.</span><span class="sxs-lookup"><span data-stu-id="d76e2-105">From the alert message, click **View Alert** to go to the **Alerts** page in the Security & Compliance Center.</span></span>

2. <span data-ttu-id="d76e2-106">Chọn cảnh báo để xem tùy chọn Xem **danh sách thư hoặc** Xem thư trong **Explorer**.</span><span class="sxs-lookup"><span data-stu-id="d76e2-106">Select the alert to see the option to **View message list** or **View messages in Explorer**.</span></span> <span data-ttu-id="d76e2-107">Cả hai tùy chọn này sẽ đưa bạn đến chi tiết của thư, trong đó có ID Thông báo.</span><span class="sxs-lookup"><span data-stu-id="d76e2-107">Both of these options take you to the details of the message, which includes the Message ID.</span></span> <span data-ttu-id="d76e2-108">Lưu ý rằng liên kết Trình khám phá Mối đe dọa sẽ tự động lọc các thư khớp với tiêu chí cảnh báo.</span><span class="sxs-lookup"><span data-stu-id="d76e2-108">Note that the Threat Explorer link will automatically filter the messages that match the alert criteria.</span></span> <span data-ttu-id="d76e2-109">Bạn có thể cần điều chỉnh bộ lọc ngày trong Trình khám phá Mối đe dọa.</span><span class="sxs-lookup"><span data-stu-id="d76e2-109">You might need to adjust the date filter in Threat Explorer.</span></span>

<span data-ttu-id="d76e2-110">Thư lừa đảo đã được chuyển phát do thay thế được cấu hình theo cách thủ công:</span><span class="sxs-lookup"><span data-stu-id="d76e2-110">The phishing message was delivered because of a manually configured override:</span></span>

- <span data-ttu-id="d76e2-111">Người dùng được phép đặt tên miền hoặc người dùng.</span><span class="sxs-lookup"><span data-stu-id="d76e2-111">An allowed sender or domain set by the user.</span></span>

- <span data-ttu-id="d76e2-112">Người gửi hoặc tên miền được phép thiết lập bởi người quản trị trong chính sách chống thư rác.</span><span class="sxs-lookup"><span data-stu-id="d76e2-112">An allowed sender or domain set by the admin in an anti-spam policy.</span></span>

- <span data-ttu-id="d76e2-113">Địa chỉ IP được cho phép trong chính sách bộ lọc kết nối.</span><span class="sxs-lookup"><span data-stu-id="d76e2-113">An allowed IP address in a connection filter policy.</span></span>

- <span data-ttu-id="d76e2-114">Quy tắc dòng thư (còn được gọi là quy tắc truyền tải) được cấu hình để cho phép thư nhập.</span><span class="sxs-lookup"><span data-stu-id="d76e2-114">A mail flow rule (also known as a transport rule) that's configured to allow messages in.</span></span>

<span data-ttu-id="d76e2-115">Nếu bạn cho rằng thư đã được đánh dấu sai [](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) là thư lừa đảo qua điện thoại, hãy sử dụng phần bổ trợ Outlook Báo cáo để gửi mẫu thư đến Microsoft.</span><span class="sxs-lookup"><span data-stu-id="d76e2-115">If you believe the message was incorrectly marked as phish, use the Outlook [Report Message add-in](https://support.office.com/article/b5caa9f1-cdf3-4443-af8c-ff724ea719d2) to submit message samples to Microsoft.</span></span>
