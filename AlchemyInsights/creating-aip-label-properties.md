---
title: Създаване на правила за етикети на ПДИ
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "4539"
- "9002266"
ms.openlocfilehash: bef170d8e38dcc91094b95604aeb1968d5c57fca
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 09/14/2020
ms.locfileid: "47732164"
---
# <a name="creating-aip-label-policies"></a><span data-ttu-id="7ae46-102">Създаване на правила за етикети на ПДИ</span><span class="sxs-lookup"><span data-stu-id="7ae46-102">Creating AIP Label Policies</span></span>

<span data-ttu-id="7ae46-103">Етикетите на Azure Information Protection (ПДИ) могат да се използват с пълния диапазон от данни, които една организация обикновено създава и съхранява, от най-ниската класификация на лични данни, към най-високата класификация на строго поверителни данни.</span><span class="sxs-lookup"><span data-stu-id="7ae46-103">Azure Information Protection(AIP) labels can be used with the full range of data that an organization typically creates and stores, from the lowest classification of personal data, to the highest classification of highly confidential data.</span></span> <span data-ttu-id="7ae46-104">Правилата за защита на информацията за Azure важат за класическия клиент на Azure Protection (ПДИ), а не за  [един унифициран клиент за етикетиране на ПДИ](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span><span class="sxs-lookup"><span data-stu-id="7ae46-104">Azure Information Protection Policies apply to the Azure Information Protection(AIP) classic client and not the  [AIP Unified Labeling client](https://docs.microsoft.com/azure/information-protection/rms-client/unifiedlabelingclient-version-release-history).</span></span> <span data-ttu-id="7ae46-105">Можете да конфигурирате множество елементи в политиката на ПДИ, включително опции, като например:</span><span class="sxs-lookup"><span data-stu-id="7ae46-105">You can configure multiple elements in an AIP policy, including options like:</span></span>

- <span data-ttu-id="7ae46-106">Опция, за която Етикетът позволява на администраторите или потребителите да класифицират и защитават (по желание) документи и имейли</span><span class="sxs-lookup"><span data-stu-id="7ae46-106">Option for which label will let administrators or user classify and protection(optional) documents and emails</span></span>
- <span data-ttu-id="7ae46-107">Опция за налагане на класификация при записване на документи и изпращане на имейли</span><span class="sxs-lookup"><span data-stu-id="7ae46-107">Option to enforce classification when users save documents and send email</span></span>
- <span data-ttu-id="7ae46-108">Опция за автоматично етикетиране на имейл съобщение, базирано на неговите прикачени файлове.</span><span class="sxs-lookup"><span data-stu-id="7ae46-108">Option to automatically label an email message, based on its attachments.</span></span>
- <span data-ttu-id="7ae46-109">Опция за управление дали лентата за защита на информацията се показва в приложенията на Office</span><span class="sxs-lookup"><span data-stu-id="7ae46-109">Option to control whether the Information Protection bar is displayed in Office applications</span></span>

<span data-ttu-id="7ae46-110">За допълнителни опции и информация относно правилата за защита на информацията за Azure вижте: [общ преглед на правилата за защита на информацията в Azure](https://docs.microsoft.com/azure/information-protection/overview-policy).</span><span class="sxs-lookup"><span data-stu-id="7ae46-110">For additional options and information on Azure Information Protection policies, see: [Overview of the Azure Information Protection policy](https://docs.microsoft.com/azure/information-protection/overview-policy).</span></span>  

<span data-ttu-id="7ae46-111">За други полезни ресурси относно политиките на ПДИ вижте:</span><span class="sxs-lookup"><span data-stu-id="7ae46-111">For other helpful resources regarding AIP policies, see:</span></span>

- [<span data-ttu-id="7ae46-112">Урок: Конфигуриране на настройките на правилата за защита на Azure информация и създаване на нов етикет</span><span class="sxs-lookup"><span data-stu-id="7ae46-112">Tutorial: Configure Azure Information Protection policy settings and create a new label</span></span>](https://docs.microsoft.com/azure/information-protection/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="7ae46-113">Конфигуриране на правилата за защита на информацията за Azure</span><span class="sxs-lookup"><span data-stu-id="7ae46-113">Configuring the Azure Information Protection policy</span></span>](https://docs.microsoft.com/azure/information-protection/configure-policy)  
- [<span data-ttu-id="7ae46-114">Създаване и конфигуриране на етикети за чувствителност и техните правила</span><span class="sxs-lookup"><span data-stu-id="7ae46-114">Create and configure sensitivity labels and their policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/create-sensitivity-labels)  
- [<span data-ttu-id="7ae46-115">Ръководство "как да" за често срещани сценарии, които използват Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7ae46-115">How-to guides for common scenarios that use Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/how-to-guides)  
- [<span data-ttu-id="7ae46-116">Преглед на документацията за защита на информацията на Azure</span><span class="sxs-lookup"><span data-stu-id="7ae46-116">Review Azure Information Protection documentation</span></span>](https://docs.microsoft.com/azure/information-protection/what-is-information-protection)  
- [<span data-ttu-id="7ae46-117">Изисквания за информация за Azure Protection</span><span class="sxs-lookup"><span data-stu-id="7ae46-117">Requirements for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/requirements)  
- [<span data-ttu-id="7ae46-118">Ръководство за бърз старт за Azure Information Protection</span><span class="sxs-lookup"><span data-stu-id="7ae46-118">Quick start tutorial for Azure Information Protection</span></span>](https://docs.microsoft.com/azure/information-protection/get-started/infoprotect-quick-start-tutorial)  
- [<span data-ttu-id="7ae46-119">Изтегляне на Azure за защита на информацията за клиента</span><span class="sxs-lookup"><span data-stu-id="7ae46-119">Download Azure Information Protection client</span></span>](https://www.microsoft.com/download/details.aspx?id=53018)