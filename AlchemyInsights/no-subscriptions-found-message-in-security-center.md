---
title: Không tìm thấy thông báo đăng ký trong Trung tâm bảo mật
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/16/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6028"
- "9001222"
ms.openlocfilehash: 01117bc535df14533e426fd2d31c336fccc75611
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 09/15/2020
ms.locfileid: "50714393"
---
# <a name="no-subscriptions-found-message-in-the-security-center"></a><span data-ttu-id="78160-102">Không tìm thấy thông báo đăng ký trong Trung tâm bảo mật</span><span class="sxs-lookup"><span data-stu-id="78160-102">No subscriptions found message in the Security Center</span></span>

<span data-ttu-id="78160-103">Nếu trong khi truy nhập trung tâm bảo mật Microsoft Defender, bạn sẽ nhận được thông báo "không tìm thấy gói đăng ký", điều này có nghĩa là Azure Active Directory (được sử dụng để đăng nhập người dùng vào cổng thông tin không có giấy phép ATP Defender của Microsoft.</span><span class="sxs-lookup"><span data-stu-id="78160-103">If while accessing Microsoft Defender Security Center you get a  "No subscriptions found" message, it means the Azure Active Directory (AAD) used to login the user to the portal doesn't have a Microsoft Defender ATP license.</span></span>  

<span data-ttu-id="78160-104">Giấy phép Windows E5 và Office E5 là các giấy phép riêng biệt.</span><span class="sxs-lookup"><span data-stu-id="78160-104">The Windows E5 and Office E5 licenses are separate licenses.</span></span>

<span data-ttu-id="78160-105">Mở một trường hợp hỗ trợ nếu giấy phép được mua nhưng không được cung cấp cho phiên bản này trong ví dụ này.</span><span class="sxs-lookup"><span data-stu-id="78160-105">Open a support case if the license was purchased but not provisioned to this AAD instance.</span></span> <span data-ttu-id="78160-106">Bạn có:</span><span class="sxs-lookup"><span data-stu-id="78160-106">Either you have:</span></span> <br/>
-   <span data-ttu-id="78160-107">Vấn đề cung cấp giấy phép có thể xảy ra.</span><span class="sxs-lookup"><span data-stu-id="78160-107">A possible license provisioning issue.</span></span><br/>
-   <span data-ttu-id="78160-108">Bạn vô tình cung cấp giấy phép cho một Microsoft khác nhau hơn một người dùng được sử dụng để xác thực vào dịch vụ.</span><span class="sxs-lookup"><span data-stu-id="78160-108">You inadvertently provisioned the license to a different Microsoft AAD than the one used for authentication into the service.</span></span>