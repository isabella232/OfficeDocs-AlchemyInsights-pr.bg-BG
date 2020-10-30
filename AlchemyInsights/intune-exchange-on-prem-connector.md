---
title: Локален конектор за Exchange
ms.author: mandia
author: mandia
manager: dougeby
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "6732"
- "9003775"
ms.openlocfilehash: 8b470655efa2dfb460c29b6b840fa793ed2aa448
ms.sourcegitcommit: f8b41ecda6db0b8f64fe0c51f1e8e6619f504d61
ms.translationtype: MT
ms.contentlocale: bg-BG
ms.lasthandoff: 10/28/2020
ms.locfileid: "48807273"
---
# <a name="intune-exchange-on-premise-connector"></a><span data-ttu-id="20b84-102">Локален конектор за Exchange</span><span class="sxs-lookup"><span data-stu-id="20b84-102">Intune Exchange on-premise Connector</span></span>

<span data-ttu-id="20b84-103">За подробности относно настройването на конектора между "Настройка" и "Exchange", който е хостван локален вижте документацията по-долу:</span><span class="sxs-lookup"><span data-stu-id="20b84-103">For details of setting up the connector between Intune and Exchange which is hosted on-premises please see the following documentation:</span></span>

[<span data-ttu-id="20b84-104">Настройване на вградения конектор на Exchange в Microsoft Настройте Azure</span><span class="sxs-lookup"><span data-stu-id="20b84-104">Set up the Intune on-premises Exchange connector in Microsoft Intune Azure</span></span>](https://docs.microsoft.com/intune/exchange-connector-install)

<span data-ttu-id="20b84-105">**ЧЗВ**</span><span class="sxs-lookup"><span data-stu-id="20b84-105">**FAQ:**</span></span>

<span data-ttu-id="20b84-106">В: виждам грешка, като например "версията на конектора на Exchange не се поддържа", когато се опитвате да настроите съединителя на Exchange.</span><span class="sxs-lookup"><span data-stu-id="20b84-106">Q: I see an error such as "The Exchange Connector version is not supported" when attempting to set up the Exchange connector.</span></span> <span data-ttu-id="20b84-107">Каква е причината?</span><span class="sxs-lookup"><span data-stu-id="20b84-107">What could be the cause?</span></span>

<span data-ttu-id="20b84-108">А: акаунтът, който използвате, е лицензиран по подходящ начин – трябва да има активен лиценз за настройване</span><span class="sxs-lookup"><span data-stu-id="20b84-108">A: The account you are using is licensed appropriately - it must have an active Intune license</span></span>

<span data-ttu-id="20b84-109">В: може ли да има няколко конектора на Exchange?</span><span class="sxs-lookup"><span data-stu-id="20b84-109">Q: Is it possible to have multiple Exchange connectors?</span></span>

<span data-ttu-id="20b84-110">А: можете да настроите само един конектор на Exchange за всеки клиент на Exchange за организация.</span><span class="sxs-lookup"><span data-stu-id="20b84-110">A: You can only set up one Exchange connector per Intune tenant per Exchange organization.</span></span> <span data-ttu-id="20b84-111">Конекторът може да се инсталира само на един сървър в организация за обмен на много сървъри.</span><span class="sxs-lookup"><span data-stu-id="20b84-111">The connector can only be installed on one server in a multi server exchange organization.</span></span>

<span data-ttu-id="20b84-112">Също така не можете да имате конектори, конфигурирани за локален Exchange и Exchange Online, конфигурирани в един и същ клиент.</span><span class="sxs-lookup"><span data-stu-id="20b84-112">Also you cannot have connectors configured for both Exchange on-premise and Exchange Online configured in the same tenant.</span></span>

<span data-ttu-id="20b84-113">В: може ли Конекторът да използва CAS масив като връзка към Exchange?</span><span class="sxs-lookup"><span data-stu-id="20b84-113">Q: Can the connector use a CAS array as its connection to Exchange?</span></span>

<span data-ttu-id="20b84-114">А: указването на CAS масив не е поддържана конфигурация в настройката на конектора.</span><span class="sxs-lookup"><span data-stu-id="20b84-114">A: Specifying a CAS array is not a supported configuration in the connector setup.</span></span> <span data-ttu-id="20b84-115">Трябва да се зададе само един сървър и трябва да бъде вградения anonymoususername във файла за конфигуриране на конектора, който може да бъде намерен в</span><span class="sxs-lookup"><span data-stu-id="20b84-115">Only a single server should be specified and should be hardcoded in the connector configuration file which can be found in</span></span>

<span data-ttu-id="20b84-116">програма за data\microsoft\microsoft на локален конектор за Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="20b84-116">program data\microsoft\microsoft Intune on premise Exchange connector\ OnpremiseExchangeConnectorServiceConfiguration.xml</span></span>

<span data-ttu-id="20b84-117">Намерете следния запис ```<ExchangeWebServiceURL />``` и заместете URL адреса със сървъра на Exchange.</span><span class="sxs-lookup"><span data-stu-id="20b84-117">Locate the following entry ```<ExchangeWebServiceURL />``` and replace the URL with the exchange server.</span></span>

<span data-ttu-id="20b84-118">**Например**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span><span class="sxs-lookup"><span data-stu-id="20b84-118">**Example:**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```</span></span>

<span data-ttu-id="20b84-119">Вижте следната документация за допълнителни отстраняване на неизправности: [отстраняване на неизправности при настройване на локален конектор на Exchange](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span><span class="sxs-lookup"><span data-stu-id="20b84-119">Please see the following documentation for additional troubleshooting: [Troubleshoot the Intune on-premises Exchange connector](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)</span></span>

<span data-ttu-id="20b84-120">**Разрешаване на многословното регистриране за съединителя на Exchange**</span><span class="sxs-lookup"><span data-stu-id="20b84-120">**Enabling Verbose logging for the Exchange connector**</span></span>

1. <span data-ttu-id="20b84-121">Отворете конфигурационен файл за проследяване на свързването на Exchange за редактиране.</span><span class="sxs-lookup"><span data-stu-id="20b84-121">Open the Exchange Connector tracing configuration file for editing.</span></span>  
<span data-ttu-id="20b84-122">Файлът се намира на адрес:%ProgramData%\Microsoft\Windows за обмен Connector\TracingConfiguration.xml</span><span class="sxs-lookup"><span data-stu-id="20b84-122">The file is located at : %ProgramData%\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml</span></span>  

<span data-ttu-id="20b84-123">**Например**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span><span class="sxs-lookup"><span data-stu-id="20b84-123">**Example:**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```</span></span>
  
2. <span data-ttu-id="20b84-124">Намерете TraceSourceLine със следния ключ: OnPremisesExchangeConnectorService</span><span class="sxs-lookup"><span data-stu-id="20b84-124">Locate the TraceSourceLine with the following key: OnPremisesExchangeConnectorService</span></span>  
  
3. <span data-ttu-id="20b84-125">Промяна на стойността на възела на SourceLevel от ActivityTracing за информация (по подразбиране) към многословен ActivityTracing</span><span class="sxs-lookup"><span data-stu-id="20b84-125">Change the SourceLevel node value from Information ActivityTracing (the default) to Verbose ActivityTracing</span></span>  

<span data-ttu-id="20b84-126">**Например**</span><span class="sxs-lookup"><span data-stu-id="20b84-126">**Example:**</span></span>
```
<TraceSourceLine>  
<Key xsi:type="xsd:string">OnPremisesExchangeConnectorService</Key>  
<Value xsi:type="TraceSource">  
<SourceLevel>All</SourceLevel>  
<Listeners>  
<Listener>  
<ListenerType>CircularTraceListener</ListenerType>
<SourceLevel>Verbose ActivityTracing</SourceLevel>
```
4. <span data-ttu-id="20b84-127">Рестартирайте услугата за Exchange на Microsoft за настройване</span><span class="sxs-lookup"><span data-stu-id="20b84-127">Restart the Microsoft Intune Exchange Service</span></span>  
5. <span data-ttu-id="20b84-128">Пълно синхронизиране в портала за настройване, докато не завърши, и след това променете XML обратно на "информационен ActivityTracing" и рестартирайте услугата за Exchange на Microsoft.</span><span class="sxs-lookup"><span data-stu-id="20b84-128">Full sync in Intune Portal until it finishes and then change the XML back to "Information ActivityTracing" and restart the Microsoft Intune Exchange Service.</span></span>  
6. <span data-ttu-id="20b84-129">Местоположения на регистрационните файлове е: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span><span class="sxs-lookup"><span data-stu-id="20b84-129">Location of the logs is : `%ProgramData%\Microsoft\Windows Intune Exchange Connector`</span></span>