---
title: OS and Web Browser Support
page_title: OS Web Browser Support
description: "Get started with Telerik UI for ASP.NET MVC and learn which are the operating systems and browsers supported by the framework components."
previous_url: /getting-started/prerequisites/browser-support, /getting-started/prerequisites/os-support
slug: webbrowsersupport_aspnetmvc
position: 1
---

# Operating System and Web Browser Support

The [Telerik UI for ASP.NET MVC helpers and framework components](https://demos.telerik.com/aspnet-mvc/) are designed to support all major operating systems and browsers. They also support hybrid mouse and touch-screen devices.

## Supported Operating Systems

The following table lists the supported operating systems.

| PLATFORM          | VERSION               |
| :---------------- | :-------------------- |
| Windows           | XP or later           |
| Windows Server    | Server 2003 or later  |
| OS X              | 10.5 or later         |
| Android           | 2.3 or later          |
| iOS               | 6.0 or later          |
| Windows Phone     | 8.0 or later          |

## Supported Developer Environments

* [.NET Framework v3.5](https://www.microsoft.com/en-us/download/details.aspx?id=21) and later.
* [ASP.NET MVC 3](http://www.asp.net/mvc/mvc3) and later.
* Visual Studio 2012 and later.
* [IIS](https://www.iis.net/) 5 and later.
* [C#](https://msdn.microsoft.com/en-us/library/aa288436(v=vs.71).aspx)  and [VB.NET](http://www.tutorialspoint.com/vb.net/).
* [SharePoint 2010](https://msdn.microsoft.com/en-us/library/office/dd776256(v=office.12).aspx) and later.

## Supported Web Browsers

The [Telerik UI for ASP.NET MVC helpers and framework components](https://demos.telerik.com/aspnet-mvc/) are designed to support all major web browsers and deliver cross-browser compatibility, standards compliance, and touch-device support.

However, depending on the specifics of your project, the components you use, and the versions of the Telerik UI helpers, their browser support may vary.

>To allow the browsers to run the required scripts, enable JavaScript on all of them.

## Browser Support for Regular Components

Most [Telerik UI for ASP.NET MVC helpers]({% slug overview_aspnetmvc6_aspnetmvc %}#list-of-helpers) have no specific limitations regarding the supported browser versions.

| BROWSER           | SUPPORTED VERSIONS            | LIMITATIONS
| :---------------- | :---------------------------- | :---------------
| Edge              | 20 or later ([officially supported versions by Microsoft only](https://en.wikipedia.org/wiki/Microsoft_Edge#Release_history)) |
| Internet Explorer* | 9 or later                    | Some features may not be available due to browser limitations |
| Chrome            | Current and previous          |
| Firefox           | [Current and ESR releases](https://en.wikipedia.org/wiki/History_of_Firefox#Release_history) ([What is ESR?](https://www.mozilla.org/en-US/firefox/organizations/faq/))|
| Opera             | 15 or later                   |
| OS X Safari       | [6.2.6 or later](https://en.wikipedia.org/wiki/Safari_version_history#Mac)|

## Browser Support for Data Visualizing Helpers

The [Telerik UI for ASP.NET MVC helpers which render data visualization]({% slug overview_aspnetmvc6_aspnetmvc %}#list-of-helpers), such as the Charts, Gauges, Barcodes, Diagrams, and Maps, may require more recent browser versions according to the following table.

**Fully supported browsers**

| BROWSER           | SUPPORTED VERSIONS            |
| :---------------- | :---------------------------- |
| Edge              | 20 or later ([officially supported versions by Microsoft only](https://en.wikipedia.org/wiki/Microsoft_Edge#Release_history)) |
| Internet Explorer | 9 or later                    |
| Chrome            | Current and previous          |
| Firefox           | [Current and ESR releases](https://en.wikipedia.org/wiki/History_of_Firefox#Release_history) ([What is ESR?](https://www.mozilla.org/en-US/firefox/organizations/faq/))|
| Opera             | 15 or later                   |
| OS X Safari       | [6.2.6 or later](https://en.wikipedia.org/wiki/Safari_version_history#Mac)|
| iOS Safari        | iOS 8 or later                |
| Chrome for Mobile | 21 or later                   |

**Browsers with limited support**

| BROWSER           | SUPPORTED VERSIONS            | LIMITATIONS                               |
| :---------------- | :---------------------------- | :-----------                              |
| Internet Explorer | 10                            | Dashed lines in canvas are not supported, which affects the image export as well |
|                   |                               | Android 2.x, therefore, uses non-interactive canvas output |
| Android           | 2.3                           | The Canvas rendering mode is only supported

## Browser Support for PDF Export

The Telerik PDF generator is tested and supported in the following desktop browsers:
* Internet Explorer 9 and later.
* Latest Chrome, Firefox, Safari, and Blink-based Opera versions.

> Internet Explorer 9 and Safari do not support the PDF-related option for saving files. To achieve this, you need to [implement a server proxy](https://docs.telerik.com/kendo-ui/controls/data-management/grid/export/pdf-export#using-server-proxy).

Officially, PDF export is not supported on mobile because of browser limitations and CORS-related security restrictions in hybrid applications. For example, it is not possible to load locally stored font files in hybrid applications. Even though exporting in PDF might work on some mobile devices in specific scenarios, PDF export is not supported in mobile browsers and hybrid mobile applications.

## Best Performance

To boost the performance of your project:
* Always use an up-to-date browser version.
* Check **Disable Script Debugging** from your browser configuration options.
* Activate **Caching** in Internet Explorer.

## Limitations

* As of the Telerik UI for ASP.NET MVC 2017 R1 release, Internet Explorer 8 is no longer supported.
* Browsers in beta stage are not supported.
* Zoomed-in pages are not supported.
* Zoomed-out pages are not supported. Different browsers handle sub-pixel calculations differently and zooming out the page may lead to unexpected behavior&mdash;for example, missing borders.
* Exporting a zoomed-in or zoomed-out page to PDF is not supported.
* [Quirks mode](https://www.quirksmode.org/css/quirksmode.html) is not supported.

    > Always specify a [DOCTYPE](https://www.sitepoint.com/web-foundations/doctypes/). Recommended DOCTYPEs include `HTML5`, `XHTML 1.1`, `XHTML 1.0 Strict` and `HTML4 Strict`. The `HTML4 Transitional` DOCTYPE fires the Quirks mode and should not be used. `XHTML 1.0 Transitional` works well in most cases, but may cause issues with the vertical positioning of icons. The correct syntax for [all DOCTYPEs](https://www.w3.org/QA/2002/04/valid-dtd-list.html) is provided on the [W3C website](https://www.w3.org/).

* Internet Explorer compatibility modes are not supported. These modes can exhibit different behavior and rendering bugs as compared to the browser versions they emulate.
* It is highly advisable to use Internet Explorer Edge mode over a META tag or an HTTP header:

    ```
    <meta http-equiv="X-UA-Compatible" content="IE=edge" />
    ```

* Telerik UI for ASP.NET MVC uses a progressive enhancement for its CSS styling. As a result, old and obsolete browsers may ignore CSS 3 styles such as rounded corners and linear gradients.

## See Also

* [jQuery Version Support by Telerik UI for ASP.NET MVC]({% slug jquerysupport_aspnetmvc %})
* [PDF and Excel Export Support by Telerik UI for ASP.NET MVC]({% slug exportsupport_aspnetmvc %})
* [Earlier Versions Support Policy by Telerik UI for ASP.NET MVC]({% slug oldversionssupportpolicy_aspnetmvc %})
