---
description: Hospedar contenido web en la aplicación Win32 con el control Microsoft Edge WebView2
title: Microsoft Edge WebView2 para aplicaciones Win32
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 05/07/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, ICoreWebView2Controller, control de explorador, HTML Edge
ms.openlocfilehash: f9dcfa996058f4499daff03d8cad033ac61db4c9
ms.sourcegitcommit: 07cda56425e5fdf90eeb3972e17041261bf720cd
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/14/2020
ms.locfileid: "10655334"
---
# <span data-ttu-id="03a86-104">interfaz ICoreWebView2MoveFocusRequestedEventHandler</span><span class="sxs-lookup"><span data-stu-id="03a86-104">interface ICoreWebView2MoveFocusRequestedEventHandler</span></span> 

```
interface ICoreWebView2MoveFocusRequestedEventHandler
  : public IUnknown
```

<span data-ttu-id="03a86-105">La persona que llama implementa este método para recibir el evento MoveFocusRequested.</span><span class="sxs-lookup"><span data-stu-id="03a86-105">The caller implements this method to receive the MoveFocusRequested event.</span></span>

## <span data-ttu-id="03a86-106">Resumen</span><span class="sxs-lookup"><span data-stu-id="03a86-106">Summary</span></span>

 <span data-ttu-id="03a86-107">Miembros</span><span class="sxs-lookup"><span data-stu-id="03a86-107">Members</span></span>                        | <span data-ttu-id="03a86-108">Descripciones</span><span class="sxs-lookup"><span data-stu-id="03a86-108">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="03a86-109">Invoke</span><span class="sxs-lookup"><span data-stu-id="03a86-109">Invoke</span></span>](#invoke) | <span data-ttu-id="03a86-110">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="03a86-110">Called to provide the implementer with the event args for the corresponding event.</span></span>

## <span data-ttu-id="03a86-111">Miembros</span><span class="sxs-lookup"><span data-stu-id="03a86-111">Members</span></span>

#### <span data-ttu-id="03a86-112">Invoke</span><span class="sxs-lookup"><span data-stu-id="03a86-112">Invoke</span></span> 

<span data-ttu-id="03a86-113">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="03a86-113">Called to provide the implementer with the event args for the corresponding event.</span></span>

> <span data-ttu-id="03a86-114">invocación [Invoke](#invoke)pública de HRESULT ([ICoreWebView2Controller](icorewebview2controller.md) \* Sender, [ICoreWebView2MoveFocusRequestedEventArgs](icorewebview2movefocusrequestedeventargs.md) \* args)</span><span class="sxs-lookup"><span data-stu-id="03a86-114">public HRESULT [Invoke](#invoke)([ICoreWebView2Controller](icorewebview2controller.md) \* sender, [ICoreWebView2MoveFocusRequestedEventArgs](icorewebview2movefocusrequestedeventargs.md) \* args)</span></span>
