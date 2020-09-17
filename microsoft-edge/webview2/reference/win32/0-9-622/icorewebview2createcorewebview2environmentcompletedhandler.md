---
description: Insertar tecnologías web (HTML, CSS y JavaScript) en las aplicaciones nativas con el control Microsoft Edge WebView2
title: WebView2 Win32 C++ ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 09/09/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, ICoreWebView2Controller, control de explorador, HTML Edge, ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler
ms.openlocfilehash: 3f6b6b9a2d4df2a450b4589c351c3ea98f7cc28f
ms.sourcegitcommit: 0faf538d5033508af4320b9b89c4ed99872f0574
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/10/2020
ms.locfileid: "11012765"
---
# <span data-ttu-id="5c6fd-104">interfaz ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler</span><span class="sxs-lookup"><span data-stu-id="5c6fd-104">interface ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler</span></span> 

```
interface ICoreWebView2CreateCoreWebView2EnvironmentCompletedHandler
  : public IUnknown
```

<span data-ttu-id="5c6fd-105">La persona que llama implementa esta interfaz para recibir el WebView2Environment creado a través de CreateCoreWebView2Environment.</span><span class="sxs-lookup"><span data-stu-id="5c6fd-105">The caller implements this interface to receive the WebView2Environment created via CreateCoreWebView2Environment.</span></span>

## <span data-ttu-id="5c6fd-106">Resumen</span><span class="sxs-lookup"><span data-stu-id="5c6fd-106">Summary</span></span>

 <span data-ttu-id="5c6fd-107">Miembros</span><span class="sxs-lookup"><span data-stu-id="5c6fd-107">Members</span></span>                        | <span data-ttu-id="5c6fd-108">Descripciones</span><span class="sxs-lookup"><span data-stu-id="5c6fd-108">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="5c6fd-109">Invoke</span><span class="sxs-lookup"><span data-stu-id="5c6fd-109">Invoke</span></span>](#invoke) | <span data-ttu-id="5c6fd-110">Se llama para proporcionar al implementador el estado de finalización y el resultado de la llamada de método asincrónica correspondiente.</span><span class="sxs-lookup"><span data-stu-id="5c6fd-110">Called to provide the implementer with the completion status and result of the corresponding asynchronous method call.</span></span>

## <span data-ttu-id="5c6fd-111">Miembros</span><span class="sxs-lookup"><span data-stu-id="5c6fd-111">Members</span></span>

#### <span data-ttu-id="5c6fd-112">Invoke</span><span class="sxs-lookup"><span data-stu-id="5c6fd-112">Invoke</span></span> 

<span data-ttu-id="5c6fd-113">Se llama para proporcionar al implementador el estado de finalización y el resultado de la llamada de método asincrónica correspondiente.</span><span class="sxs-lookup"><span data-stu-id="5c6fd-113">Called to provide the implementer with the completion status and result of the corresponding asynchronous method call.</span></span>

> <span data-ttu-id="5c6fd-114">invocación [Invoke](#invoke)de HRESULT pública (HRESULT ErrorCode, [ICoreWebView2Environment](icorewebview2environment.md) \* createdEnvironment)</span><span class="sxs-lookup"><span data-stu-id="5c6fd-114">public HRESULT [Invoke](#invoke)(HRESULT errorCode, [ICoreWebView2Environment](icorewebview2environment.md) \* createdEnvironment)</span></span>
