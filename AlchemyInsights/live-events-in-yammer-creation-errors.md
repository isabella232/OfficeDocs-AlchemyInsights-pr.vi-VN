---
title: Các sự kiện trực tiếp trong lỗi tạo yammer
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002495"
- "5112"
ms.openlocfilehash: 1b342b17e4b91804a75c46352f3ef7d7814bfcee
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/14/2020
ms.locfileid: "47675464"
---
# <a name="live-events-in-yammer-creation-errors"></a><span data-ttu-id="15da1-102">Các sự kiện trực tiếp trong lỗi tạo yammer</span><span class="sxs-lookup"><span data-stu-id="15da1-102">Live events in Yammer creation errors</span></span>

<span data-ttu-id="15da1-103">**Tạo sự kiện yammer trực tiếp**</span><span class="sxs-lookup"><span data-stu-id="15da1-103">**Yammer Live Event creation**</span></span>

<span data-ttu-id="15da1-104">Yammer sẽ hiển thị tùy chọn để tạo sự kiện trực tiếp vào mọi thời điểm.</span><span class="sxs-lookup"><span data-stu-id="15da1-104">Yammer will show the option to create a live event at all times.</span></span> <span data-ttu-id="15da1-105">Trong một số trường hợp, người dùng có thể không đáp ứng các điều kiện tiên quyết để tạo sự kiện trực tiếp và nhận được lỗi khi họ tìm cách tạo.</span><span class="sxs-lookup"><span data-stu-id="15da1-105">In some cases, a user may not meet the prerequisites for creating a live event and receive an error when they attempt to create it.</span></span> <span data-ttu-id="15da1-106">Các mục dưới đây bao gồm các lý do phổ biến cho vấn đề này và cung cấp các cách để giải quyết cho người dùng cuối.</span><span class="sxs-lookup"><span data-stu-id="15da1-106">The items below cover common reasons for this problem and provide ways to resolve it for end users.</span></span>

<span data-ttu-id="15da1-107">**Ai có thể tạo sự kiện trực tiếp**</span><span class="sxs-lookup"><span data-stu-id="15da1-107">**Who can create live events**</span></span>
- <span data-ttu-id="15da1-108">Một Office 365 Enterprise E1, E3 hoặc E5 License hoặc giấy phép Office 365 A3 hoặc A5.</span><span class="sxs-lookup"><span data-stu-id="15da1-108">An Office 365 Enterprise E1, E3, or E5 license or an Office 365 A3 or A5 license.</span></span>
- <span data-ttu-id="15da1-109">Quyền tạo sự kiện trực tiếp trong Trung tâm quản trị nhóm Microsoft.</span><span class="sxs-lookup"><span data-stu-id="15da1-109">Permission to create live events in Microsoft Teams admin center.</span></span>
- <span data-ttu-id="15da1-110">Quyền tạo sự kiện trực tiếp trong Microsoft Stream (cho các sự kiện được tạo bằng cách sử dụng một ứng dụng hoặc thiết bị phát rộng bên ngoài).</span><span class="sxs-lookup"><span data-stu-id="15da1-110">Permission to create live events in Microsoft Stream (for events produced using an external broadcasting app or device).</span></span>
- <span data-ttu-id="15da1-111">Thành viên nhóm đầy đủ trong tổ chức (không thể là khách mời hoặc từ tổ chức khác).</span><span class="sxs-lookup"><span data-stu-id="15da1-111">Full team membership in the org (can’t be a guest or from another org).</span></span>
- <span data-ttu-id="15da1-112">Lập lịch cuộc họp riêng tư, chia sẻ screenvà chia sẻ video IP, được bật trong chính sách cuộc họp nhóm.</span><span class="sxs-lookup"><span data-stu-id="15da1-112">Private meeting scheduling, screensharing, and IP video sharing, turned on in Team meeting policy.</span></span>

<span data-ttu-id="15da1-113">**Các chính sách tạo sự kiện trực tiếp**</span><span class="sxs-lookup"><span data-stu-id="15da1-113">**Live event creation policies**</span></span>

<span data-ttu-id="15da1-114">Yammer theo chính sách sự kiện trực tiếp được đặt trong đối tượng thuê Office 365 của bạn cho dòng.</span><span class="sxs-lookup"><span data-stu-id="15da1-114">Yammer follows the Live Event policies set in your Office 365 tenant for Stream.</span></span> <span data-ttu-id="15da1-115">Theo mặc định, mọi người trong tổ chức của bạn có thể tạo sự kiện trực tiếp.</span><span class="sxs-lookup"><span data-stu-id="15da1-115">By default, everyone in your organization can create a live event.</span></span> <span data-ttu-id="15da1-116">Người quản trị có thể [thực hiện các thay đổi đối với thiết đặt này mà có thể ngăn người dùng tạo sự kiện trực tiếp](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span><span class="sxs-lookup"><span data-stu-id="15da1-116">Administrators may [make changes to this setting which may prevent users from creating a live event](https://docs.microsoft.com/stream/live-event-administration#enabling-and-restricting-users-to-creating).</span></span> <span data-ttu-id="15da1-117">Điều quan trọng là nên kiểm tra xem người dùng có quyền tạo ra các sự kiện trực tiếp nếu họ nhận được lỗi chính sách hay không.</span><span class="sxs-lookup"><span data-stu-id="15da1-117">It is important to check that users have permissions to create live events if they receive a policy error.</span></span>
