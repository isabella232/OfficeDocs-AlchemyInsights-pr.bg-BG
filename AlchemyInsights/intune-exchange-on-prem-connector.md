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
# <a name="intune-exchange-on-premise-connector"></a>Локален конектор за Exchange

За подробности относно настройването на конектора между "Настройка" и "Exchange", който е хостван локален вижте документацията по-долу:

[Настройване на вградения конектор на Exchange в Microsoft Настройте Azure](https://docs.microsoft.com/intune/exchange-connector-install)

**ЧЗВ**

В: виждам грешка, като например "версията на конектора на Exchange не се поддържа", когато се опитвате да настроите съединителя на Exchange. Каква е причината?

А: акаунтът, който използвате, е лицензиран по подходящ начин – трябва да има активен лиценз за настройване

В: може ли да има няколко конектора на Exchange?

А: можете да настроите само един конектор на Exchange за всеки клиент на Exchange за организация. Конекторът може да се инсталира само на един сървър в организация за обмен на много сървъри.

Също така не можете да имате конектори, конфигурирани за локален Exchange и Exchange Online, конфигурирани в един и същ клиент.

В: може ли Конекторът да използва CAS масив като връзка към Exchange?

А: указването на CAS масив не е поддържана конфигурация в настройката на конектора. Трябва да се зададе само един сървър и трябва да бъде вградения anonymoususername във файла за конфигуриране на конектора, който може да бъде намерен в

програма за data\microsoft\microsoft на локален конектор за Exchange \ OnpremiseExchangeConnectorServiceConfiguration.xml

Намерете следния запис ```<ExchangeWebServiceURL />``` и заместете URL адреса със сървъра на Exchange.

**Например**
```<ExchangeWebServiceURL> https://Exchangeserver.domain.com/ews/exchange.asmx<ExchangeWebServiceURL />```

Вижте следната документация за допълнителни отстраняване на неизправности: [отстраняване на неизправности при настройване на локален конектор на Exchange](https://support.microsoft.com/help/4471887/troubleshooting-exchange-connector-in-microsoft-intune)

**Разрешаване на многословното регистриране за съединителя на Exchange**

1. Отворете конфигурационен файл за проследяване на свързването на Exchange за редактиране.  
Файлът се намира на адрес:%ProgramData%\Microsoft\Windows за обмен Connector\TracingConfiguration.xml  

**Например**
``` <C:\ProgramData\Microsoft\Windows Intune Exchange Connector\TracingConfiguration.xml>```
  
2. Намерете TraceSourceLine със следния ключ: OnPremisesExchangeConnectorService  
  
3. Промяна на стойността на възела на SourceLevel от ActivityTracing за информация (по подразбиране) към многословен ActivityTracing  

**Например**
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
4. Рестартирайте услугата за Exchange на Microsoft за настройване  
5. Пълно синхронизиране в портала за настройване, докато не завърши, и след това променете XML обратно на "информационен ActivityTracing" и рестартирайте услугата за Exchange на Microsoft.  
6. Местоположения на регистрационните файлове е: `%ProgramData%\Microsoft\Windows Intune Exchange Connector`