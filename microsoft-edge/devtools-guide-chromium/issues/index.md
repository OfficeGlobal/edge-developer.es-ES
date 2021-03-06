---
description: Use la herramienta problemas para encontrar y corregir problemas con el sitio Web.
title: Buscar y solucionar problemas con la herramienta problemas de Microsoft Edge DevTools
author: MSEdgeTeam
ms.author: msedgedevrel
ms.date: 10/19/2020
ms.topic: article
ms.prod: microsoft-edge
keywords: Microsoft Edge, desarrollo web, herramientas F12, DevTools
ms.openlocfilehash: 4691db9542ecff93d1b59e243844109e0c730d23
ms.sourcegitcommit: 99eee78698dc95b2a3fa638a5b063ef449899cda
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 10/20/2020
ms.locfileid: "11124729"
---
<!-- Copyright Sam Dutton 

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       https://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.  -->  

# Buscar y solucionar problemas con la herramienta problemas de Microsoft Edge DevTools  

La herramienta **problemas** de Microsoft Edge DevTools reduce la fatiga de las notificaciones y el desorden de la **consola**.  Utilícelo para buscar soluciones a problemas detectados por el explorador, como problemas de cookies y contenido mixto.  

> [!NOTE]
> En Microsoft Edge 84, la herramienta **problemas** admite tres tipos de problemas:  
> *   [Problemas de cookies][MDNSameSiteCookies]  
> *   [Contenido mixto][MDNMixedContent]  
> *   [Problemas de COEP][W3CCOEPSpec]
> 
> El equipo de Microsoft Edge DevTools planea admitir más tipos de problemas en futuras versiones de Microsoft Edge.  

## Abrir la herramienta problemas en el cajón de DevTools  

1.  Visite una página, como [SameSite-Sandbox.Glitch.me][GlitchSamesiteSandbox], que contiene problemas para corregir.  
1.  [Abra DevTools][DevtoolsOpen].  
1.  :::row:::
       :::column span="":::
          Seleccione el botón **ir a problemas** de la barra de advertencia amarilla.  
          
          :::image type="complex" source="../media/issues-open-issues-tab.msft.png" alt-text="Botón ir a problemas de la barra de advertencia amarilla cuando se detectan problemas" lightbox="../media/issues-open-issues-tab.msft.png":::
             El botón **ir a problemas** de la barra de advertencia amarilla cuando se detectan problemas.  
          :::image-end:::  
       :::column-end:::
       :::column span="":::
          También puede elegir **problemas** en el menú **más herramientas** .  
          
          :::image type="complex" source="../media//issues-more-tools-menu.msft.png" alt-text="Botón ir a problemas de la barra de advertencia amarilla cuando se detectan problemas" lightbox="../media//issues-more-tools-menu.msft.png":::
             Herramienta **problemas** en el menú **más herramientas**  
          :::image-end:::  
       :::column-end:::
    :::row-end:::
    
1.  Seleccione el botón **volver a cargar la página** , si es necesario.  
    
    :::image type="complex" source="../media/issues-tab-before-refresh.msft.png" alt-text="Botón ir a problemas de la barra de advertencia amarilla cuando se detectan problemas" lightbox="../media/issues-tab-before-refresh.msft.png":::
       Herramienta **problemas** del cajón de DevTools con el botón **volver a cargar página**  
    :::image-end:::  

    Los problemas notificados en la **consola** son difíciles de comprender, como las advertencias de cookie en la siguiente imagen.  En función de los problemas que se hayan informado, es posible que no tenga claro lo que debe hacer.  
    
    :::image type="complex" source="../media/issues-tab-after-refresh.msft.png" alt-text="Botón ir a problemas de la barra de advertencia amarilla cuando se detectan problemas" lightbox="../media/issues-tab-after-refresh.msft.png":::
       Herramienta **problemas** en el cajón de DevTools con tres problemas de cookies  
    :::image-end:::  
    
## Ver los elementos de la herramienta problemas  

La herramienta **problemas** del alimentador de DevTools presenta advertencias en una forma estructurada, agregada y que se ejecuta correctamente.  

1.  Seleccione un elemento de la herramienta **problemas** para obtener información sobre cómo corregir el problema y encontrar los recursos afectados.  
    
    :::image type="complex" source="../media/issues-tab-issue-open.msft.png" alt-text="Botón ir a problemas de la barra de advertencia amarilla cuando se detectan problemas" lightbox="../media/issues-tab-issue-open.msft.png":::
       **Marcar las cookies entre sitios como** un problema seguro abierto en la herramienta **problemas**  
    :::image-end:::  
    
    Cada elemento tiene cuatro componentes:  
    
    *   Un titular que describe el problema.  
    *   Descripción que proporciona el contexto y la solución.  
    *   Una sección de **recursos afectados** con vínculos a recursos dentro del contexto de DevTools adecuado, como el panel red.  
    *   Vínculos a más instrucciones.  
    
1.  Seleccione los elementos de **recursos afectados** para ver los detalles.  En el siguiente ejemplo, la **marca de las cookies entre sitios como** un problema seguro afecta a una cookie y a dos solicitudes.  
    
    :::image type="complex" source="../media/issues-tab-affected-resources.msft.png" alt-text="Botón ir a problemas de la barra de advertencia amarilla cuando se detectan problemas" lightbox="../media/issues-tab-affected-resources.msft.png":::
       Recursos afectados abiertos en la herramienta **problemas** del cajón de DevTools  
    :::image-end:::  
    
## Ver problemas en contexto  

1.  Seleccione un vínculo de recursos para ver el elemento en el contexto adecuado dentro de DevTools.  En el ejemplo siguiente, seleccione `samesite-sandbox.glitch.me` en **solicitudes** para mostrar las cookies adjuntas a la solicitud.  
    
    :::image type="complex" source="../media/issues-tab-view-request.msft.png" alt-text="Botón ir a problemas de la barra de advertencia amarilla cuando se detectan problemas" lightbox="../media/issues-tab-view-request.msft.png":::
       Ver la cookie afectada en el panel de **red** DevTools  
    :::image-end:::  

1.  Desplácese para ver el elemento con un problema: en el ejemplo siguiente, la `ck02` cookie.  Desplace el puntero sobre la columna **SameSite** para ver el `None` valor detectado por el problema.  
    
    :::image type="complex" source="../media/issues-tab-view-issue.msft.png" alt-text="Botón ir a problemas de la barra de advertencia amarilla cuando se detectan problemas" lightbox="../media/issues-tab-view-issue.msft.png":::
       `None` valor de la columna **SameSite** de la `ck02` cookie en el panel de **red** DevTools  
    :::image-end:::  

## Contactar al equipo de Microsoft Edge DevTools  

[!INCLUDE [contact DevTools team note](../includes/contact-devtools-team-note.md)]  

<!-- links -->  

[DevtoolsOpen]: ../open.md "Abrir Microsoft Edge DevTools | Microsoft docs"  

[GlitchSamesiteSandbox]: https://samesite-sandbox.glitch.me "Pruebas de cookie SameSite | Intento"  

[MDNSameSiteCookies]: https://developer.mozilla.org/docs/Web/HTTP/Headers/Set-Cookie/SameSite "SameSite cookies | MDN"  
[MDNMixedContent]: https://developer.mozilla.org/docs/Web/Security/Mixed_content "Contenido mixto | MDN"  

[W3CCOEPSpec]: https://wicg.github.io/cross-origin-embedder-policy "Directiva de Embedder entre orígenes | Grupo de comunidades de la web"  

> [!NOTE]
> Algunas partes de esta página son modificaciones basadas en el trabajo creado y [compartido por Google][GoogleSitePolicies] y se usan según las condiciones descritas en la [licencia internacional de Creative Commons Atribution 4,0][CCA4IL].  
> La página original se encuentra [aquí](https://developers.google.com/web/tools/chrome-devtools/issues/index) y está creada por [Sam Dutton][SamDutton] \ (Defensor del desarrollador \).  
[![Licencia de Creative Commons][CCby4Image]][CCA4IL]  
Este trabajo dispone de licencia conforme a [Licencia internacional de Creative Commons Attribution 4.0][CCA4IL].  

[CCA4IL]: https://creativecommons.org/licenses/by/4.0  
[CCby4Image]: https://i.creativecommons.org/l/by/4.0/88x31.png  
[GoogleSitePolicies]: https://developers.google.com/terms/site-policies  
[KayceBasques]: https://developers.google.com/web/resources/contributors/kaycebasques  
[SamDutton]: https://developers.google.com/web/resources/contributors/samdutton  
