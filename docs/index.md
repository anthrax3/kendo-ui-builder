---
title: Introduction
page_title: Introduction | Kendo UI Builder
description: "Welcome to the Kendo UI® Builder by Progress® tool for creating and managing Angular and AngularJS-based web applications."
slug: intro_kuib
position: 0
---

# Introduction to Kendo UI Builder

Kendo UI® Builder by Progress® (Kendo UI Builder) is a tool for creating and managing web applications.

The Builder separates the user interface (UI) settings&mdash;views and modules&mdash;from the business logic of the project which runs on the application server. The UIs are also convenient for revamping existing applications and enabling them to support the implementation of Kendo UI components. In addition, the tool delivers extension points for customization and supports the creation of Angular and AngularJS-based projects.

For more information on how to integrate the Builder into OpenEdge business applications, refer to the [official Progress<sup>®</sup> Software Documentation](https://www.progress.com/documentation/kendo-ui-builder).  

## Building Blocks

Basically, the Builder provides its options through the delivery of [modules](#toc-modules), [data providers](#toc-data-providers), and [extension points](#toc-extension-points).

<!-- diagram -- >

KUIB -> Modules         -> Views          -> System
                                          -> Predefined
                                          -> Custom (Blank)    -> Components    -> Predefined
                                                                                -> Custom
    -> Data Providers   -> Data Services
                        -> Data Sources
    -> Extension Points -> Style          -> Theme
                                          -> View
                                          -> Application
                        -> Template
                        -> View
                        -> Component

### Modules

Modules consist of:

* Views&mdash;Provide the setting and outlook options for the current application page.
    * The [system views]({% slug systemviews_kuib %}) are built-in and cannot be modified.
    * The [predefined views]({% slug predefinedviews_kuib %}) are built-in and offer a predefined layout which can be modified.
    * The [custom (user-defined) view]({% slug customviews_kuib %}) is the Blank view which can be created and customized according to the requirements of the business project. The user-defined view allows you to add, edit, or remove both predefined and custom components.  
* Components&mdash;Represent the widgets that will be rendered by the application and can be added to a Blank view.
    * The [predefined components]({% slug overviewcomp_kuib %}) offer a predefined layout which can be used in the application either as they are or after you update them.
    * The [custom (user-defined) component]({% slug customcomp_kuib %}) is a blank component which can be created and customized according to the requirements of the business project.

> The modules and the views, which handle the UI of the application, comprise the [Kendo UI Designer]({% slug getstarted_kdesigner %}).

### Data Providers

Data providers handle the data connectivity of the application. They enable services for establishing the connection between the data you want to display and the data source you want to use.

* The [data services]({% slug dataprovidersoverview_kuib %}) support the input of third-party or custom service endpoints.
* The [data sources]({% slug dataspurces_kuib %}) contain the datasets and enable you to display all available or a specific portion of data.

### Extension Points

Extension points are the parts of the web application that you can customize.

* The [styles extension points]({% slug customstyles_kuib %}) deliver options for customizing the appearance of the whole application or of the current theme, view, or component.  
* The [templates extension points]({% slug customtemplatestyles_kuib %}) deliver options for customizing the content optimization and rendition.
* The [views extension points]({% slug customviews_kuib %}) deliver options for customizing each view.  
* The [components extension points]({% slug customcomponents_kuib %}) deliver options for customizing each component.

## Basic Approaches

The data definitions of the application are stored in JSON metadata that is separate from the UI implementation. The metadata is then used by the integrated Generator to compile the HTML5, CSS, and JavaScript files that are built for and used by the application. The generation of the application also allows you to immediately preview the project in the Designer by applying live data. For further development testing and production, you can then deploy the application to separate web servers.

To create functional views within one or more application modules, you need to submit inputs which include a set of selectable Kendo UI templates. Each application module can contain one or more user-defined (custom) views and, depending on the data you want to render, you can bind each view to one or more data sources. The Builder allows you to define multiple data providers for an application&mdash;depending on the specific view, you can select one or more data providers and bind that view to a portion of the data or to all the data from a data source. As a result, some views can be bound to one data source at a time while others can be bound to multiple data sources.

By using their corresponding properties, you can configure the [modules]({% slug modulesoverview_kuib %}) and their [views]({% slug viewsoverview_kuib %}), and the [data providers]({% slug dataprovidersoverview_kuib %}) and their [data sources]({% slug dataspurces_kuib %}). These properties help define the application metadata which is separately saved for each module and data provider that you define.

The Builder also enables you to customize each view through code extensions, which manage its event handlers, and the custom sections in the view layout. Other available extension points that are subject to customization are the styles, templates, and components in the application.

## Suggested Links

* [Getting Started with the Kendo UI Builder]({% slug getstarted_kuib %})
* [Getting Started with the Kendo UI Designer]({% slug getstarted_kdesigner %})
* [Modules]({% slug modulesoverview_kuib %})
* [Views]({% slug viewsoverview_kuib %})
* [Components]({% slug overviewcomp_kuib %})
* [Data Providers]({% slug dataprovidersoverview_kuib %})
* [Extension Points]({% slug extensionpoints_kuib %})
* [Frameworks]({% slug angular_kuib %})