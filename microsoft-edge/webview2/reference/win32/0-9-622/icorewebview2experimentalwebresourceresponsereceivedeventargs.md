---
description: Insertar tecnologías web (HTML, CSS y JavaScript) en las aplicaciones nativas con el control Microsoft Edge WebView2
title: WebView2 Win32 C++ ICoreWebView2ExperimentalWebResourceResponseReceivedEventArgs
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 09/10/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, ICoreWebView2Controller, control de explorador, HTML Edge, ICoreWebView2ExperimentalWebResourceResponseReceivedEventArgs
ms.openlocfilehash: 552421aa003be2ea52493f16ad94ed2b08e8c3a9
ms.sourcegitcommit: 0faf538d5033508af4320b9b89c4ed99872f0574
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/10/2020
ms.locfileid: "11012703"
---
# <span data-ttu-id="65339-104">interfaz ICoreWebView2ExperimentalWebResourceResponseReceivedEventArgs</span><span class="sxs-lookup"><span data-stu-id="65339-104">interface ICoreWebView2ExperimentalWebResourceResponseReceivedEventArgs</span></span> 

[!INCLUDE [prerelease-note](../../includes/prerelease-note.md)]

```
interface ICoreWebView2ExperimentalWebResourceResponseReceivedEventArgs
  : public IUnknown
```

<span data-ttu-id="65339-105">Argumentos de evento para el evento WebResourceResponseReceived.</span><span class="sxs-lookup"><span data-stu-id="65339-105">Event args for the WebResourceResponseReceived event.</span></span>

## <span data-ttu-id="65339-106">Resumen</span><span class="sxs-lookup"><span data-stu-id="65339-106">Summary</span></span>

 <span data-ttu-id="65339-107">Miembros</span><span class="sxs-lookup"><span data-stu-id="65339-107">Members</span></span>                        | <span data-ttu-id="65339-108">Descripciones</span><span class="sxs-lookup"><span data-stu-id="65339-108">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="65339-109">get_Request</span><span class="sxs-lookup"><span data-stu-id="65339-109">get_Request</span></span>](#get_request) | <span data-ttu-id="65339-110">Objeto de solicitud de recursos Web.</span><span class="sxs-lookup"><span data-stu-id="65339-110">Web resource request object.</span></span> <span data-ttu-id="65339-111">Se omitirán todas las modificaciones realizadas a este objeto.</span><span class="sxs-lookup"><span data-stu-id="65339-111">Any modifications to this object will be ignored.</span></span>
[<span data-ttu-id="65339-112">get_Response</span><span class="sxs-lookup"><span data-stu-id="65339-112">get_Response</span></span>](#get_response) | <span data-ttu-id="65339-113">Objeto de respuesta de recursos Web.</span><span class="sxs-lookup"><span data-stu-id="65339-113">Web resource response object.</span></span>
[<span data-ttu-id="65339-114">PopulateResponseContent</span><span class="sxs-lookup"><span data-stu-id="65339-114">PopulateResponseContent</span></span>](#populateresponsecontent) | <span data-ttu-id="65339-115">Método Async para solicitar la secuencia de contenido de la respuesta.</span><span class="sxs-lookup"><span data-stu-id="65339-115">Async method to request the Content stream of the response.</span></span>

<span data-ttu-id="65339-116">Contendrá la solicitud a medida que se envió y la respuesta a medida que se recibió.</span><span class="sxs-lookup"><span data-stu-id="65339-116">Will contain the request as it was sent and the response as it was received.</span></span> <span data-ttu-id="65339-117">Nota: para obtener la secuencia de contenido de la respuesta, primero llame a PopulateResponseContent y espere a que se complete la llamada asincrónica, de lo contrario el objeto de la secuencia de contenido devuelto será null.</span><span class="sxs-lookup"><span data-stu-id="65339-117">Note: To get the response content stream, first call PopulateResponseContent and wait for the async call to complete, otherwise the content stream object returned will be null.</span></span>

## <span data-ttu-id="65339-118">Miembros</span><span class="sxs-lookup"><span data-stu-id="65339-118">Members</span></span>

#### <span data-ttu-id="65339-119">get_Request</span><span class="sxs-lookup"><span data-stu-id="65339-119">get_Request</span></span> 

<span data-ttu-id="65339-120">Objeto de solicitud de recursos Web.</span><span class="sxs-lookup"><span data-stu-id="65339-120">Web resource request object.</span></span> <span data-ttu-id="65339-121">Se omitirán todas las modificaciones realizadas a este objeto.</span><span class="sxs-lookup"><span data-stu-id="65339-121">Any modifications to this object will be ignored.</span></span>

> <span data-ttu-id="65339-122">[get_Request](#get_request)de HRESULT público (solicitud[ICoreWebView2WebResourceRequest](icorewebview2webresourcerequest.md) \* \*)</span><span class="sxs-lookup"><span data-stu-id="65339-122">public HRESULT [get_Request](#get_request)([ICoreWebView2WebResourceRequest](icorewebview2webresourcerequest.md) \*\* request)</span></span>

#### <span data-ttu-id="65339-123">get_Response</span><span class="sxs-lookup"><span data-stu-id="65339-123">get_Response</span></span> 

<span data-ttu-id="65339-124">Objeto de respuesta de recursos Web.</span><span class="sxs-lookup"><span data-stu-id="65339-124">Web resource response object.</span></span>

> <span data-ttu-id="65339-125">[get_Response](#get_response)de HRESULT público (respuesta de[ICoreWebView2WebResourceResponse](icorewebview2webresourceresponse.md) \* \*)</span><span class="sxs-lookup"><span data-stu-id="65339-125">public HRESULT [get_Response](#get_response)([ICoreWebView2WebResourceResponse](icorewebview2webresourceresponse.md) \*\* response)</span></span>

<span data-ttu-id="65339-126">Se omitirán todas las modificaciones realizadas a este objeto.</span><span class="sxs-lookup"><span data-stu-id="65339-126">Any modifications to this object will be ignored.</span></span>

#### <span data-ttu-id="65339-127">PopulateResponseContent</span><span class="sxs-lookup"><span data-stu-id="65339-127">PopulateResponseContent</span></span> 

<span data-ttu-id="65339-128">Método Async para solicitar la secuencia de contenido de la respuesta.</span><span class="sxs-lookup"><span data-stu-id="65339-128">Async method to request the Content stream of the response.</span></span>

> <span data-ttu-id="65339-129">[PopulateResponseContent](#populateresponsecontent)(controlador[ICoreWebView2ExperimentalWebResourceResponseReceivedEventArgsPopulateResponseContentCompletedHandler](icorewebview2experimentalwebresourceresponsereceivedeventargspopulateresponsecontentcompletedhandler.md) \*) Public HRESULT</span><span class="sxs-lookup"><span data-stu-id="65339-129">public HRESULT [PopulateResponseContent](#populateresponsecontent)([ICoreWebView2ExperimentalWebResourceResponseReceivedEventArgsPopulateResponseContentCompletedHandler](icorewebview2experimentalwebresourceresponsereceivedeventargspopulateresponsecontentcompletedhandler.md) \* handler)</span></span>

```cpp
                    args->PopulateResponseContent(
                        Callback<
                            ICoreWebView2ExperimentalWebResourceResponseReceivedEventArgsPopulateResponseContentCompletedHandler>(
                            [this, webResourceRequest, webResourceResponse](HRESULT result) {
                                std::wstring message =
                                    L"{ \"kind\": \"event\", \"name\": "
                                    L"\"WebResourceResponseReceived\", \"args\": {"
                                    L"\"request\": " +
                                    RequestToJsonString(webResourceRequest.get()) +
                                    L", "
                                    L"\"response\": " +
                                    ResponseToJsonString(webResourceResponse.get()) + L"}";

                                message +=
                                    WebViewPropertiesToJsonString(m_webviewEventSource.get());
                                message += L"}";
                                PostEventMessage(message);
                                return S_OK;
                            })
                            .Get());
```
