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
ms.openlocfilehash: 576f54f2a7ecc2e1e99758719e80cc589c5bc791
ms.sourcegitcommit: 8dca1c1367853e45a0a975bc89b1818adb117bd4
ms.translationtype: MT
ms.contentlocale: es-ES
ms.lasthandoff: 06/08/2020
ms.locfileid: "10699472"
---
# interfaz ICoreWebView2ExperimentalWindowFeatures 

> [!NOTE]
> Esta es una API experimental que se incluye con nuestra versión preliminar SDK versión 0.9.538.

```
interface ICoreWebView2ExperimentalWindowFeatures
  : public IUnknown
```

Características de la ventana de una ventana emergente de vista previa.

## Resumen

 Miembros                        | Descripciones
--------------------------------|---------------------------------------------
[get_Height](#get_height) | El alto de la ventana.
[get_Left](#get_left) | La posición izquierda de la ventana. Dará un error si HasPosition es falso.
[get_MenuBar](#get_menubar) | Si se muestra o no la barra de menús.
[get_ScrollBars](#get_scrollbars) | Si se muestran o no las barras de desplazamiento.
[get_Status](#get_status) | Si desea o no agregar una barra de estado.
[get_Toolbar](#get_toolbar) | Si desea que se muestre o no la barra de herramientas del explorador.
[get_Top](#get_top) | La posición superior de la ventana. Dará un error si HasPosition es falso.
[get_Width](#get_width) | Ancho de la ventana.
[HasPosition](#hasposition) | Ha especificado valores de la izquierda y de la parte superior.
[HasSize](#hassize) | Ha especificado valores de alto y ancho.

Estos campos coinciden con el ' windowFeatures ' pasado a Window. Open según lo especificado en[https://developer.mozilla.org/en-US/docs/Web/API/Window/open#Window_features](https://developer.mozilla.org/en-US/docs/Web/API/Window/open#Window_features)

## Miembros

#### get_Height 

El alto de la ventana.

> [get_Height](#get_height)de HRESULT público (UINT32 * height)

El valor mínimo es 100. Dará un error si HasSize es falso.

#### get_Left 

La posición izquierda de la ventana. Dará un error si HasPosition es falso.

> [get_Left](#get_left)de HRESULT público (UINT32 * Left)

#### get_MenuBar 

Si se muestra o no la barra de menús.

> [get_MenuBar](#get_menubar)de HRESULT público (bool * MenuBar)

#### get_ScrollBars 

Si se muestran o no las barras de desplazamiento.

> [get_ScrollBars](#get_scrollbars)de HRESULT público (bool * ScrollBars)

#### get_Status 

Si desea o no agregar una barra de estado.

> [get_Status](#get_status)de HRESULT público (bool * status)

#### get_Toolbar 

Si desea que se muestre o no la barra de herramientas del explorador.

> [get_Toolbar](#get_toolbar)de HRESULT público (una barra de herramientas de bool *)

#### get_Top 

La posición superior de la ventana. Dará un error si HasPosition es falso.

> [get_Top](#get_top)de HRESULT público (UINT32 * Top)

#### get_Width 

Ancho de la ventana.

> [get_Width](#get_width)de HRESULT público (UINT32 * width)

El valor mínimo es 100. Dará un error si HasSize es falso.

#### HasPosition 

Ha especificado valores de la izquierda y de la parte superior.

> [HASPOSITION](#hasposition)HRESULT público (bool * HasPosition)

#### HasSize 

Ha especificado valores de alto y ancho.

> [HASSIZE](#hassize)HRESULT público (bool * HasSize)
