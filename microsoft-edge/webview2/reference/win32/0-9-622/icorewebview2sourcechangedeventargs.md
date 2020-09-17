---
description: Insertar tecnologías web (HTML, CSS y JavaScript) en las aplicaciones nativas con el control Microsoft Edge WebView2
title: WebView2 Win32 C++ ICoreWebView2SourceChangedEventArgs
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 09/09/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, ICoreWebView2Controller, control de explorador, HTML Edge, ICoreWebView2SourceChangedEventArgs
ms.openlocfilehash: 7417b4790d327bbd5a415dc1237e0604963598e0
ms.sourcegitcommit: 0faf538d5033508af4320b9b89c4ed99872f0574
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/10/2020
ms.locfileid: "11012749"
---
# <span data-ttu-id="5e27f-104">interfaz ICoreWebView2SourceChangedEventArgs</span><span class="sxs-lookup"><span data-stu-id="5e27f-104">interface ICoreWebView2SourceChangedEventArgs</span></span> 

```
interface ICoreWebView2SourceChangedEventArgs
  : public IUnknown
```

<span data-ttu-id="5e27f-105">Argumentos de evento para el evento SourceChanged.</span><span class="sxs-lookup"><span data-stu-id="5e27f-105">Event args for the SourceChanged event.</span></span>

## <span data-ttu-id="5e27f-106">Resumen</span><span class="sxs-lookup"><span data-stu-id="5e27f-106">Summary</span></span>

 <span data-ttu-id="5e27f-107">Miembros</span><span class="sxs-lookup"><span data-stu-id="5e27f-107">Members</span></span>                        | <span data-ttu-id="5e27f-108">Descripciones</span><span class="sxs-lookup"><span data-stu-id="5e27f-108">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="5e27f-109">get_IsNewDocument</span><span class="sxs-lookup"><span data-stu-id="5e27f-109">get_IsNewDocument</span></span>](#get_isnewdocument) | <span data-ttu-id="5e27f-110">True si la página a la que se navega es un documento nuevo.</span><span class="sxs-lookup"><span data-stu-id="5e27f-110">True if the page being navigated to is a new document.</span></span>

## <span data-ttu-id="5e27f-111">Miembros</span><span class="sxs-lookup"><span data-stu-id="5e27f-111">Members</span></span>

#### <span data-ttu-id="5e27f-112">get_IsNewDocument</span><span class="sxs-lookup"><span data-stu-id="5e27f-112">get_IsNewDocument</span></span> 

<span data-ttu-id="5e27f-113">True si la página a la que se navega es un documento nuevo.</span><span class="sxs-lookup"><span data-stu-id="5e27f-113">True if the page being navigated to is a new document.</span></span>

> <span data-ttu-id="5e27f-114">[get_IsNewDocument](#get_isnewdocument)de HRESULT público (bool \* IsNewDocument)</span><span class="sxs-lookup"><span data-stu-id="5e27f-114">public HRESULT [get_IsNewDocument](#get_isnewdocument)(BOOL \* isNewDocument)</span></span>
