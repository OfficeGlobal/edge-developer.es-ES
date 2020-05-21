---
description: Hospedar contenido web en la aplicación Win32 con el control de WebView 2 de Microsoft Edge
title: Control WebView2 de Microsoft Edge
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 05/19/2020
ms.topic: conceptual
ms.prod: microsoft-edge
ms.technology: webview
keywords: IWebView2, IWebView2WebView, webview2, WebView, aplicaciones Win32, Win32, Edge, ICoreWebView2, CoreWebView2, ICoreWebView2Host, control del explorador, HTML Edge, Windows Forms, WinForms, WPF, .NET
ms.openlocfilehash: 184a64fde28345cd52dd6d772284f0393114ec02
ms.sourcegitcommit: 5bdffe91a6594f77eeffa4e864fda90a02784771
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/19/2020
ms.locfileid: "10659639"
---
# <span data-ttu-id="e723c-104">Introducción a Microsoft Edge WebView2 (versión preliminar)</span><span class="sxs-lookup"><span data-stu-id="e723c-104">Introduction to Microsoft Edge WebView2 (Preview)</span></span>  

<span data-ttu-id="e723c-105">El control Microsoft Edge WebView2 permite incrustar tecnologías web \ (HTML, CSS y JavaScript \) en las aplicaciones nativas.</span><span class="sxs-lookup"><span data-stu-id="e723c-105">The Microsoft Edge WebView2 control enables you to embed web technologies \(HTML, CSS, and JavaScript\) in your native applications.</span></span>  <span data-ttu-id="e723c-106">El control WebView2 usa [Microsoft Edge (cromo)](https://www.microsoftedgeinsider.com) como motor de representación para mostrar el contenido web en aplicaciones nativas.</span><span class="sxs-lookup"><span data-stu-id="e723c-106">The WebView2 control uses [Microsoft Edge (Chromium)](https://www.microsoftedgeinsider.com) as the rendering engine to display the web content in native applications.</span></span>  <span data-ttu-id="e723c-107">Con WebView2, puedes incrustar código web en diferentes partes de tu aplicación nativa o compilar toda la aplicación nativa dentro de una sola vista Web.</span><span class="sxs-lookup"><span data-stu-id="e723c-107">With WebView2, you may embed web code in different parts of your native application, or build the entire native application within a single WebView.</span></span>  <span data-ttu-id="e723c-108">Para obtener información sobre cómo empezar a crear una aplicación de WebView2, consulte [Introducción](./index.md#getting-started).</span><span class="sxs-lookup"><span data-stu-id="e723c-108">For information on how to start building a WebView2 application, see [Get Started](./index.md#getting-started).</span></span>  

:::image type="complex" source="./media/WebView2/whatwebview.png" alt-text="¿Qué es la vista previa?":::
   <span data-ttu-id="e723c-110">¿Qué es la vista previa?</span><span class="sxs-lookup"><span data-stu-id="e723c-110">What is WebView</span></span>  
:::image-end:::  

> [!NOTE]
> <span data-ttu-id="e723c-111">La vista previa de WebView2 está pensada para el prototipo anticipado y para recopilar comentarios con el fin de ayudar a dar forma a la API.</span><span class="sxs-lookup"><span data-stu-id="e723c-111">The WebView2 Preview is intended for early prototyping and to gather feedback to help to shape the API.</span></span>  <span data-ttu-id="e723c-112">El equipo de WebView de Microsoft Edge no recomienda usar la vista previa en las aplicaciones de producción porque es posible que se [produzcan cambios importantes](./releasenotes.md).</span><span class="sxs-lookup"><span data-stu-id="e723c-112">The Microsoft Edge WebView team does not recommend that you use the preview in your production apps because there may be [breaking changes](./releasenotes.md).</span></span>  

## <span data-ttu-id="e723c-113">Enfoque de aplicaciones híbridas</span><span class="sxs-lookup"><span data-stu-id="e723c-113">Hybrid Application Approach</span></span>  

<span data-ttu-id="e723c-114">Los programadores suelen tener que elegir entre crear una aplicación web o una aplicación nativa.</span><span class="sxs-lookup"><span data-stu-id="e723c-114">Developers often have to choose between building a web application or a native application.</span></span>  <span data-ttu-id="e723c-115">La decisión depende del equilibrio entre el alcance y el potencial de energía.</span><span class="sxs-lookup"><span data-stu-id="e723c-115">The decision hinges on the trade-off between reach and power.</span></span>  <span data-ttu-id="e723c-116">Las aplicaciones web permiten un amplio alcance.</span><span class="sxs-lookup"><span data-stu-id="e723c-116">Web applications allow for a broad reach.</span></span>  <span data-ttu-id="e723c-117">Como desarrollador web, puede volver a usar la mayoría, si no todo el código, en todas las plataformas.</span><span class="sxs-lookup"><span data-stu-id="e723c-117">As a Web developer, you may reuse most, if not all of your code, across all different platforms.</span></span>  <span data-ttu-id="e723c-118">Las aplicaciones nativas, sin embargo, usan las capacidades de toda la plataforma nativa.</span><span class="sxs-lookup"><span data-stu-id="e723c-118">Native applications, however, utilize the capabilities of the entire native platform.</span></span>  

:::image type="complex" source="./media/WebView2/webnative.png" alt-text="Web Native":::
   <span data-ttu-id="e723c-120">Web Native</span><span class="sxs-lookup"><span data-stu-id="e723c-120">Web native</span></span>  
:::image-end:::  

<span data-ttu-id="e723c-121">Las aplicaciones híbridas permiten a los desarrolladores disfrutar de lo mejor de ambos mundos.</span><span class="sxs-lookup"><span data-stu-id="e723c-121">Hybrid applications allow developers to enjoy the best of both worlds.</span></span>  <span data-ttu-id="e723c-122">Los programadores de aplicaciones híbridas se benefician de la Ubiquity y fortaleza de la plataforma web, así como de la potencia y capacidades completas de la plataforma nativa.</span><span class="sxs-lookup"><span data-stu-id="e723c-122">Hybrid application developers benefit from the ubiquity and strength of the web platform, and the power and full capabilities of the native platform.</span></span>  

## <span data-ttu-id="e723c-123">Beneficios de WebView2</span><span class="sxs-lookup"><span data-stu-id="e723c-123">WebView2 Benefits</span></span>   

:::image type="complex" source="./media/WebView2/webviewreasons.png" alt-text="Motivos de la vista en vista previa":::
   <span data-ttu-id="e723c-125">Motivos de la vista en vista previa</span><span class="sxs-lookup"><span data-stu-id="e723c-125">WebView reasons</span></span>  
:::image-end:::  

:::row:::
   :::column span="1":::
      **<span data-ttu-id="e723c-126">Ecosistema web \ & Aptitudes</span><span class="sxs-lookup"><span data-stu-id="e723c-126">Web ecosystem \& skillset</span></span>**  
      <span data-ttu-id="e723c-127">Use toda la plataforma web, bibliotecas, herramientas y talento que existen en el ecosistema Web.</span><span class="sxs-lookup"><span data-stu-id="e723c-127">Utilize the entire web platform, libraries, tooling, and talent that exists within the web ecosystem.</span></span>  
   :::column-end:::
   :::column span="1":::
      **<span data-ttu-id="e723c-128">Innovación rápida</span><span class="sxs-lookup"><span data-stu-id="e723c-128">Rapid Innovation</span></span>**  
      <span data-ttu-id="e723c-129">El desarrollo web permite una implementación e iteración más rápidas.</span><span class="sxs-lookup"><span data-stu-id="e723c-129">Web development allows for faster deployment and iteration.</span></span>  
   :::column-end:::
   :::column span="1":::
      **<span data-ttu-id="e723c-130">Compatibilidad con Windows 7, 8, 10</span><span class="sxs-lookup"><span data-stu-id="e723c-130">Windows 7, 8, 10 Support</span></span>**  
      <span data-ttu-id="e723c-131">Compatibilidad con una experiencia de usuario coherente en Windows 7, 8 y 10.</span><span class="sxs-lookup"><span data-stu-id="e723c-131">Support for a consistent user experience across Windows 7, 8, and 10.</span></span>  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
      **<span data-ttu-id="e723c-132">Capacidades nativas</span><span class="sxs-lookup"><span data-stu-id="e723c-132">Native capabilities</span></span>**  
      <span data-ttu-id="e723c-133">Acceder al conjunto completo de API nativas.</span><span class="sxs-lookup"><span data-stu-id="e723c-133">Access the full set of Native APIs.</span></span>  
   :::column-end:::
   :::column span="1":::
      **<span data-ttu-id="e723c-134">Uso compartido de código</span><span class="sxs-lookup"><span data-stu-id="e723c-134">Code-sharing</span></span>**  
      <span data-ttu-id="e723c-135">Agregar código web a su código base permite un aumento de la reutilización en varias plataformas.</span><span class="sxs-lookup"><span data-stu-id="e723c-135">Add web code to your codebase allows for increased re-use across multiple platforms.</span></span>  
   :::column-end:::
   :::column span="1":::
      **<span data-ttu-id="e723c-136">Soporte técnico de Microsoft</span><span class="sxs-lookup"><span data-stu-id="e723c-136">Microsoft support</span></span>**  
      <span data-ttu-id="e723c-137">Microsoft proporciona soporte técnico y agrega nuevas solicitudes de características cuando WebView2 se publica como GA.</span><span class="sxs-lookup"><span data-stu-id="e723c-137">Microsoft provides support and adds new feature requests when WebView2 is release as GA.</span></span>  
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="1":::
      **<span data-ttu-id="e723c-138">Distribución de hoja perenne</span><span class="sxs-lookup"><span data-stu-id="e723c-138">Evergreen distribution</span></span>**  
      <span data-ttu-id="e723c-139">Use una versión actualizada de cromo con actualizaciones de plataforma y revisiones de seguridad regulares.</span><span class="sxs-lookup"><span data-stu-id="e723c-139">Rely on an up-to-date version of Chromium with regular platform updates and security patches.</span></span>  
   :::column-end:::
   :::column span="1":::
      <span data-ttu-id="e723c-140">**Fijo** \ (próximamente \)</span><span class="sxs-lookup"><span data-stu-id="e723c-140">**Fixed** \(coming soon\)</span></span>  
      <span data-ttu-id="e723c-141">Elija empaquetar los bits de cromo en la aplicación.</span><span class="sxs-lookup"><span data-stu-id="e723c-141">Choose to package the Chromium bits in your application.</span></span>  
   :::column-end:::
   :::column span="1":::
      **<span data-ttu-id="e723c-142">Adopción incremental</span><span class="sxs-lookup"><span data-stu-id="e723c-142">Incremental adoption</span></span>**  
      <span data-ttu-id="e723c-143">Agregue componentes Web por partes a la aplicación.</span><span class="sxs-lookup"><span data-stu-id="e723c-143">Add web components piece by piece to your application.</span></span>  
   :::column-end:::
:::row-end:::  

## <span data-ttu-id="e723c-144">Tareas iniciales</span><span class="sxs-lookup"><span data-stu-id="e723c-144">Getting Started</span></span>  

<span data-ttu-id="e723c-145">Para compilar y probar la aplicación con el control WebView2, debe tener instalado tanto [Microsoft Edge (cromo)](https://www.microsoftedgeinsider.com/download) como el [SDK de WebView2](https://aka.ms/webviewnuget) .</span><span class="sxs-lookup"><span data-stu-id="e723c-145">To build and test your application using the WebView2 control, you need to have both [Microsoft Edge (Chromium)](https://www.microsoftedgeinsider.com/download) and the [WebView2 SDK](https://aka.ms/webviewnuget) installed.</span></span>  <span data-ttu-id="e723c-146">Seleccione una de las siguientes opciones para comenzar.</span><span class="sxs-lookup"><span data-stu-id="e723c-146">Select one of the following options to get started.</span></span>  

*   [<span data-ttu-id="e723c-147">Introducción a Win32 C/C++</span><span class="sxs-lookup"><span data-stu-id="e723c-147">Getting Started with Win32 C/C++</span></span>](./gettingstarted/win32.md)  
*   [<span data-ttu-id="e723c-148">Introducción a WPF</span><span class="sxs-lookup"><span data-stu-id="e723c-148">Getting Started with WPF</span></span>](./gettingstarted/wpf.md)  
*   [<span data-ttu-id="e723c-149">Introducción a WinForms</span><span class="sxs-lookup"><span data-stu-id="e723c-149">Getting Started with WinForms</span></span>](./gettingstarted/winforms.md)  

<span data-ttu-id="e723c-150">El repositorio de [muestras de WebView2](https://github.com/MicrosoftEdge/WebView2Samples) contiene ejemplos que muestran todas las características de los SDK de WebView2 y los patrones de uso de API.</span><span class="sxs-lookup"><span data-stu-id="e723c-150">The [WebView2 Samples](https://github.com/MicrosoftEdge/WebView2Samples) repository contains samples that demonstrate all of the WebView2 SDKs features and API usage patterns.</span></span> <span data-ttu-id="e723c-151">A medida que se agregan más características al SDK de WebView2, se actualizarán las aplicaciones de ejemplo.</span><span class="sxs-lookup"><span data-stu-id="e723c-151">As more features are added to the WebView2 SDK, the sample applications will be updated.</span></span>   

## <span data-ttu-id="e723c-152">Plataformas compatibles</span><span class="sxs-lookup"><span data-stu-id="e723c-152">Supported Platforms</span></span>  

<span data-ttu-id="e723c-153">Una vista previa para desarrolladores está disponible en los siguientes entornos de programación.</span><span class="sxs-lookup"><span data-stu-id="e723c-153">A developer preview is available on the following programming environments.</span></span>  

*   <span data-ttu-id="e723c-154">C/C++ Win32</span><span class="sxs-lookup"><span data-stu-id="e723c-154">Win32 C/C++</span></span>  
*   <span data-ttu-id="e723c-155">.NET Framework 4.6.2 o posterior</span><span class="sxs-lookup"><span data-stu-id="e723c-155">.NET Framework 4.6.2 or later</span></span>  
*   <span data-ttu-id="e723c-156">.NET Core 3,0 o posterior</span><span class="sxs-lookup"><span data-stu-id="e723c-156">.NET Core 3.0 or later</span></span>  
*   [<span data-ttu-id="e723c-157">WinUI 3,0</span><span class="sxs-lookup"><span data-stu-id="e723c-157">WinUI 3.0</span></span>](/uwp/toolkits/winui3/)  

<span data-ttu-id="e723c-158">Mun ejecuta Windows 10, Windows 8,1, Windows 8, Windows 7, Windows Server 2016, Windows Server 2012/2012R2 o Windows Server 2008 R2.</span><span class="sxs-lookup"><span data-stu-id="e723c-158">You mun run Windows 10, Windows 8.1, Windows 8, Windows 7, Windows Server 2016, Windows Server 2012/2012R2, or Windows Server 2008 R2.</span></span>   

## <span data-ttu-id="e723c-159">Pasos siguientes</span><span class="sxs-lookup"><span data-stu-id="e723c-159">Next Steps</span></span>  

<span data-ttu-id="e723c-160">Para obtener información más detallada sobre cómo crear e implementar aplicaciones de WebView2, desproteja nuestra documentación conceptual</span><span class="sxs-lookup"><span data-stu-id="e723c-160">For more detailed information on how to build and deploy WebView2 applications, checkout our conceptual documentation</span></span><!-- and how-to guides--><span data-ttu-id="e723c-161">.</span><span class="sxs-lookup"><span data-stu-id="e723c-161">.</span></span>  

#### <span data-ttu-id="e723c-162">Conceptos</span><span class="sxs-lookup"><span data-stu-id="e723c-162">Concepts</span></span>  

*   [<span data-ttu-id="e723c-163">SDK de WebView2 y versiones de Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="e723c-163">WebView2 SDK and Microsoft Edge Versioning</span></span>](./concepts/versioning.md)
*   [<span data-ttu-id="e723c-164">Distribuir aplicaciones de WebView2</span><span class="sxs-lookup"><span data-stu-id="e723c-164">Distributing WebView2 Applications</span></span>](./concepts/distribution.md)  
 
#### <span data-ttu-id="e723c-165">Guías de procedimientos</span><span class="sxs-lookup"><span data-stu-id="e723c-165">How-To Guides</span></span>  

*   [<span data-ttu-id="e723c-166">Depurar WebView2 con DevTools y la depuración de scripts de Visual Studio</span><span class="sxs-lookup"><span data-stu-id="e723c-166">Debugging WebView2 with DevTools and Visual Studio Script Debugging</span></span>](./howto/debug.md)  
*   [<span data-ttu-id="e723c-167">Automatizar y depurar WebView2 con Microsoft EdgeDriver</span><span class="sxs-lookup"><span data-stu-id="e723c-167">Automating and Debugging WebView2 with Microsoft EdgeDriver</span></span>](./howto/webdriver.md)  

<!--todo: add how-tos when available  -->  

## <span data-ttu-id="e723c-168">Ponerse en contacto con el equipo de WebView2</span><span class="sxs-lookup"><span data-stu-id="e723c-168">Getting in touch with the WebView2 team</span></span>  

<span data-ttu-id="e723c-169">Ayuda a crear una experiencia WebView2 más rica compartiendo tus comentarios.</span><span class="sxs-lookup"><span data-stu-id="e723c-169">Help build a richer WebView2 experience by sharing your feedback.</span></span>  <span data-ttu-id="e723c-170">Visita el repositorio de [comentarios](https://aka.ms/webviewfeedback) de WebView para enviar solicitudes de características o informes de errores.</span><span class="sxs-lookup"><span data-stu-id="e723c-170">Visit the WebView [feedback repo](https://aka.ms/webviewfeedback) to submit feature requests or bug reports.</span></span>  <span data-ttu-id="e723c-171">También es un buen lugar para buscar problemas conocidos.</span><span class="sxs-lookup"><span data-stu-id="e723c-171">It is also a good place to search for known issues.</span></span>  

> [!NOTE]
> <span data-ttu-id="e723c-172">Durante la vista previa del desarrollador, el equipo de WebView de Microsoft Edge también recopila datos para ayudar a crear una vista previa mejorada.</span><span class="sxs-lookup"><span data-stu-id="e723c-172">During developer preview, the Microsoft Edge WebView team also collects data to help build a better WebView.</span></span>  <span data-ttu-id="e723c-173">Los usuarios pueden desactivar la recopilación de datos de WebView desplazándose a `edge://settings/privacy` en el explorador Microsoft Edge y desactivando la recopilación de datos del explorador.</span><span class="sxs-lookup"><span data-stu-id="e723c-173">Users may turn off WebView data collection by navigating to `edge://settings/privacy` in the Microsoft Edge browser and turning off browser data collection.</span></span>  