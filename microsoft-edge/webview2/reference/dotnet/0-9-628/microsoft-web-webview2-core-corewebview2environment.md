---
description: Insertar tecnologías web (HTML, CSS y JavaScript) en las aplicaciones nativas con el control Microsoft Edge WebView2
title: Microsoft. Web. WebView2. Core. CoreWebView2Environment
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 09/11/2020
ms.topic: reference
ms.prod: microsoft-edge
ms.technology: webview
keywords: Microsoft. Web. WebView2, Core, WebView2, WebView, dotnet, WPF, WinForms, App, Edge, CoreWebView2, CoreWebView2Controller, control de explorador, Edge HTML, Microsoft. Web. WebView2. Core. CoreWebView2Environment
ms.openlocfilehash: 05b8a10c723ae57b2c95551f4d5043f3336eba3b
ms.sourcegitcommit: 65db518273b3cd69f1b3c528809600719b9b70aa
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/16/2020
ms.locfileid: "11016329"
---
# <span data-ttu-id="a695d-104">Clase Microsoft. Web. WebView2. Core. CoreWebView2Environment</span><span class="sxs-lookup"><span data-stu-id="a695d-104">Microsoft.Web.WebView2.Core.CoreWebView2Environment class</span></span> 

<span data-ttu-id="a695d-105">Espacio de nombres: Microsoft. Web. WebView2. Core </span><span class="sxs-lookup"><span data-stu-id="a695d-105">Namespace: Microsoft.Web.WebView2.Core</span></span>\
<span data-ttu-id="a695d-106">Ensamblado: Microsoft.Web.WebView2.Core.dll</span><span class="sxs-lookup"><span data-stu-id="a695d-106">Assembly: Microsoft.Web.WebView2.Core.dll</span></span>

<span data-ttu-id="a695d-107">Esto representa el entorno de WebView2.</span><span class="sxs-lookup"><span data-stu-id="a695d-107">This represents the WebView2 Environment.</span></span>

## <span data-ttu-id="a695d-108">Resumen</span><span class="sxs-lookup"><span data-stu-id="a695d-108">Summary</span></span>

 <span data-ttu-id="a695d-109">Miembros</span><span class="sxs-lookup"><span data-stu-id="a695d-109">Members</span></span>                        | <span data-ttu-id="a695d-110">Descripciones</span><span class="sxs-lookup"><span data-stu-id="a695d-110">Descriptions</span></span>
--------------------------------|---------------------------------------------
[<span data-ttu-id="a695d-111">BrowserVersionString</span><span class="sxs-lookup"><span data-stu-id="a695d-111">BrowserVersionString</span></span>](#browserversionstring) | <span data-ttu-id="a695d-112">Información de versión del explorador del CoreWebView2Environment actual, incluido el nombre del canal si no es el canal estable.</span><span class="sxs-lookup"><span data-stu-id="a695d-112">The browser version info of the current CoreWebView2Environment, including channel name if it is not the stable channel.</span></span>
[<span data-ttu-id="a695d-113">NewBrowserVersionAvailable</span><span class="sxs-lookup"><span data-stu-id="a695d-113">NewBrowserVersionAvailable</span></span>](#newbrowserversionavailable) | <span data-ttu-id="a695d-114">NewBrowserVersionAvailable se desencadena cuando se instala una versión más reciente del explorador Edge y está disponible para su uso a través de WebView2.</span><span class="sxs-lookup"><span data-stu-id="a695d-114">NewBrowserVersionAvailable fires when a newer version of the Edge browser is installed and available for use via WebView2.</span></span>
[<span data-ttu-id="a695d-115">CompareBrowserVersions</span><span class="sxs-lookup"><span data-stu-id="a695d-115">CompareBrowserVersions</span></span>](#comparebrowserversions) | <span data-ttu-id="a695d-116">Compare las versiones del explorador para determinar si coinciden o son diferentes.</span><span class="sxs-lookup"><span data-stu-id="a695d-116">Compare browser versions to determine if they match or are different.</span></span>
[<span data-ttu-id="a695d-117">CreateAsync</span><span class="sxs-lookup"><span data-stu-id="a695d-117">CreateAsync</span></span>](#createasync) | <span data-ttu-id="a695d-118">Crea un entorno de WebView2 de perenne con la versión instalada de Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a695d-118">Creates an evergreen WebView2 Environment using the installed version of Microsoft Edge.</span></span>
[<span data-ttu-id="a695d-119">CreateCoreWebView2CompositionControllerAsync</span><span class="sxs-lookup"><span data-stu-id="a695d-119">CreateCoreWebView2CompositionControllerAsync</span></span>](#createcorewebview2compositioncontrollerasync) | <span data-ttu-id="a695d-120">Cree de forma asincrónica una nueva vista de vista para usarla con el hospedaje visual.</span><span class="sxs-lookup"><span data-stu-id="a695d-120">Asynchronously create a new WebView for use with visual hosting.</span></span>
[<span data-ttu-id="a695d-121">CreateCoreWebView2ControllerAsync</span><span class="sxs-lookup"><span data-stu-id="a695d-121">CreateCoreWebView2ControllerAsync</span></span>](#createcorewebview2controllerasync) | <span data-ttu-id="a695d-122">Cree de forma asincrónica una nueva vista de vista previa.</span><span class="sxs-lookup"><span data-stu-id="a695d-122">Asynchronously create a new WebView.</span></span>
[<span data-ttu-id="a695d-123">CreateCoreWebView2PointerInfo</span><span class="sxs-lookup"><span data-stu-id="a695d-123">CreateCoreWebView2PointerInfo</span></span>](#createcorewebview2pointerinfo) | <span data-ttu-id="a695d-124">Cree un CoreWebView2PointerInfo vacío.</span><span class="sxs-lookup"><span data-stu-id="a695d-124">Create an empty CoreWebView2PointerInfo.</span></span>
[<span data-ttu-id="a695d-125">CreateWebResourceResponse</span><span class="sxs-lookup"><span data-stu-id="a695d-125">CreateWebResourceResponse</span></span>](#createwebresourceresponse) | <span data-ttu-id="a695d-126">Crear un nuevo objeto de respuesta de recursos Web.</span><span class="sxs-lookup"><span data-stu-id="a695d-126">Create a new web resource response object.</span></span>
[<span data-ttu-id="a695d-127">GetAvailableBrowserVersionString</span><span class="sxs-lookup"><span data-stu-id="a695d-127">GetAvailableBrowserVersionString</span></span>](#getavailablebrowserversionstring) | <span data-ttu-id="a695d-128">Obtener la información de versión del explorador.</span><span class="sxs-lookup"><span data-stu-id="a695d-128">Get the browser version information.</span></span>
[<span data-ttu-id="a695d-129">GetProviderForHwnd</span><span class="sxs-lookup"><span data-stu-id="a695d-129">GetProviderForHwnd</span></span>](#getproviderforhwnd) | <span data-ttu-id="a695d-130">Devuelve el proveedor de automatización de la interfaz de usuario de la CoreWebView2CompositionController que se corresponde con el HWND dado.</span><span class="sxs-lookup"><span data-stu-id="a695d-130">Returns the UI Automation Provider for the CoreWebView2CompositionController that corresponds with the given HWND.</span></span>

<span data-ttu-id="a695d-131">Las vistas web creadas a partir de un entorno se ejecutan en el proceso del explorador especificado con los parámetros de entorno y los objetos creados a partir de un entorno se deben usar en el mismo entorno.</span><span class="sxs-lookup"><span data-stu-id="a695d-131">WebViews created from an environment run on the Browser process specified with environment parameters and objects created from an environment should be used in the same environment.</span></span> <span data-ttu-id="a695d-132">No se garantiza que su uso en diferentes entornos sea compatible y podría fallar.</span><span class="sxs-lookup"><span data-stu-id="a695d-132">Using it in different environments are not guaranteed to be compatible and may fail.</span></span> 

## <span data-ttu-id="a695d-133">Miembros</span><span class="sxs-lookup"><span data-stu-id="a695d-133">Members</span></span>

#### <span data-ttu-id="a695d-134">BrowserVersionString</span><span class="sxs-lookup"><span data-stu-id="a695d-134">BrowserVersionString</span></span> 

<span data-ttu-id="a695d-135">Información de versión del explorador del CoreWebView2Environment actual, incluido el nombre del canal si no es el canal estable.</span><span class="sxs-lookup"><span data-stu-id="a695d-135">The browser version info of the current CoreWebView2Environment, including channel name if it is not the stable channel.</span></span>

> <span data-ttu-id="a695d-136">cadena pública [BrowserVersionString](#browserversionstring)</span><span class="sxs-lookup"><span data-stu-id="a695d-136">public string [BrowserVersionString](#browserversionstring)</span></span>

<span data-ttu-id="a695d-137">Coincide con el formato de la API de GetAvailableCoreWebView2BrowserVersionString.</span><span class="sxs-lookup"><span data-stu-id="a695d-137">This matches the format of the GetAvailableCoreWebView2BrowserVersionString API.</span></span> <span data-ttu-id="a695d-138">Los nombres de los canales son ' beta ', ' dev ' y ' Canarias '.</span><span class="sxs-lookup"><span data-stu-id="a695d-138">Channel names are 'beta', 'dev', and 'canary'.</span></span>

#### <span data-ttu-id="a695d-139">NewBrowserVersionAvailable</span><span class="sxs-lookup"><span data-stu-id="a695d-139">NewBrowserVersionAvailable</span></span> 

<span data-ttu-id="a695d-140">NewBrowserVersionAvailable se desencadena cuando se instala una versión más reciente del explorador Edge y está disponible para su uso a través de WebView2.</span><span class="sxs-lookup"><span data-stu-id="a695d-140">NewBrowserVersionAvailable fires when a newer version of the Edge browser is installed and available for use via WebView2.</span></span>

> <span data-ttu-id="a695d-141">evento público EventHandler< > [NewBrowserVersionAvailable](#newbrowserversionavailable)</span><span class="sxs-lookup"><span data-stu-id="a695d-141">public event EventHandler< object > [NewBrowserVersionAvailable](#newbrowserversionavailable)</span></span>

<span data-ttu-id="a695d-142">Para usar la versión más reciente del explorador, debe crear un entorno y una vista Web nuevos.</span><span class="sxs-lookup"><span data-stu-id="a695d-142">To use the newer version of the browser you must create a new environment and WebView.</span></span> <span data-ttu-id="a695d-143">Este evento solo se activará para la nueva versión desde el mismo canal de borde desde el que se está ejecutando el código.</span><span class="sxs-lookup"><span data-stu-id="a695d-143">This event will only be fired for new version from the same Edge channel that the code is running from.</span></span> <span data-ttu-id="a695d-144">Cuando no se esté ejecutando con Edge instalado, no se desencadenará ningún evento.</span><span class="sxs-lookup"><span data-stu-id="a695d-144">When not running with installed Edge, no event will be fired.</span></span>

<span data-ttu-id="a695d-145">Puesto que una carpeta datos de usuario solo puede ser usada por un único proceso del explorador a la vez, si desea usar la misma carpeta datos de usuario en las vistas web con la nueva versión del explorador, debe cerrar primero el entorno y las vistas de web que usan la versión anterior del explorador.</span><span class="sxs-lookup"><span data-stu-id="a695d-145">Because a user data folder can only be used by one browser process at a time, if you want to use the same user data folder in the WebViews using the new version of the browser, you must close the environment and WebViews that are using the older version of the browser first.</span></span> <span data-ttu-id="a695d-146">O simplemente pide al usuario que reinicie la aplicación.</span><span class="sxs-lookup"><span data-stu-id="a695d-146">Or simply prompt the user to restart the app.</span></span>

#### <span data-ttu-id="a695d-147">CompareBrowserVersions</span><span class="sxs-lookup"><span data-stu-id="a695d-147">CompareBrowserVersions</span></span> 

<span data-ttu-id="a695d-148">Compare las versiones del explorador para determinar si coinciden o son diferentes.</span><span class="sxs-lookup"><span data-stu-id="a695d-148">Compare browser versions to determine if they match or are different.</span></span>

> <span data-ttu-id="a695d-149">public static int [CompareBrowserVersions](#comparebrowserversions)(cadena version1, String version2)</span><span class="sxs-lookup"><span data-stu-id="a695d-149">public static int [CompareBrowserVersions](#comparebrowserversions)(string version1, string version2)</span></span>

<span data-ttu-id="a695d-150">Devuelve-1, 0 o 1 dependiendo de si la primera versión es menor, igual o superior a la que se compara con la segunda versión.</span><span class="sxs-lookup"><span data-stu-id="a695d-150">Returns -1, 0 or 1 depending on whether the first version is less than, equal to or greater than the second version being compared.</span></span>

<span data-ttu-id="a695d-151">La entrada puede usar directamente el versionInfo Obtenido de GetAvailableCoreWebView2BrowserVersionString, la información de canal se pasará por alto.</span><span class="sxs-lookup"><span data-stu-id="a695d-151">Input can directly use the versionInfo obtained from GetAvailableCoreWebView2BrowserVersionString, channel info will be ignored.</span></span>

##### <span data-ttu-id="a695d-152">Parameters</span><span class="sxs-lookup"><span data-stu-id="a695d-152">Parameters</span></span>
* `version1` <span data-ttu-id="a695d-153">Primera versión que se va a comparar.</span><span class="sxs-lookup"><span data-stu-id="a695d-153">The first version to compare.</span></span> 

* `version2` <span data-ttu-id="a695d-154">La segunda versión que se compara.</span><span class="sxs-lookup"><span data-stu-id="a695d-154">The second version to compare.</span></span>

#### <span data-ttu-id="a695d-155">CreateAsync</span><span class="sxs-lookup"><span data-stu-id="a695d-155">CreateAsync</span></span> 

<span data-ttu-id="a695d-156">Crea un entorno de WebView2 de perenne con la versión instalada de Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="a695d-156">Creates an evergreen WebView2 Environment using the installed version of Microsoft Edge.</span></span>

> <span data-ttu-id="a695d-157">tarea pública estática asincrónica< [CoreWebView2Environment](microsoft-web-webview2-core-corewebview2environment.md)  >  [CreateAsync](#createasync)(String browserExecutableFolder, String userDataFolder, CoreWebView2EnvironmentOptions Options)</span><span class="sxs-lookup"><span data-stu-id="a695d-157">public static async Task< [CoreWebView2Environment](microsoft-web-webview2-core-corewebview2environment.md) > [CreateAsync](#createasync)(string browserExecutableFolder, string userDataFolder, CoreWebView2EnvironmentOptions options)</span></span>

##### <span data-ttu-id="a695d-158">Parameters</span><span class="sxs-lookup"><span data-stu-id="a695d-158">Parameters</span></span>
* `browserExecutableFolder` <span data-ttu-id="a695d-159">La ruta de acceso relativa a la carpeta que contiene la versión fija del motor en tiempo de ejecución de WebView2.</span><span class="sxs-lookup"><span data-stu-id="a695d-159">The relative path to the folder that contains the fixed version of the WebView2 Runtime.</span></span> 

* `userDataFolder` <span data-ttu-id="a695d-160">userDataFolder se puede especificar para cambiar la ubicación de la carpeta de datos de usuario predeterminada para WebView2.</span><span class="sxs-lookup"><span data-stu-id="a695d-160">userDataFolder can be specified to change the default user data folder location for WebView2.</span></span> 

* `options` <span data-ttu-id="a695d-161">Opciones usadas para crear un entorno WebView2.</span><span class="sxs-lookup"><span data-stu-id="a695d-161">Options used to create WebView2 Environment.</span></span>

#### <span data-ttu-id="a695d-162">CreateCoreWebView2CompositionControllerAsync</span><span class="sxs-lookup"><span data-stu-id="a695d-162">CreateCoreWebView2CompositionControllerAsync</span></span> 

[!INCLUDE [prerelease-note](../../includes/prerelease-note.md)]

<span data-ttu-id="a695d-163">Cree de forma asincrónica una nueva vista de vista para usarla con el hospedaje visual.</span><span class="sxs-lookup"><span data-stu-id="a695d-163">Asynchronously create a new WebView for use with visual hosting.</span></span>

> <span data-ttu-id="a695d-164">tarea asincrónica pública< [CoreWebView2CompositionController](microsoft-web-webview2-core-corewebview2compositioncontroller.md)  >  [CreateCoreWebView2CompositionControllerAsync](#createcorewebview2compositioncontrollerasync)(IntPtr ParentWindow)</span><span class="sxs-lookup"><span data-stu-id="a695d-164">public async Task< [CoreWebView2CompositionController](microsoft-web-webview2-core-corewebview2compositioncontroller.md) > [CreateCoreWebView2CompositionControllerAsync](#createcorewebview2compositioncontrollerasync)(IntPtr ParentWindow)</span></span>

<span data-ttu-id="a695d-165">parentWindow es el HWND en el que la aplicación se conectará al árbol visual de la vista de ventana.</span><span class="sxs-lookup"><span data-stu-id="a695d-165">parentWindow is the HWND in which the app will connect the visual tree of the WebView.</span></span> <span data-ttu-id="a695d-166">Este es el HWND que la aplicación recibirá una entrada de puntero o de mouse para la vista de ventana (y deberá usar SendMouseInput/SendPointerInput para reenviar).</span><span class="sxs-lookup"><span data-stu-id="a695d-166">This will be the HWND that the app will receive pointer/ mouse input meant for the WebView (and will need to use SendMouseInput/ SendPointerInput to forward).</span></span> <span data-ttu-id="a695d-167">Si la aplicación mueve el árbol visual WebView a una ventana distinta de otra, debe establecer CoreWebView2CompositionController. ParentWindow para actualizar el nuevo HWND primario del árbol visual.</span><span class="sxs-lookup"><span data-stu-id="a695d-167">If the app moves the WebView visual tree to underneath a different window, then it needs to set CoreWebView2CompositionController.ParentWindow to update the new parent HWND of the visual tree.</span></span>

<span data-ttu-id="a695d-168">Establezca la propiedad RootVisualTarget en el CoreWebView2CompositionController creado para proporcionar un objeto visual que hospede el árbol visual del explorador.</span><span class="sxs-lookup"><span data-stu-id="a695d-168">Set RootVisualTarget property on the created CoreWebView2CompositionController to provide a visual to host the browser's visual tree.</span></span>

<span data-ttu-id="a695d-169">Se recomienda que el identificador de modelo de usuario de la aplicación conjunto de aplicaciones para el proceso o la ventana de la aplicación.</span><span class="sxs-lookup"><span data-stu-id="a695d-169">It is recommended that the application set Application User Model ID for the process or the application window.</span></span> <span data-ttu-id="a695d-170">Si no se establece ninguna, durante la creación de WebView un identificador de modelo de usuario de aplicación generado se establece en la ventana raíz de parentWindow.</span><span class="sxs-lookup"><span data-stu-id="a695d-170">If none is set, during WebView creation a generated Application User Model ID is set to root window of parentWindow.</span></span>

#### <span data-ttu-id="a695d-171">CreateCoreWebView2ControllerAsync</span><span class="sxs-lookup"><span data-stu-id="a695d-171">CreateCoreWebView2ControllerAsync</span></span> 

<span data-ttu-id="a695d-172">Cree de forma asincrónica una nueva vista de vista previa.</span><span class="sxs-lookup"><span data-stu-id="a695d-172">Asynchronously create a new WebView.</span></span>

> <span data-ttu-id="a695d-173">tarea asincrónica pública< [CoreWebView2Controller](microsoft-web-webview2-core-corewebview2controller.md)  >  [CreateCoreWebView2ControllerAsync](#createcorewebview2controllerasync)(IntPtr ParentWindow)</span><span class="sxs-lookup"><span data-stu-id="a695d-173">public async Task< [CoreWebView2Controller](microsoft-web-webview2-core-corewebview2controller.md) > [CreateCoreWebView2ControllerAsync](#createcorewebview2controllerasync)(IntPtr ParentWindow)</span></span>

<span data-ttu-id="a695d-174">parentWindow es el HWND en el que se debe mostrar la vista en la vista previa y desde la que se recibe la entrada.</span><span class="sxs-lookup"><span data-stu-id="a695d-174">parentWindow is the HWND in which the WebView should be displayed and from which receive input.</span></span> <span data-ttu-id="a695d-175">La vista en WebView agregará una ventana secundaria a la ventana proporcionada durante la creación de WebView.</span><span class="sxs-lookup"><span data-stu-id="a695d-175">The WebView will add a child window to the provided window during WebView creation.</span></span> <span data-ttu-id="a695d-176">El orden Z y otros elementos afectados por el orden de ventanas relacionados se verán afectados según corresponda.</span><span class="sxs-lookup"><span data-stu-id="a695d-176">Z-order and other things impacted by sibling window order will be affected accordingly.</span></span>

<span data-ttu-id="a695d-177">Se recomienda que el identificador de modelo de usuario de la aplicación conjunto de aplicaciones para el proceso o la ventana de la aplicación.</span><span class="sxs-lookup"><span data-stu-id="a695d-177">It is recommended that the application set Application User Model ID for the process or the application window.</span></span> <span data-ttu-id="a695d-178">Si no se establece ninguna, durante la creación de WebView un identificador de modelo de usuario de aplicación generado se establece en la ventana raíz de parentWindow.</span><span class="sxs-lookup"><span data-stu-id="a695d-178">If none is set, during WebView creation a generated Application User Model ID is set to root window of parentWindow.</span></span>

#### <span data-ttu-id="a695d-179">CreateCoreWebView2PointerInfo</span><span class="sxs-lookup"><span data-stu-id="a695d-179">CreateCoreWebView2PointerInfo</span></span> 

[!INCLUDE [prerelease-note](../../includes/prerelease-note.md)]

<span data-ttu-id="a695d-180">Cree un CoreWebView2PointerInfo vacío.</span><span class="sxs-lookup"><span data-stu-id="a695d-180">Create an empty CoreWebView2PointerInfo.</span></span>

> <span data-ttu-id="a695d-181">Public [CoreWebView2PointerInfo](microsoft-web-webview2-core-corewebview2pointerinfo.md) [CreateCoreWebView2PointerInfo](#createcorewebview2pointerinfo)()</span><span class="sxs-lookup"><span data-stu-id="a695d-181">public [CoreWebView2PointerInfo](microsoft-web-webview2-core-corewebview2pointerinfo.md) [CreateCoreWebView2PointerInfo](#createcorewebview2pointerinfo)()</span></span>

<span data-ttu-id="a695d-182">La CoreWebView2PointerInfo devuelta debe rellenarse con toda la información relevante antes de llamar a SendPointerInput.</span><span class="sxs-lookup"><span data-stu-id="a695d-182">The returned CoreWebView2PointerInfo needs to be populated with all of the relevant info before calling SendPointerInput.</span></span>

#### <span data-ttu-id="a695d-183">CreateWebResourceResponse</span><span class="sxs-lookup"><span data-stu-id="a695d-183">CreateWebResourceResponse</span></span> 

<span data-ttu-id="a695d-184">Crear un nuevo objeto de respuesta de recursos Web.</span><span class="sxs-lookup"><span data-stu-id="a695d-184">Create a new web resource response object.</span></span>

> <span data-ttu-id="a695d-185">Public [CoreWebView2WebResourceResponse](microsoft-web-webview2-core-corewebview2webresourceresponse.md) [CreateWebResourceResponse](#createwebresourceresponse)(contenido de Stream, int StatusCode, String ReasonPhrase, encabezados de cadena)</span><span class="sxs-lookup"><span data-stu-id="a695d-185">public [CoreWebView2WebResourceResponse](microsoft-web-webview2-core-corewebview2webresourceresponse.md) [CreateWebResourceResponse](#createwebresourceresponse)(Stream Content, int StatusCode, string ReasonPhrase, string Headers)</span></span>

<span data-ttu-id="a695d-186">La cabecera es la cadena de encabezado de respuesta sin formato delimitada por newline.</span><span class="sxs-lookup"><span data-stu-id="a695d-186">The headers is the raw response header string delimited by newline.</span></span> <span data-ttu-id="a695d-187">También es posible crear este objeto con una cadena de encabezados vacía y, a continuación, usar el CoreWebView2HttpResponseHeaders para construir los encabezados línea a línea.</span><span class="sxs-lookup"><span data-stu-id="a695d-187">It's also possible to create this object with empty headers string and then use the CoreWebView2HttpResponseHeaders to construct the headers line by line.</span></span> <span data-ttu-id="a695d-188">Para obtener información sobre otros parámetros, consulte CoreWebView2WebResourceResponse.</span><span class="sxs-lookup"><span data-stu-id="a695d-188">For information on other parameters see CoreWebView2WebResourceResponse.</span></span>

#### <span data-ttu-id="a695d-189">GetAvailableBrowserVersionString</span><span class="sxs-lookup"><span data-stu-id="a695d-189">GetAvailableBrowserVersionString</span></span> 

<span data-ttu-id="a695d-190">Obtener la información de versión del explorador.</span><span class="sxs-lookup"><span data-stu-id="a695d-190">Get the browser version information.</span></span>

> <span data-ttu-id="a695d-191">cadena estática pública [GetAvailableBrowserVersionString](#getavailablebrowserversionstring)(cadena browserExecutableFolder)</span><span class="sxs-lookup"><span data-stu-id="a695d-191">public static string [GetAvailableBrowserVersionString](#getavailablebrowserversionstring)(string browserExecutableFolder)</span></span>

<span data-ttu-id="a695d-192">También puede obtener el nombre del canal si el canal no es estable.</span><span class="sxs-lookup"><span data-stu-id="a695d-192">You also get the channel name if the channel is not a stable channel.</span></span> <span data-ttu-id="a695d-193">Si usas el tiempo de ejecución de WebView2, no se devuelve ningún nombre de canal.</span><span class="sxs-lookup"><span data-stu-id="a695d-193">If you use the WebView2 Runtime, no channel name is returned.</span></span>

##### <span data-ttu-id="a695d-194">Parameters</span><span class="sxs-lookup"><span data-stu-id="a695d-194">Parameters</span></span>
* `browserExecutableFolder` <span data-ttu-id="a695d-195">La ruta de acceso relativa a la carpeta que contiene la versión fija del motor en tiempo de ejecución de WebView2.</span><span class="sxs-lookup"><span data-stu-id="a695d-195">The relative path to the folder that contains the fixed version of the WebView2 Runtime.</span></span>

#### <span data-ttu-id="a695d-196">GetProviderForHwnd</span><span class="sxs-lookup"><span data-stu-id="a695d-196">GetProviderForHwnd</span></span> 

[!INCLUDE [prerelease-note](../../includes/prerelease-note.md)]

<span data-ttu-id="a695d-197">Devuelve el proveedor de automatización de la interfaz de usuario de la CoreWebView2CompositionController que se corresponde con el HWND dado.</span><span class="sxs-lookup"><span data-stu-id="a695d-197">Returns the UI Automation Provider for the CoreWebView2CompositionController that corresponds with the given HWND.</span></span>

> <span data-ttu-id="a695d-198">[GetProviderForHwnd](#getproviderforhwnd)de objeto público (HWND HWND)</span><span class="sxs-lookup"><span data-stu-id="a695d-198">public object [GetProviderForHwnd](#getproviderforhwnd)(IntPtr hwnd)</span></span>