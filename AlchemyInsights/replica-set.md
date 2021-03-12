---
title: Tập hợp bản sao
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
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714589"
---
# <a name="replica-set"></a><span data-ttu-id="d7ab1-102">Tập hợp bản sao</span><span class="sxs-lookup"><span data-stu-id="d7ab1-102">Replica set</span></span>

<span data-ttu-id="d7ab1-103">Tiếng a cũng được gọi là tên miền được quản lý.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="d7ab1-104">Nó thực sự là hai bộ điều khiển tên miền được chạy và duy trì bởi bộ phụ trợ.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="d7ab1-105">Hai hàm này bao gồm một hình DC chính và một bản sao.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="d7ab1-106">Sao lưu trong phần thêm (tên miền được quản lý) là một quy trình tự động do nền tảng Azure quản lý.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="d7ab1-107">Trong trường hợp có sự cố với tên miền được quản lý của bạn, Azure hỗ trợ có thể hỗ trợ bạn trong việc khôi phục từ bản sao lưu.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="d7ab1-108">Bạn tạo mỗi bản sao trong một mạng ảo.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="d7ab1-109">Mỗi mạng ảo phải được peered đến mọi mạng ảo khác mà lưu trữ tập hợp bản sao của tên miền được quản lý.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="d7ab1-110">Cấu hình này tạo một topo mạng lưới hỗ trợ sao chép thư mục.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="d7ab1-111">Mạng ảo có thể hỗ trợ nhiều bộ bản sao, được cung cấp cho mỗi tập hợp bản sao nằm trong một mạng con khác.</span><span class="sxs-lookup"><span data-stu-id="d7ab1-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="d7ab1-112">Để biết thêm chi tiết về bộ bản sao, hãy xem [bộ khái niệm bản sao](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="d7ab1-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
