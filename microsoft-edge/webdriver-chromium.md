---
description: Obtenga información sobre cómo probar su sitio web o aplicación en Microsoft Edge o automatizar el explorador con Webdriver.
title: Controlador WebDrive (cromo)
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 05/11/2020
ms.topic: article
ms.prod: microsoft-edge
ms.technology: devtools
keywords: Microsoft Edge, desarrollo web, HTML, CSS, JavaScript, desarrollador, WebDrive, Selenium, pruebas, herramientas, automatización, prueba
ms.openlocfilehash: 0cb135553b04cd0cf160755eacc0dbae245d13b7
ms.sourcegitcommit: 24430258f363b7dd85f7067afd4565bf102b4a1f
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 05/12/2020
ms.locfileid: "10645318"
---
# Controlador WebDrive (cromo)  

La API [Webdriver][W3CWebdriver] W3C es una plataforma e interfaz independiente del idioma y Protocolo de conexión que permite a los programas o las secuencias de comandos controlar el comportamiento de un explorador Web, como Microsoft Edge \ (cromo \).  

Webdriver permite a los desarrolladores crear pruebas automatizadas que simulan la interacción del usuario.  Las pruebas y simuladores de WebDrive se diferencian de las pruebas unitarias de JavaScript porque el acceso a la funcionalidad y la información que JavaScript se ejecuta en el explorador no es compatible con WebDrive, y permite simular con más precisión eventos de usuario o eventos a nivel de OS.  El controlador WebDrive es capaz de administrar las pruebas en varias ventanas, pestañas y páginas web en una sola sesión de prueba.  

A continuación se explica cómo empezar a usar Webdriver para Microsoft Edge \ (cromo \).  

## Instalar Microsoft Edge (cromo)  

Si todavía no lo ha hecho, [instale Microsoft Edge (cromo)][MicrosoftEdge].  Si estás usando una versión preinstalada de Microsoft Edge en tu equipo, verifica que dispongas de Microsoft Edge \ (cromo \) y no Microsoft Edge \ (EdgeHTML \).  Una forma rápida de comprobar es cargar `edge://settings/help` en el explorador y confirmar que el número de versión es V75 o posterior.  

## Descargar el controlador Microsoft Edge  

Webdriver requiere un controlador específico del explorador para automatizar cada explorador.  Para Microsoft Edge \ (cromo \), Webdriver requiere el [controlador Microsoft Edge][MicrosoftDeveloperEdgeToolsWebdriver] adecuado para la compilación de Microsoft Edge que desea probar o automatizar.  

Para encontrar su número de compilación correcto, siga estos pasos.  

1.  Iniciar Microsoft Edge 
1.  Ver la versión de Microsoft Edge \ (cromo \).  
    *   Ve a `edge://settings/help`  
    *   Seleccionar la `...`  >  **configuración**  >   **de Microsoft Edge**  
1.  Compruebe si la versión de WebDrive es correcta para su compilación, de modo que se ejecute correctamente.  

:::image type="complex" source="./media/webdriver-chromium/edge-version.png" alt-text="El número de compilación para Microsoft Edge Canarias el 14 de enero de 2020":::
   Figura 1.  El número de compilación para Microsoft Edge Canarias el 14 de enero de 2020  
:::image-end:::

<!--  
> ##### Figure 1  
> The build number for Microsoft Edge Canary on January 14, 2020
> ![The build number for Microsoft Edge Canary on January 14, 2020][ImageWebdriverChromiumEdgeVersion]  
-->  

Ahora, [descarga la versión coincidente del controlador de Microsoft Edge][MicrosoftDeveloperEdgeToolsWebdriverDownloads].  

:::image type="complex" source="./media/webdriver-chromium/edge-driver-install.png" alt-text="Sección de descargas de la página del controlador de Microsoft Edge":::
   Figura 2.  Sección de descargas de la página del [controlador de Microsoft Edge][MicrosoftDeveloperEdgeToolsWebdriverDownloads]  
:::image-end:::

<!--  
> ##### Figure 2
> The Downloads section of the [Microsoft Edge Driver page][MicrosoftDeveloperEdgeToolsWebdriverDownloads]
> ![The Downloads section of the Microsoft Edge Driver page][ImageWebdriverChromiumEdgeDriverInstall]  
-->  

> [!NOTE]
> Microsoft Edge \ (EdgeHTML \) no funciona con el [controlador de Microsoft Edge][MicrosoftDeveloperEdgeToolsWebdriverDownloads].  Para automatizar Microsoft Edge \ (EdgeHTML \), debe descargar [Microsoft Webdriver para Microsoft Edge \ (EdgeHTML \)][Webdriver].  

## Elegir un enlace de idioma de controlador  

El último componente que debe descargar es un controlador de cliente específico del idioma.  El enlace de idioma traduce el código que escribiste en Python, Java, C \ #, Ruby y JavaScript en comandos que el controlador de Microsoft Edge que descargaste en la [sección anterior](#download-microsoft-edge-driver) puede ejecutarse en Microsoft Edge \ (cromo \).  

[Descargue el enlace de idioma de Webdrives que prefiera][SeleniumDownloads].  El equipo de Microsoft Edge es muy recomendable [Selenium 4,00-alpha05][NugetPackagesSeleniumWebdriver400alpha05] o una versión posterior, ya que cuenta con compatibilidad integrada para Microsoft Edge \ (cromo \).  Sin embargo, puedes conducir a Microsoft Edge \ (cromo \) en todas las versiones anteriores de Selenium, incluida la versión estable actual de Selenium 3.  

> [!IMPORTANT]
> Si anteriormente estabas automatizado o probando Microsoft Edge \ (cromo \) con `ChromeDriver` y `ChromeOptions` , el código de Webdriver no se ejecuta correctamente en Microsoft Edge V80 o posterior.  Este es un cambio importante y Microsoft Edge \ (cromo \) ya no acepta estos comandos.  Debe cambiar las pruebas para usar el `EdgeOptions` controlador de clase y [Microsoft Edge][MicrosoftDeveloperEdgeToolsWebdriver].  

### Uso de Selenium 3  

[Selenium 3][|::ref1::|] es la versión estable más reciente de Selenium.  De forma predeterminada, Selenium 3 impulsa la versión anterior de Microsoft Edge \ (EdgeHTML \) y no tiene compatibilidad integrada para Microsoft Edge \ (cromo \).  Para usar Selenium 3 con Microsoft Edge \ (cromo \), instala el paquete [de herramientas de Selenium para Microsoft Edge][GithubMicrosoftEdgeSeleniumTools] .  Las Selenium Tools para Microsoft Edge extienden Selenium 3 con un controlador actualizado que te ayudará a escribir pruebas automatizadas de los exploradores Microsoft Edge \ (EdgeHTML \) y nuevos Microsoft Edge \ (cromo \).  

Selenium Tools para Microsoft Edge es una solución para desarrolladores que prefieren permanecer en Selenium 3 y los programadores que tienen pruebas de explorador existentes y desean agregar cobertura para el nuevo navegador Microsoft Edge \ (cromo \) sin cambiar las versiones de Selenium.  Las `EdgeDriver` `EdgeDriverService` clases y incluidas en las herramientas son totalmente compatibles con los equivalentes integrados en Selenium y ejecutan Microsoft Edge \ (EdgeHTML \) de forma predeterminada, por lo que las herramientas se pueden usar como un nuevo sustituto de colocación para las clases de borde existentes en Selenium.  

[Instala las herramientas de Selenium para Microsoft Edge][GithubMicrosoftEdgeSeleniumTools] para empezar a usar Microsoft Edge \ (cromo \) con tu proyecto de Selenium 3.  

## Usar Microsoft Edge (cromo) con Webdriver

Los siguientes ejemplos son ejecutables con Selenium 3 o 4.  Para usar con Selenium 3, las [herramientas de Selenium para Microsoft Edge][GithubMicrosoftEdgeSeleniumTools] deben estar instaladas.  

### Uso básico  

Para usar con Microsoft Edge \ (EdgeHTML \), simplemente cree una instancia predeterminada de la `EdgeDriver` clase.

#### [C#](#tab/c-sharp/)  

<a id="basic-usage-code" />  

```csharp
var driver = new EdgeDriver();
```  

#### [Fundación](#tab/python/)  

<a id="basic-usage-code" />  

```python
driver = Edge()
```  

* * *  

### Conduciendo Microsoft Edge (cromo)  

Para usar con Microsoft Edge \ (cromo \) en su lugar, cree una `EdgeDriver` clase nueva y pásela el `EdgeOptions` objeto con la `UseChromium` propiedad establecida en `true` .  

#### [C#](#tab/c-sharp/)  

<a id="diving-microsoft-edge-chromium-code" />  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;

var driver = new EdgeDriver(options);
```  

#### [Fundación](#tab/python/)  

<a id="diving-microsoft-edge-chromium-code" />  

```python
options = EdgeOptions()
options.use_chromium = True

driver = Edge(options)
```  

* * *  

### Elección de archivos binarios de explorador específicos (solo cromo)  

Use la `EdgeOptions` clase para elegir un binario específico.  Es útil para probar los [canales de vista previa de Microsoft Edge][MicrosoftedgeinsiderDownload] , como Microsoft Edge beta.  

#### [C#](#tab/c-sharp/)  

<a id="choosing-specific-browser-binaries-chrome-only-code" />  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;
options.BinaryLocation = @"C:\Program Files (x86)\Microsoft\Edge Beta\Application\msedge.exe";

var driver = new EdgeDriver(options);
```  

#### [Fundación](#tab/python/)  

<a id="choosing-specific-browser-binaries-chrome-only-code" />  

```python
options = EdgeOptions()
options.use_chromium = True
options.binary_location = r"C:\Program Files (x86)\Microsoft\Edge Beta\Application\msedge.exe"

driver = Edge(options)
```  

* * *  

### Personalizar el servicio del controlador Microsoft Edge  

#### [C#](#tab/c-sharp/)  

<a id="customizing-microsoft-edge-driver-services-code" />  

Cuando `EdgeDriver` se crea una instancia de clase con `EdgeOptions` Class, se crea e inicia automáticamente la `EdgeDriverService` clase correspondiente para Microsoft Edge \ (EdgeHTML \) o Microsoft Edge \ (cromo \).  

Si desea crear un `EdgeDriverService` , cree uno configurado para Microsoft Edge \ (cromo \) con el `CreateChromiumService()` método.  Es posible que le resulte útil para personalizaciones adicionales, como habilitar la salida de registro detallado en el siguiente código.  

```csharp
using (var service = EdgeDriverService.CreateChromiumService())
{
    service.UseVerboseLogging = true;

    var driver = new EdgeDriver(service);
}
```  

> [!NOTE]
> No es necesario proporcionar el `EdgeOptions` objeto cuando se pasa la `EdgeDriver` instancia de clase `EdgeDriverService` .  La `EdgeDriver` clase usa las opciones predeterminadas para Microsoft Edge \ (EdgeHTML \) o Microsoft Edge \ (cromo \) según el tipo de servicio que proporcionaste.  
> 
> Sin embargo, si desea proporcionar tanto una `EdgeDriverService` clase como una `EdgeOptions` , debe asegurarse de que ambas estén configuradas para la misma versión de Microsoft Edge.  Por ejemplo, no es posible usar una clase predeterminada de Microsoft Edge \ (EdgeHTML \) `EdgeDriverService` y propiedades de cromo en la `EdgeOptions` clase.  La `EdgeDriver` clase produce un error para evitar el uso de versiones diferentes.  

#### [Fundación](#tab/python/)  

<a id="customizing-microsoft-edge-driver-services-code" />  

Al usar Python, el `Edge` objeto crea y administra el `EdgeService` .  Para configurar el `EdgeService` , pase argumentos adicionales al `Edge` objeto:

```python
service_args = ['--verbose']
driver = Edge(service_args = service_args)
```  

* * *  

### Uso de opciones específicas de cromo  

Usar la `EdgeOptions` clase con la `UseChromium` propiedad establecida en `true` proporciona acceso a los mismos métodos y propiedades que están disponibles en la clase [ChromeOptions][SeleniumWebDriverChromeoptionsClass] en Selenium.  Por ejemplo, al igual que con otros exploradores de cromo, usa el `EdgeOptions.AddArguments()` método para ejecutar Microsoft Edge \ (cromo \) en el [modo sin encabezado][WikiHeadlessBrowser] en el siguiente código.  

#### [C#](#tab/c-sharp/)  

<a id="using-chromium-specific-options-code" />  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;
options.AddArgument("headless");
options.AddArgument("disable-gpu");
```  

#### [Fundación](#tab/python/)  

<a id="using-chromium-specific-options-code" />  

```python
options = EdgeOptions()
options.use_chromium = True
options.add_argument('headless')
options.add_argument('disable-gpu')
```  

* * *  

> [!NOTE]
> Estas [propiedades y métodos específicos de cromo][SeleniumWebDriverChromeoptionsClass] siempre están disponibles, pero no tienen efecto si la `UseChromium` propiedad no está configurada en `true` .  De forma similar, las propiedades y los métodos existentes diseñados para Microsoft Edge \ (EdgeHTML \) no tienen efecto si `UseChromium` propiedad se establece en `true` .  

<!--  
### [C#](#tab/c-sharp/)  

<a id="selenium-usage" />  

#### Basic Usage  

To use with Microsoft Edge \(EdgeHTML\), simply create a default instance of the `EdgeDriver` class.

```csharp
var driver = new EdgeDriver();
```  

#### Driving Microsoft Edge (Chromium)  

To use with Microsoft Edge \(Chromium\) instead, create a new `EdgeDriver` class and pass it the `EdgeOptions` object with the `UseChromium` property set to `true`.  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;

var driver = new EdgeDriver(options);
```  

#### Choosing Specific Browser Binaries (Chromium-Only)  

Use the `EdgeOptions` class to choose a specific binary.  It is useful for testing [Microsoft Edge preview channels][MicrosoftedgeinsiderDownload] such as Microsoft Edge Beta.  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;
options.BinaryLocation = @"C:\Program Files (x86)\Microsoft\Edge Beta\Application\msedge.exe";

var driver = new EdgeDriver(options);
```  

#### Customizing the Edge Driver Service  

When an `EdgeDriver` class instance is created using `EdgeOptions` class, it automatically creates and launches the appropriate `EdgeDriverService` class for either Microsoft Edge \(EdgeHTML\) or Microsoft Edge \(Chromium\).  

If you want to create an `EdgeDriverService`, create one configured for Microsoft Edge \(Chromium\) using the `CreateChromiumService()` method.  You may find it useful for additional customizations like enabling verbose log output in the following code.  

```csharp
using (var service = EdgeDriverService.CreateChromiumService())
{
    service.UseVerboseLogging = true;

    var driver = new EdgeDriver(service);
}
```  

> [!NOTE]
> You do not need to provide the `EdgeOptions` object when passing the `EdgeDriver` class instance the `EdgeDriverService`.  The `EdgeDriver` class uses the default options for either Microsoft Edge \(EdgeHTML\) or Microsoft Edge \(Chromium\) depending on what kind of service you provide.  
> 
> However, if you want to provide both an `EdgeDriverService` and `EdgeOptions` classes, you must ensure that both are configured for the same version of Microsoft Edge.  For example, it is not possible to use a default Microsoft Edge \(EdgeHTML\) `EdgeDriverService` class and Chromium properties in the `EdgeOptions` class.  The `EdgeDriver` class throws an error to prevent using different versions.  

#### Using Chromium-Specific Options  

Using the `EdgeOptions` class with the `UseChromium` property set to `true` gives you access to all of the same methods and properties that are available in the [ChromeOptions][SeleniumWebDriverChromeoptionsClass] class in Selenium.  For example, just like with other Chromium browsers, use the `EdgeOptions.AddArguments()` method to run Microsoft Edge \(Chromium\) in [headless mode][WikiHeadlessBrowser] in the following code.  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;
options.AddArgument("headless");
options.AddArgument("disable-gpu");
```  

> [!NOTE]
> These [Chromium-specific properties and methods][SeleniumWebDriverChromeoptionsClass] are always available but have no effect if the `UseChromium` property is not set to `true`.  Similarly, existing properties and methods meant for Microsoft Edge \(EdgeHTML\) have no effect if `UseChromium` property is set to `true`.  

### [Python](#tab/python/)  

<a id="selenium-usage" />  

#### Basic Usage  

To use with Microsoft Edge \(EdgeHTML\), simply create a default instance of the `EdgeDriver` class.

```python
driver = Edge()
```  

#### Driving Microsoft Edge (Chromium)  

To use with Microsoft Edge \(Chromium\) instead, create a new `EdgeDriver` class and pass it the `EdgeOptions` object with the `UseChromium` property set to `true`.  

```python
options = EdgeOptions()
options.use_chromium = True

driver = Edge(options)
```  

#### Choosing Specific Browser Binaries (Chromium-Only)  

Use the `EdgeOptions` class to choose a specific binary.  It is useful for testing [Microsoft Edge preview channels][MicrosoftedgeinsiderDownload] such as Microsoft Edge Beta.  

```python
options = EdgeOptions()
options.use_chromium = True
options.binary_location = r"C:\Program Files (x86)\Microsoft\Edge Beta\Application\msedge.exe"

driver = Edge(options)
```  

#### Customizing the Edge Driver Service  

When an `EdgeDriver` class instance is created using `EdgeOptions` class, it automatically creates and launches the appropriate `EdgeDriverService` class for either Microsoft Edge \(EdgeHTML\) or Microsoft Edge \(Chromium\).  

If you want to create an `EdgeDriverService`, create one configured for Microsoft Edge \(Chromium\) using the `CreateChromiumService()` method.  You may find it useful for additional customizations like enabling verbose log output in the following code.  

When using Python, the `Edge` object creates and manages the `EdgeService`.  To configure the `EdgeService`, pass additional arguments to the `Edge` object:

```python
service_args = ['--verbose']
driver = Edge(service_args = service_args)
```  

#### Using Chromium-Specific Options  

Using the `EdgeOptions` class with the `UseChromium` property set to `true` gives you access to all of the same methods and properties that are available in the [ChromeOptions][SeleniumWebDriverChromeoptionsClass] class in Selenium.  For example, just like with other Chromium browsers, use the `EdgeOptions.AddArguments()` method to run Microsoft Edge \(Chromium\) in [headless mode][WikiHeadlessBrowser] in the following code.  

```python
options = EdgeOptions()
options.use_chromium = True
options.add_argument('headless')
options.add_argument('disable-gpu')
```  

> [!NOTE]
> These [Chromium-specific properties and methods][SeleniumWebDriverChromeoptionsClass] are always available but have no effect if the `UseChromium` property is not set to `true`.  Similarly, existing properties and methods meant for Microsoft Edge \(EdgeHTML\) have no effect if `UseChromium` property is set to `true`.  

* * *  

-->  

<!--  
### Basic Usage  

To use with Microsoft Edge \(EdgeHTML\), simply create a default instance of the `EdgeDriver` class.

#### C\#  

```csharp
var driver = new EdgeDriver();
```  

#### Python  

```python
driver = Edge()
```  

### Driving Microsoft Edge (Chromium)  

To use with Microsoft Edge \(Chromium\) instead, create a new `EdgeDriver` class and pass it the `EdgeOptions` object with the `UseChromium` property set to `true`.  

#### C\#  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;

var driver = new EdgeDriver(options);
```  

#### Python  

```python
options = EdgeOptions()
options.use_chromium = True

driver = Edge(options)
```  

### Choosing Specific Browser Binaries (Chromium-Only)  

Use the `EdgeOptions` class to choose a specific binary.  It is useful for testing [Microsoft Edge preview channels][MicrosoftedgeinsiderDownload] such as Microsoft Edge Beta.  

#### C\#  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;
options.BinaryLocation = @"C:\Program Files (x86)\Microsoft\Edge Beta\Application\msedge.exe";

var driver = new EdgeDriver(options);
```  

#### Python  

```python
options = EdgeOptions()
options.use_chromium = True
options.binary_location = r"C:\Program Files (x86)\Microsoft\Edge Beta\Application\msedge.exe"

driver = Edge(options)
```  

### Customizing the Edge Driver Service  

#### C\#  

When an `EdgeDriver` class instance is created using `EdgeOptions` class, it automatically creates and launches the appropriate `EdgeDriverService` class for either Microsoft Edge \(EdgeHTML\) or Microsoft Edge \(Chromium\).  

If you want to create an `EdgeDriverService`, create one configured for Microsoft Edge \(Chromium\) using the `CreateChromiumService()` method.  You may find it useful for additional customizations like enabling verbose log output in the following code.  

```csharp
using (var service = EdgeDriverService.CreateChromiumService())
{
    service.UseVerboseLogging = true;

    var driver = new EdgeDriver(service);
}
```  

> [!NOTE]
> You do not need to provide the `EdgeOptions` object when passing the `EdgeDriver` class instance the `EdgeDriverService`.  The `EdgeDriver` class uses the default options for either Microsoft Edge \(EdgeHTML\) or Microsoft Edge \(Chromium\) depending on what kind of service you provide.  
> 
> However, if you want to provide both an `EdgeDriverService` and `EdgeOptions` classes, you must ensure that both are configured for the same version of Microsoft Edge.  For example, it is not possible to use a default Microsoft Edge \(EdgeHTML\) `EdgeDriverService` class and Chromium properties in the `EdgeOptions` class.  The `EdgeDriver` class throws an error to prevent using different versions.  

#### Python  

When using Python, the `Edge` object creates and manages the `EdgeService`.  To configure the `EdgeService`, pass additional arguments to the `Edge` object:

```python
service_args = ['--verbose']
driver = Edge(service_args = service_args)
```  

### Using Chromium-Specific Options  

Using the `EdgeOptions` class with the `UseChromium` property set to `true` gives you access to all of the same methods and properties that are available in the [ChromeOptions][SeleniumWebDriverChromeoptionsClass] class in Selenium.  For example, just like with other Chromium browsers, use the `EdgeOptions.AddArguments()` method to run Microsoft Edge \(Chromium\) in [headless mode][WikiHeadlessBrowser] in the following code.  

#### C\#  

```csharp
var options = new EdgeOptions();
options.UseChromium = true;
options.AddArgument("headless");
options.AddArgument("disable-gpu");
```  

#### Python  

```python
options = EdgeOptions()
options.use_chromium = True
options.add_argument('headless')
options.add_argument('disable-gpu')
```  

> [!NOTE]
> These [Chromium-specific properties and methods][SeleniumWebDriverChromeoptionsClass] are always available but have no effect if the `UseChromium` property is not set to `true`.  Similarly, existing properties and methods meant for Microsoft Edge \(EdgeHTML\) have no effect if `UseChromium` property is set to `true`.  
-->  

## Otras formas de configurar Webdriver  

### Chocolate  

Si usas [chocolate][Chocolatey] como el administrador de paquetes, instala el controlador Microsoft Edge ejecutando el siguiente comando.  

```console
choco install selenium-chromium-edge-driver
```  

Para obtener más información, consulta el [controlador de Selenium de cromo en chocolatey][ChocolateyPackagesSeleniumChromiumEdgeDriver].  

### Docker  

Si está usando un [acoplador][DockerHub], Descargue una imagen preconfigurada con Microsoft Edge \ (cromo \) y el [controlador Microsoft Edge][MicrosoftDeveloperEdgeToolsWebdriver] ya instalado ejecutando el siguiente comando.  

```console
docker run -d -p 9515:9515 mcr.microsoft.com/msedge/msedgedriver
```  

Para obtener más información, consulte [contenedor en el concentrador de acoplamiento][DockerHubMsedgedriver].  

## Ponerse en contacto con el equipo de Microsoft Edge DevTools    

El equipo de Microsoft Edge está ansioso por escuchar sus comentarios sobre el uso de Webdriver, Selenium y Microsoft Edge.  Use el icono de **comentarios** en las [@EdgeDevTools][TwitterTweetEdgeDevTools] de Microsoft Edge DevTools o Tweet para que el equipo sepa lo que piensa.  


:::image type="complex" source="./devtools-guide-chromium/media/devtools-feedback.png" alt-text="El icono de comentarios en el DevTools de Microsoft Edge":::
   El icono de **comentarios** en el DevTools de Microsoft Edge  
:::image-end:::

<!--  
> ##### Figure 3  
> The **Feedback** icon in the Microsoft Edge DevTools  
> ![The example.png file produced by example.js][ImageDevtoolsGuideChromiumMediaDevtoolsFeedback])  
-->  

<!-- image links -->  

<!--[ImageWebdriverChromiumEdgeVersion]: ./media/webdriver-chromium/edge-version.png "Figure 1: The build number for Microsoft Edge Canary on January 14, 2020"  -->  
<!--[ImageWebdriverChromiumEdgeDriverInstall]: ./media/webdriver-chromium/edge-driver-install.png "Figure 2: The Downloads section of the Microsoft Edge Driver page"  -->
<!--[ImageDevtoolsGuideChromiumMediaDevtoolsFeedback]: ./devtools-guide-chromium/media/devtools-feedback.png "Figure 3: The example.png file produced by example.js"  -->  

<!-- links -->  

[Webdriver]: ./webdriver.md "Webdriver (EdgeHTML) | Microsoft docs"  

[Chocolatey]: https://chocolatey.org "Chocolate | Software de chocolate"  
[ChocolateyPackagesSeleniumChromiumEdgeDriver]: https://chocolatey.org/packages/selenium-chromium-edge-driver "Controlador de borde de cromo de Selenium | Chocolate"  

[DockerHub]: https://hub.docker.com "Concentrador de acoplamiento"  
[DockerHubMsedgedriver]: https://hub.docker.com/_/microsoft-msedge-msedgedriver?tab=description "msedgedriver | Concentrador de acoplamiento"  

[GithubMicrosoftEdgeSeleniumTools]: https://github.com/microsoft/edge-selenium-tools "Microsoft/Edge-Selenium-Tools | GitHub"  
[GithubSeleniumHq]: https://github.com/SeleniumHQ/selenium "SeleniumHQ/Selenium | GitHub"  

[MicrosoftDeveloperEdgeToolsWebdriver]: https://developer.microsoft.com/microsoft-edge/tools/webdriver "Controlador WebDrive | Microsoft Developer"
[MicrosoftDeveloperEdgeToolsWebdriverDownloads]: https://developer.microsoft.com/microsoft-edge/tools/webdriver/#downloads "Descargas: Webdriver | Microsoft Developer"  

[MicrosoftEdge]: https://www.microsoft.com/edge "Descargar nuevo explorador Microsoft Edge"  

[MicrosoftedgeinsiderDownload]: https://www.microsoftedgeinsider.com/download "Descargar los canales de Insider de Microsoft Edge"  

[NugetPackagesMicrosoftEdgeSeleniumtools]: https://www.nuget.org/packages/Microsoft.Edge.SeleniumTools "Microsoft. Edge. SeleniumTools | Galería de NuGet"  
[NugetPackagesSeleniumWebdriver31410]: https://www.nuget.org/packages/Selenium.WebDriver/3.141.0 "Selenium. WebDrive 3.141.0 | Galería de NuGet"  
[NugetPackagesSeleniumWebdriver400alpha05]: https://www.nuget.org/packages/Selenium.WebDriver/4.0.0-alpha05 "Selenium. WebDrive 4.0.0-alpha05 | Galería de NuGet"  

[SeleniumHQ]: https://www.selenium.dev "SeleniumHQ"  
[SeleniumDownloads]: https://selenium.dev/downloads "Descargas | Selenium"  
[SeleniumWebDriverChromeoptionsClass]: https://www.selenium.dev/selenium/docs/api/dotnet/?topic=html/T_OpenQA_Selenium_Chrome_ChromeOptions.htm "Clase ChromeOptions: Webdriver | Selenium"  

[TwitterTweetEdgeDevTools]: https://twitter.com/intent/tweet?text=@EdgeDevTools "@EdgeDevTools | Publicar un tweet"  

[W3CWebdriver]: https://w3.org/TR/webdriver2 "Controlador WebDrive"  

[WikiHeadlessBrowser]: https://en.wikipedia.org/wiki/Headless_browser "Explorador sin periféricos | Wikipedia"