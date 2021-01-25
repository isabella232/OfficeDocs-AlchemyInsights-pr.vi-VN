---
title: Khắc phục sự cố trạng thái kiểm dịch
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7853"
- "9004348"
ms.openlocfilehash: 3ee932b7788f4aff3c8bc762c5c917124edfe065
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949927"
---
# <a name="troubleshoot-quarantine-state"></a><span data-ttu-id="34047-102">Khắc phục sự cố trạng thái kiểm dịch</span><span class="sxs-lookup"><span data-stu-id="34047-102">Troubleshoot quarantine state</span></span>

<span data-ttu-id="34047-103">Dịch vụ cung cấp Azure Active Directory (AD) giám sát trạng thái của cấu hình của bạn.</span><span class="sxs-lookup"><span data-stu-id="34047-103">The Azure Active Directory (AD) provisioning service monitors the health of your configuration.</span></span> <span data-ttu-id="34047-104">Nó cũng đặt các ứng dụng không lành mạnh **trong trạng thái** kiểm dịch.</span><span class="sxs-lookup"><span data-stu-id="34047-104">It also places unhealthy apps in a **quarantine** state.</span></span> <span data-ttu-id="34047-105">Nếu hầu hết, hoặc tất cả các cuộc gọi được thực hiện đối với hệ thống đích nhất quán không thành công, thì việc cung cấp sẽ được đánh dấu là **trong cách ly**.</span><span class="sxs-lookup"><span data-stu-id="34047-105">If most, or all, of the calls made against the target system consistently fail, then the provisioning job is marked as **in quarantine**.</span></span> <span data-ttu-id="34047-106">Một ví dụ về lỗi là **một lỗi đã nhận được vì thông tin xác thực của người quản trị không hợp lệ**.</span><span class="sxs-lookup"><span data-stu-id="34047-106">An example of a failure is **an error received because of invalid admin credentials**.</span></span> <span data-ttu-id="34047-107">Để biết thêm thông tin, hãy xem mục [cung cấp ứng dụng trong trạng thái cách ly](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span><span class="sxs-lookup"><span data-stu-id="34047-107">For more information, see [Application provisioning in quarantine status](https://docs.microsoft.com/azure/active-directory/app-provisioning/application-provisioning-quarantine-status).</span></span>

<span data-ttu-id="34047-108">Để khắc phục sự cố đồng bộ đám mây, hãy xem các [vấn đề về cách ly](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span><span class="sxs-lookup"><span data-stu-id="34047-108">To troubleshoot cloud sync, see [Provisioning quarantined problems](https://docs.microsoft.com/azure/active-directory/cloud-sync/how-to-troubleshoot#provisioning-quarantined-problems).</span></span> 
