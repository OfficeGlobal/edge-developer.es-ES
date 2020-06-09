---
description: Hospedar contenido web en la aplicación Win32 con el control Microsoft Edge WebView2
title: Microsoft Edge WebView2 para aplicaciones Win32
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 06/05/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, ICoreWebView2Controller, control de explorador, HTML Edge
ms.openlocfilehash: 05dd401064635a6b20f1936b1efaac025b45749f
ms.sourcegitcommit: 8dca1c1367853e45a0a975bc89b1818adb117bd4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/08/2020
ms.locfileid: "10699386"
---
# <span data-ttu-id="fbb1d-104">interfaz ICoreWebView2AcceleratorKeyPressedEventHandler</span><span class="sxs-lookup"><span data-stu-id="fbb1d-104">interface ICoreWebView2AcceleratorKeyPressedEventHandler</span></span> 

```
interface ICoreWebView2AcceleratorKeyPressedEventHandler
  : public IUnknown
```

<span data-ttu-id="fbb1d-105">La persona que llama implementa esta interfaz para recibir el evento AcceleratorKeyPressed.</span><span class="sxs-lookup"><span data-stu-id="fbb1d-105">The caller implements this interface to receive the AcceleratorKeyPressed event.</span></span>

## <span data-ttu-id="fbb1d-106">Resumen</span><span class="sxs-lookup"><span data-stu-id="fbb1d-106">Summary</span></span>

 <span data-ttu-id="fbb1d-107">Miembros</span><span class="sxs-lookup"><span data-stu-id="fbb1d-107">Members</span></span>                        | <span data-ttu-id="fbb1d-108">Descripciones</span><span class="sxs-lookup"><span data-stu-id="fbb1d-108">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="fbb1d-109">Invoke</span><span class="sxs-lookup"><span data-stu-id="fbb1d-109">Invoke</span></span>](#invoke) | <span data-ttu-id="fbb1d-110">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="fbb1d-110">Called to provide the implementer with the event args for the corresponding event.</span></span>

## <span data-ttu-id="fbb1d-111">Miembros</span><span class="sxs-lookup"><span data-stu-id="fbb1d-111">Members</span></span>

#### <span data-ttu-id="fbb1d-112">Invoke</span><span class="sxs-lookup"><span data-stu-id="fbb1d-112">Invoke</span></span> 

<span data-ttu-id="fbb1d-113">Se llama para proporcionar al implementador los argumentos del evento para el evento correspondiente.</span><span class="sxs-lookup"><span data-stu-id="fbb1d-113">Called to provide the implementer with the event args for the corresponding event.</span></span>

> <span data-ttu-id="fbb1d-114">invocación [Invoke](#invoke)pública de HRESULT ([ICoreWebView2Controller](icorewebview2controller.md) \* Sender, [ICoreWebView2AcceleratorKeyPressedEventArgs](icorewebview2acceleratorkeypressedeventargs.md) \* args)</span><span class="sxs-lookup"><span data-stu-id="fbb1d-114">public HRESULT [Invoke](#invoke)([ICoreWebView2Controller](icorewebview2controller.md) \* sender, [ICoreWebView2AcceleratorKeyPressedEventArgs](icorewebview2acceleratorkeypressedeventargs.md) \* args)</span></span>
