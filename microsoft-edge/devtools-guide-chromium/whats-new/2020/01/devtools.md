---
description: Vista 3D, integración de Visual Studio con Microsoft Edge y mucho más.
title: Novedades de DevTools (Microsoft Edge 81)
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 09/11/2020
ms.topic: article
ms.prod: microsoft-edge
keywords: Microsoft Edge, desarrollo web, herramientas F12, DevTools
ms.openlocfilehash: 3081ebb256a9ede637aaaddc3c3cdf7a70a201bb
ms.sourcegitcommit: b337717957529239434b4e8e1e167aebf0543518
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 09/15/2020
ms.locfileid: "11015478"
---
<!-- Copyright Kayce Basques 

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       https://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.  -->  

# Novedades de DevTools (Microsoft Edge 81)  

## Anuncios del equipo de Microsoft Edge DevTools  

Las siguientes secciones son una lista de anuncios que puede haber perdido del equipo de DevTools de Microsoft Edge. Compruébelos para probar nuevas características en DevTools, Visual Studio Code Extensions y mucho más.  Para mantenerte al tanto de las últimas y mejores características de las herramientas para desarrolladores, descarga los [canales de Microsoft Edge Preview][MicrosoftEdgePreviewChannels] y mantente [en Twitter][EdgeDevToolsTwitterAccount].  

### Mejoras de accesibilidad para el DevTools  

El equipo de DevTools ha contribuido a 170 cambios en cromo para solucionar problemas de alto impacto en el contraste de color, el teclado y el lector de pantalla en el DevTools.  Cada desarrollador que crea la web debe poder usar el DevTools.  

:::image type="complex" source="../../images/2020/01/a11y-performance-tool.msft.gif" alt-text="La herramienta de rendimiento en el DevTools con la navegación con el teclado y las mejoras del lector de pantalla" lightbox="../../images/2020/01/a11y-performance-tool.msft.gif":::
   La herramienta de **rendimiento** en el DevTools con la navegación con el teclado y las mejoras del lector de pantalla  
:::image-end:::  

¿Desea saber cómo hacer que su página web sea accesible para todos los usuarios?  Descargue [Insight Insights][AccessibilityInsights] y extensiones [Webhint][WebhintBrowserExtension] para Microsoft Edge para comenzar.  

Si usa lectores de pantalla o el teclado para desplazarse por la DevTools, envíenos sus comentarios con un [Tweet][PostTweetEdgeDevTools] o haga clic en el icono para [Enviar comentarios](#getting-in-touch-with-microsoft-edge-devtools-team) .  

[#963183][CR963183] de problemas de cromo  

### Usar el DevTools en otros idiomas  

Muchos programadores usan otras herramientas de desarrollo, como StackOverflow y Visual Studio, en su idioma nativo, no solo en inglés.  Nos complace anunciar la localización de la DevTools, que ahora puedes usar en uno de los 10 idiomas además del inglés:  

:::row:::
   :::column span="":::
      Chino \ (simplificado \)- &#20013;&#25991;&#65288;&#31616;&#20307;&#65289;
   :::column-end:::
   :::column span="":::
      Chino (tradicional \)- &#20013;&#25991;&#65288;&#32321;&#39636;&#65289;
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
      Francés: Francisco&#231;AIS
   :::column-end:::
   :::column span="":::
      Alemán-Deutsch
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
      Italiano-Italiano
   :::column-end:::
   :::column span="":::
       &#26085;&#26412;&#35486; japonés
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
      Coreano:  &#54620;&#44397;&#50612;
   :::column-end:::
   :::column span="":::
      Portugués-Portugu&#234;s
   :::column-end:::
:::row-end:::
:::row:::
   :::column span="":::
      Ruso:  &#1088;&#1091;&#1089;&#1089;&#1082;&#1080;&#1081;
   :::column-end:::
   :::column span="":::
      Español-Espa&#241;ol
   :::column-end:::
:::row-end:::

<!--  
|  |  |  
|:--- |:--- |  
| Chinese (Simplified) - 中文(简体)（简体）| Chinese (Traditional) - 中文(繁體)（繁體）|  
| French – français | German - deutsch |  
| Italian - italiano | Portuguese - português |  
| Korean - 한국어 | Japanese - 日本語 |  
| Russian – русский | Spanish - español |  
-->  

El DevTools coincide automáticamente con el idioma que usas para Microsoft Edge en `edge://settings/languages` .  

Si desea que Microsoft Edge esté en un idioma y que su DevTools permanezca en inglés, presione `F1` la DevTools para abrir la [configuración][Settings] y deshabilitar el **idioma del explorador**.  

:::image type="complex" source="../../images/2020/01/localized-devtools.msft.png" alt-text="El DevTools en alemán" lightbox="../../images/2020/01/localized-devtools.msft.png":::
   El DevTools en alemán  
:::image-end:::  

Los mensajes de **consola** no se localizan.  Solo las cadenas usadas en la interfaz de usuario de DevTools se muestran en el idioma que usas para Microsoft Edge.  

Si desea usar la DevTools en un idioma diferente al de los que están disponibles, [Tweet][PostTweetEdgeDevTools] o haga clic en el icono para [Enviar comentarios](#getting-in-touch-with-microsoft-edge-devtools-team) .  

[#941561][CR941561] de problemas de cromo  

### extensión webhint de Microsoft Edge  

La extensión webhint de Microsoft Edge te permite examinar fácilmente tu página web y obtener comentarios sobre la accesibilidad, la compatibilidad de explorador, la seguridad, el rendimiento y mucho más dentro de la DevTools.  Para obtener más información, consulte [https://webhint.io][Webhint] .  

:::image type="complex" source="../../images/2020/01/webhint-browser-extension.msft.png" alt-text="La pestaña sugerencias de la DevTools cuando está instalada la extensión de explorador webhint" lightbox="../../images/2020/01/webhint-browser-extension.msft.png":::
   La pestaña **sugerencias** de la DevTools cuando está instalada la extensión de explorador webhint  
:::image-end:::  

[Prueba la extensión de explorador webhint en Microsoft Edge][MicrosoftEdgeInsiderAddons].  Una vez que haya instalado la extensión, abra el DevTools y seleccione la pestaña sugerencias.  Desde aquí, ejecute un examen de sitios personalizable.  Visita [webhint.IO][WebhintBrowserExtension] para obtener más información.  

### Vista 3D  

Use la **vista 3D** para depurar la aplicación web desplazándose por el [modelo de objeto de documento \ (Dom \)][MDNDocumentObjectModel] o el contexto de apilamiento [de índice z][MDNZIndex] .  

:::image type="complex" source="../../images/2020/01/3dview.msft.png" alt-text="Vista 3D en el DevTools" lightbox="../../images/2020/01/3dview.msft.png":::
   Vista 3D en el DevTools  
:::image-end:::  

Para acceder a la vista 3D, pulse `Ctrl`  +  `Shift`  +  `P` , escriba en la **vista 3D** y seleccione **Mostrar vista en 3D**.  

Trabajamos en la interfaz de usuario y agregamos más funcionalidad a la vista 3D; por lo tanto, envíanos tus [comentarios](#getting-in-touch-with-microsoft-edge-devtools-team).  

[#987787][CR987787] de problemas de cromo  

### Extensiones de código de Visual Studio  

El equipo de DevTools también ha publicado algunas extensiones para [código Visual Studio][VisualStudioCode] que te permiten usar la potencia de DevTools directamente desde tu editor de texto. Consulta las siguientes extensiones:  

#### Elementos de Microsoft Edge  

Use la herramienta elementos de Visual Studio para agregar los elementos de la extensión de código de Visual Studio [Microsoft Edge \ (cromo \)][VisualStudioMarketplaceElementsMicrosoftEdgeChromiumExtension] .  

:::image type="complex" source="../../images/2020/01/elements-for-edge.msft.png" alt-text="La herramienta elementos en Visual Studio código que usa los elementos de la extensión de Microsoft Edge" lightbox="../../images/2020/01/elements-for-edge.msft.png":::
   La herramienta **elementos** en Visual Studio código que usa los elementos de la extensión de Microsoft Edge  
:::image-end:::  

Para obtener más información, consulta [los elementos de la extensión de código de Microsoft Edge Visual Studio][VisualStudioCodeElementEdgeExtension].  

#### Depurador para Microsoft Edge  

Con el [depurador de la extensión de código de Microsoft Edge][VisualStudioMarketplaceDebuggerEdge] Visual Studio, depura JavaScript ejecutándose directamente en Microsoft Edge desde el código de Visual Studio.  

:::image type="complex" source="../../images/2020/01/vscode-debugger.msft.png" alt-text="El depurador para la extensión de Microsoft Edge en Visual Studio Code" lightbox="../../images/2020/01/vscode-debugger.msft.png":::
   El depurador para la extensión de Microsoft Edge en Visual Studio Code  
:::image-end:::  

Para obtener más información, consulte [Cómo depurar Microsoft Edge desde código de Visual Studio][VisualStudioCodeDebuggerEdgeExtension].  

#### webhint  

La extensión de código [webhint][VisualStudioMarketplaceWebhintExtension] de Visual Studio usa `webhint` para mejorar la página web mientras estás escribiendo. Esta extensión ejecuta y notifica diagnósticos en los archivos de área de trabajo según el `webhint` análisis.  

:::image type="complex" source="../../images/2020/01/webhint-vscode-extension.msft.png" alt-text="Extensión de código webhint de Visual Studio que analiza un archivo. TSX en código de Visual Studio" lightbox="../../images/2020/01/webhint-vscode-extension.msft.png":::
   Extensión de código webhint de Visual Studio que analiza un `.tsx` archivo en código Visual Studio  
:::image-end:::  

[Más información sobre la extensión webhint de Visual Studio Code][WebhintVisualStudioCodeExtension].  

### Integración con Visual Studio  

En Visual Studio 2019 versión 16,2 o posterior, usa el depurador de Visual Studio para depurar JavaScript que se ejecuta en Microsoft Edge.  [Descarga Visual Studio 2019][MicrosoftVisualStudioDownloads] para probar esta característica.  

:::image type="complex" source="../../images/2020/01/vs.msft.png" alt-text="Visual Studio con la opción de iniciar la aplicación web en Microsoft Edge Canarias, dev o beta" lightbox="../../images/2020/01/vs.msft.png":::
   Visual Studio con la opción de iniciar la aplicación web en Microsoft Edge Canarias, dev o beta  
:::image-end:::  

[Obtenga más información sobre la depuración de Microsoft Edge desde Visual Studio][MicrosoftVisualStudio].  

### Mensajes de la consola de prevención de seguimiento  

La prevención de seguimiento es una característica exclusiva de Microsoft Edge que le protege de ser rastreada por los sitios web que no ha visitado antes.  La configuración predeterminada de prevención de rastreo es el modo equilibrado, que bloquea los rastreadores de terceros y los rastreadores maliciosos conocidos para obtener una experiencia que equilibre la compatibilidad de la privacidad y la Web.  Para obtener más información sobre la compatibilidad de su página web cuando se bloquean determinados rastreadores, también hemos añadido mensajes de advertencia en la consola cuando se bloquea un rastreador.  

:::image type="complex" source="../../images/2020/01/tracking-prevention.msft.png" alt-text="Mensajes en la consola cuando el seguimiento de prevención bloquea el acceso al almacenamiento de un rastreador" lightbox="../../images/2020/01/tracking-prevention.msft.png":::
   Mensajes en la consola cuando el seguimiento de prevención bloquea el acceso al almacenamiento de un rastreador  
:::image-end:::  

[Obtenga más información acerca de la prevención de seguimiento y el equilibrio entre privacidad y compatibilidad web][TrackingPrevention].  

## Anuncios del proyecto de cromo  

En las siguientes secciones se anuncian características adicionales disponibles en Microsoft Edge 81 que se han contribuido al proyecto de código abierto.  

### Compatibilidad de moto G4 en el modo de dispositivo  

Después de [Habilitar la barra de herramientas del dispositivo][DeviceToolbar], simule las dimensiones de una ventanilla de moto G4 en la lista de **dispositivos** .  

:::image type="complex" source="../../images/2020/01/motog4.msft.png" alt-text="Simulación de una ventanilla de moto G4" lightbox="../../images/2020/01/motog4.msft.png":::
   Simulación de una ventanilla de moto G4  
:::image-end:::  

Haga clic en [Mostrar marco del dispositivo][DeviceFrame] para mostrar el hardware de moto G4 en la ventanilla.  

:::image type="complex" source="../../images/2020/01/motog4frame.msft.png" alt-text="Mostrar el hardware de moto G4" lightbox="../../images/2020/01/motog4frame.msft.png":::
   Mostrar el hardware de moto G4  
:::image-end:::  

Características relacionadas:  

*   Abra el [menú de comandos][CommandMenu] y ejecute el `Capture screenshot` comando para tomar una captura de pantalla de la ventanilla que incluye el hardware moto G4 (después de habilitar **Mostrar marco de dispositivo**).  
*   [Limite la red y la CPU][ThrottleNetworkAndCpu] para simular de forma más precisa las condiciones de navegación web de un usuario móvil.  

[#924693][CR924693] de problemas de cromo  

### Actualizaciones relacionadas con cookies  

#### Cookies bloqueados en el panel cookies  

El panel cookies en el panel de la aplicación ahora muestra las cookies bloqueadas con un fondo amarillo.  

:::image type="complex" source="../../images/2020/01/blockedcookies.msft.png" alt-text="Cookies bloqueados en el panel de cookies del panel de aplicaciones" lightbox="../../images/2020/01/blockedcookies.msft.png":::
   Cookies bloqueados en el panel de cookies del panel de aplicaciones  
:::image-end:::  

[#1030258][CR1030258] de problemas de cromo  <!-- inaccessible  -->  

#### Prioridad de la cookie en el panel de cookies  

Las tablas de cookies de los paneles red y aplicación ahora incluyen una columna de **prioridad** .  

> [!CAUTION]
> Los exploradores basados en cromo, como Microsoft Edge, son los únicos exploradores que admiten la prioridad de las cookies.  

[#1026879][CR1026879] de problemas de cromo  

#### Editar todos los valores de cookies  

Ahora todas las celdas de las tablas de cookies se pueden editar, excepto las celdas de la columna **tamaño** , porque esa columna representa el tamaño de red de la cookie, en bytes.  Vea [los campos][CookiesFields] para obtener una explicación de cada columna.  

:::image type="complex" source="../../images/2020/01/editcookie.msft.png" alt-text="Editar un valor de cookie" lightbox="../../images/2020/01/editcookie.msft.png":::
   Editar un valor de cookie  
:::image-end:::  

#### Copiar como Node.js fetch para incluir datos de cookies  

Haga clic con el botón secundario en una solicitud de red y seleccione **copiar**  >  **copia como Node.js fetch** para obtener una `fetch` expresión que incluya datos de cookies.  

:::image type="complex" source="../../images/2020/01/fetchcookies.msft.png" alt-text="Copiar como captura de Node.js" lightbox="../../images/2020/01/fetchcookies.msft.png":::
   Copiar como captura de Node.js  
:::image-end:::  

[#1029826][CR1029826] de problemas de cromo  

### Iconos más exactos del manifiesto de la aplicación Web  

Anteriormente, el panel manifiesto del panel de aplicaciones enviaba sus propias solicitudes para mostrar los iconos del manifiesto de la aplicación Web.  DevTools ahora muestra el mismo icono de manifiesto que usa Microsoft Edge.  

:::image type="complex" source="../../images/2020/01/manifesticons.msft.png" alt-text="Iconos en el panel manifiesto" lightbox="../../images/2020/01/manifesticons.msft.png":::
   Iconos en el panel manifiesto  
:::image-end:::  

[#985402][CR985402] de problemas de cromo  

### Mantenga el mouse sobre las propiedades de contenido CSS para ver valores sin escape  

Desplace el puntero sobre el valor de una `content` propiedad para ver la versión sin escape del valor.  

Por ejemplo, en esta [demostración][CSSContentDemo] , cuando Inspeccione el `p::after` seudoelemento, verá una cadena de escape en el panel Estilos:  

:::image type="complex" source="../../images/2020/01/escapedstring.msft.png" alt-text="La cadena de escape" lightbox="../../images/2020/01/escapedstring.msft.png":::
   La cadena de escape  
:::image-end:::  

Cuando pasa el puntero sobre el `content` valor, Ve el valor unescape:  

:::image type="complex" source="../../images/2020/01/unescapedstring.msft.png" alt-text="Valor sin escape" lightbox="../../images/2020/01/unescapedstring.msft.png":::
   Valor sin escape  
:::image-end:::  

### Errores de mapas de origen más detallados en la consola  

La consola ahora proporciona más información sobre por qué no se pudo cargar o analizar un mapa de origen.  Anteriormente, se ha proporcionado un error sin explicar qué falló.  

:::image type="complex" source="../../images/2020/01/sourcemap.msft.png" alt-text="Un error de carga del mapa de origen en la consola" lightbox="../../images/2020/01/sourcemap.msft.png":::
   Un error de carga del mapa de origen en la consola  
:::image-end:::  

### Configuración para deshabilitar el desplazamiento más allá del final de un archivo  

Abrir [configuración][Settings] y deshabilitar **preferencias**  >  **orígenes**:  >  **permite desplazarse más allá del final del archivo** para deshabilitar el comportamiento predeterminado de la interfaz de usuario que permite desplazarse hasta el final de un archivo en el panel **fuentes** .  

:::image type="complex" source="../../images/2020/01/settings.msft.png" alt-text="Deshabilitar la opción permitir el desplazamiento más allá del final del archivo" lightbox="../../images/2020/01/settings.msft.png":::
   Deshabilitar la **opción permitir el desplazamiento más allá del final del archivo** en configuración  
:::image-end:::  

:::image type="complex" source="../../images/2020/01/scrollingsources.msft.png" alt-text="El desplazamiento más allá del final de un archivo ya está deshabilitado en el panel orígenes" lightbox="../../images/2020/01/scrollingsources.msft.png":::
   El desplazamiento más allá del final de un archivo ya está deshabilitado en el panel orígenes  
:::image-end:::  

## Descargar los canales de Microsoft Edge Preview  

Si está en Windows o macOS, considere la posibilidad de usar los [canales de Microsoft Edge Preview][MicrosoftEdgePreviewChannels] como su explorador de desarrollo predeterminado.  Los canales de previsualización proporcionan acceso a las características más recientes de DevTools.  

## Ponerse en contacto con el equipo de Microsoft Edge DevTools  

[!INCLUDE [contact DevTools team note](../../includes/contact-whats-new-note.md)]  

<!-- links -->  

[DeviceToolbar]: /microsoft-edge/devtools-guide-chromium/device-mode/index#simulate-a-mobile-viewport "Simular un área de visualización móvil: simular dispositivos móviles con el modo de dispositivo en Microsoft Edge DevTools | Microsoft docs"
[DeviceFrame]: /microsoft-edge/devtools-guide-chromium/device-mode/index#show-device-frame "Mostrar fotograma de dispositivo: simular dispositivos móviles con el modo de dispositivo en Microsoft Edge DevTools | Microsoft docs"
[CommandMenu]: /microsoft-edge/devtools-guide-chromium/command-menu/index "Ejecutar comandos con el menú de comandos de Microsoft Edge DevTools | Microsoft docs"  
[ThrottleNetworkAndCpu]: /microsoft-edge/devtools-guide-chromium/device-mode/index#throttle-the-network-and-cpu "Limitar la red y la CPU: simular dispositivos móviles con el modo de dispositivo en Microsoft Edge DevTools | Microsoft docs"
[Settings]: /microsoft-edge/devtools-guide-chromium/customize/index#settings "Configuración-personalizar Microsoft Edge DevTools | Microsoft docs"
[MicrosoftVisualStudio]: /microsoft-edge/visual-studio/index "Visual Studio | Microsoft docs"  
[CookiesFields]: /microsoft-edge/devtools-guide-chromium/storage/cookies#fields "Campos: ver, editar y eliminar cookies con Microsoft Edge DevTools | Microsoft docs"  

[VisualStudioCodeDebuggerEdgeExtension]: /microsoft-edge/visual-studio-code/debugger-for-edge "Depurador para la extensión de código de Microsoft Edge Visual Studio"  
[VisualStudioCodeElementEdgeExtension]: /microsoft-edge/visual-studio-code/elements-for-edge "Elementos de la extensión de código de Microsoft Edge Visual Studio"  

[MicrosoftEdgePreviewChannels]: https://aka.ms/microsoftedge "Canales de Microsoft Edge Preview"  

[VisualStudioCode]: https://aka.ms/vscode "Código de Visual Studio"  
[VisualStudioMarketplaceDebuggerEdge]: https://aka.ms/debugger4code "Depurador para Microsoft Edge-Marketplace de Visual Studio"  
[VisualStudioMarketplaceElementsMicrosoftEdgeChromiumExtension]: https://aka.ms/elements4code "Elementos de Microsoft Edge \ (cromo \)-Visual Studio Marketplace"  
[VisualStudioMarketplaceWebhintExtension]: https://aka.ms/webhint4code "webhint-catálogo de soluciones de Visual Studio"

[TrackingPrevention]: https://aka.ms/microsoftedge/tracking-prevention-blog "Mejorar la prevención de seguimiento en la entrada de blog de Microsoft Edge"

[MicrosoftEdgeInsiderAddons]: https://aka.ms/webhint/edge-extension "Complementos de Insider de Microsoft Edge"  
[MicrosoftVisualStudioDownloads]: https://aka.ms/vs/download "Descargar Visual Studio 2019 para Windows & Mac"  

[PostTweetEdgeDevTools]: https://aka.ms/tweet/edgedevtools "@EdgeDevTools | Publicar un tweet"  

[CR924693]: https://crbug.com/924693 "Solicitud de característica: agregar moto G4 a la lista de modos de dispositivo | Errores de cromo"  
[CR1030258]: https://crbug.com/1030258 "CR 1030258 | Errores de cromo"  
[CR1026879]: https://crbug.com/1026879 "La pestaña cookie en la consola de desarrollo ya no muestra la prioridad | Errores de cromo"  
[CR1029826]: https://crbug.com/1029826 "ficha red: > clic con el botón secundario para solicitar > copiar-> copia como fetch no copia cookies | Errores de cromo"  
[CR985402]: https://crbug.com/985402 "las cadenas de error del manifiesto de la aplicación web son confusas | Errores de cromo"  
[CR963183]: https://crbug.com/963183 "DevTools no son compatibles con WCAG | Errores de cromo"  
[CR941561]: https://crbug.com/941561 "Localizabilidad de la DevTools | Errores de cromo"  
[CR987787]: https://crbug.com/987787 "Vista 3D de Dom | Errores de cromo"  

[CSSContentDemo]: https://mathiasbynens.github.io/css-dbg-stories/css-escapes.html "Demostración de contenido CSS sin escape"  

[GitHubMicrosoftDocsEdgeDeveloperNewIssue]: https://aka.ms/edgedevtoolsdocs/feedback "Nuevo problema: MicrosoftDocs/Edge-Developer"  

[TheWebWeWant]: https://aka.ms/webwewant "La web que queremos"  
[AccessibilityInsights]: https://aka.ms/a11yinsights "Información de accesibilidad"  
[MDNDocumentObjectModel]: https://developer.mozilla.org/docs/Web/API/Document_Object_Model "Modelo de objetos de documento (DOM) | MDN"  
[MDNZIndex]: https://developer.mozilla.org/docs/Web/CSS/z-index "índice z | MDN"  
[EdgeDevToolsTwitterAccount]: https://aka.ms/twitter/edgedevtools "@EdgeDevTools cuenta de Twitter"  

[Webhint]: https://aka.ms/webhint "sugerencia"  

[WebhintBrowserExtension]: https://aka.ms/webhint/browser-extension "Extensión de explorador webhint | documentación de webhint"  
[WebhintVisualStudioCodeExtension]: https://aka.ms/webhint/code-extension "Extensión de código webhint de Visual Studio | documentación de webhint"  

> [!NOTE]
> Algunas partes de esta página son modificaciones basadas en el trabajo creado y [compartido por Google][GoogleSitePolicies] y se usan según las condiciones descritas en la [licencia internacional de Creative Commons Atribution 4,0][CCA4IL].  
> La página original se encuentra [aquí](https://developers.google.com/web/updates/2020/01/devtools/index) y está modificada por [Kayce vascos][KayceBasques] \ (redactor técnico, Chrome DevTools \ & Lighthouse \).  

[![Licencia de Creative Commons][CCby4Image]][CCA4IL]  
Este trabajo dispone de licencia conforme a [Licencia internacional de Creative Commons Attribution 4.0][CCA4IL].  

[CCA4IL]: https://creativecommons.org/licenses/by/4.0  
[CCby4Image]: https://i.creativecommons.org/l/by/4.0/88x31.png  
[GoogleSitePolicies]: https://developers.google.com/terms/site-policies  
[KayceBasques]: https://developers.google.com/web/resources/contributors/kaycebasques  