---
title: Tạo chính sách nhãn AIP
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: de7d76564cabb0a5dd1a836984df6b1a63b2b218
ms.sourcegitcommit: 8fdcd2acd31e8a4b9a8a0b91674f397d2f7889c1
ms.translationtype: MT
ms.contentlocale: vi-VN
ms.lasthandoff: 06/03/2020
ms.locfileid: "44569517"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="e8fd6-102">Tạo chính sách nhãn AIP</span><span class="sxs-lookup"><span data-stu-id="e8fd6-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="e8fd6-103">Các nhãn bảo vệ thông tin Azure (AIP) có thể được sử dụng với đầy đủ dữ liệu mà một tổ chức thường tạo ra và lưu trữ, từ phân loại dữ liệu cá nhân thấp nhất, đến phân loại cao nhất của dữ liệu được bảo mật cao.</span><span class="sxs-lookup"><span data-stu-id="e8fd6-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="e8fd6-104">Azure bảo vệ thông tin chính sách áp dụng cho khách hàng truyền thống Azure thông tin bảo vệ (AIP) và không [AIP hợp nhất dán nhãn khách hàng](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="e8fd6-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="e8fd6-105">Bạn có thể cấu hình nhiều phần tử trong chính sách AIP, bao gồm các tùy chọn như:</span><span class="sxs-lookup"><span data-stu-id="e8fd6-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="e8fd6-106">Tùy chọn cho nhãn sẽ cho phép quản trị viên hoặc người dùng phân loại và bảo vệ (tùy chọn) tài liệu và email</span><span class="sxs-lookup"><span data-stu-id="e8fd6-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="e8fd6-107">Tùy chọn để thực thi phân loại khi người dùng lưu tài liệu và gửi email</span><span class="sxs-lookup"><span data-stu-id="e8fd6-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="e8fd6-108">Tùy chọn để tự động gắn nhãn một email, dựa trên các tập tin đính kèm của nó.</span><span class="sxs-lookup"><span data-stu-id="e8fd6-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="e8fd6-109">Tùy chọn để kiểm soát xem thanh bảo vệ thông tin được hiển thị trong ứng dụng Office</span><span class="sxs-lookup"><span data-stu-id="e8fd6-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="e8fd6-110">Để biết thêm tùy chọn và thông tin về chính sách bảo vệ thông tin Azure, hãy xem: [tổng quan về chính sách bảo vệ thông tin Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="e8fd6-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="e8fd6-111">Đối với các tài nguyên hữu ích khác về chính sách AIP, xem:</span><span class="sxs-lookup"><span data-stu-id="e8fd6-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="e8fd6-112">Hướng dẫn: cấu hình thiết đặt chính sách bảo vệ thông tin Azure và tạo nhãn mới</span><span class="sxs-lookup"><span data-stu-id="e8fd6-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="e8fd6-113">Cấu hình chính sách bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="e8fd6-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="e8fd6-114">Tạo và đặt cấu hình nhãn độ nhạy và chính sách của chúng</span><span class="sxs-lookup"><span data-stu-id="e8fd6-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="e8fd6-115">Hướng dẫn cách để các trường hợp phổ biến sử dụng bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="e8fd6-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="e8fd6-116">Đánh giá tài liệu về bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="e8fd6-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="e8fd6-117">Yêu cầu đối với bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="e8fd6-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="e8fd6-118">Hướng dẫn bắt đầu nhanh để bảo vệ thông tin Azure</span><span class="sxs-lookup"><span data-stu-id="e8fd6-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="e8fd6-119">Tải về Azure bảo vệ thông tin khách hàng</span><span class="sxs-lookup"><span data-stu-id="e8fd6-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)