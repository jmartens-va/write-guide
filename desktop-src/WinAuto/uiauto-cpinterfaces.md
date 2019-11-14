---
title: Control Pattern Interfaces for Providers
description: This section describes control pattern interfaces implemented by UI Automation providers to expose information about controls in unmanaged Windows applications.
ms.assetid: 08d0226d-845c-4564-a059-539b62fc7909
ms.topic: article
ms.date: 05/31/2018
---

# Control Pattern Interfaces for Providers

This section describes *control pattern* interfaces implemented by UI Automation providers to expose information about controls in unmanaged Windows applications.

## In this section



| Interface                                                                          | Description                                                                                                                                                                                                                                                                                                         |
|------------------------------------------------------------------------------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**IAnnotationProvider**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-iannotationprovider)<br/>           | Exposes the properties of an annotation in a document.<br/>                                                                                                                                                                                                                                                   |
| [**IDockProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-idockprovider)<br/>                           | Provides access to an element in a docking container. <br/>                                                                                                                                                                                                                                                   |
| [**IDragProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-idragprovider)<br/>                           | Enables a Microsoft UI Automation element to describe itself as an element that can be dragged as part of a drag-and-drop operation.<br/>                                                                                                                                                                     |
| [**IDropTargetProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-idroptargetprovider)<br/>               | Enables a UI Automation element to describe itself as an element that can receive a drop of a dragged element as part of a UI Automation drag-and-drop operation.<br/>                                                                                                                                        |
| [**IExpandCollapseProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iexpandcollapseprovider)<br/>       | Provides access to a control that visually expands to display content, and collapses to hide content. <br/>                                                                                                                                                                                                   |
| [**IGridItemProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-igriditemprovider)<br/>                   | Provides access to individual child controls of containers that implement [**IGridProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-igridprovider).<br/>                                                                                                                                                                                 |
| [**IGridProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-igridprovider)<br/>                           | Provides access to controls that act as containers for a collection of child elements organized in a two-dimensional logical coordinate system that can be traversed (that is, a UI Automation client can move to adjacent controls) by using the keyboard.<br/>                                              |
| [**IInvokeProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iinvokeprovider)<br/>                       | Provides access to controls that initiate or perform a single, unambiguous action and do not maintain state when activated.<br/>                                                                                                                                                                              |
| [**IItemContainerProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iitemcontainerprovider)<br/>         | Provides access to controls that act as containers of other controls, such as a virtual list-view. <br/>                                                                                                                                                                                                      |
| [**ILegacyIAccessibleProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ilegacyiaccessibleprovider)<br/> | Enables UI Automation clients to access the underlying [**IAccessible**](/windows/desktop/api/oleacc/nn-oleacc-iaccessible) implementation of Microsoft Active Accessibility elements.<br/>                                                                                                                                                     |
| [**IMultipleViewProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-imultipleviewprovider)<br/>           | Provides access to controls that provide, and are able to switch between, multiple representations of the same set of information or child controls.<br/>                                                                                                                                                     |
| [**IObjectModelProvider**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-iobjectmodelprovider)<br/>         | Provides access to the underlying object model implemented by a control or application. <br/>                                                                                                                                                                                                                 |
| [**IRangeValueProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-irangevalueprovider)<br/>               | Provides access to controls that can be set to a value within a range. <br/>                                                                                                                                                                                                                                  |
| [**IScrollItemProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iscrollitemprovider)<br/>               | Provides access to individual child controls of containers that implement [**IScrollProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iscrollprovider). <br/>                                                                                                                                                                            |
| [**IScrollProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iscrollprovider)<br/>                       | Provides access to controls that act as scrollable containers for a collection of child objects.<br/>                                                                                                                                                                                                         |
| [**ISelectionItemProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iselectionitemprovider)<br/>         | Provides access to individual, selectable child controls of containers that implement [**ISelectionProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iselectionprovider). <br/>                                                                                                                                                          |
| [**ISelectionProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iselectionprovider)<br/>                 | Provides access to controls that act as containers for a collection of individual, selectable child items.<br/>                                                                                                                                                                                               |
| [**ISelectionProvider2**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iselectionprovider2)<br/>               | Extends the [**ISelectionItemProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iselectionitemprovider) interface to provide information about selected items.<br/>                                                                                                                                                                       |
| [**ISpreadsheetItemProvider**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-ispreadsheetitemprovider)<br/> | Provides access to information about an item (cell) in a spreadsheet. <br/>                                                                                                                                                                                                                                   |
| [**ISpreadsheetProvider**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-ispreadsheetprovider)<br/>         | Provides access to items (cells) in a spreadsheet.<br/>                                                                                                                                                                                                                                                       |
| [**IStylesProvider**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-istylesprovider)<br/>                   | Provides access to the visual styles associated with the content of a document.<br/>                                                                                                                                                                                                                          |
| [**ISynchronizedInputProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-isynchronizedinputprovider)<br/> | Enables UI Automation client applications to direct the mouse or keyboard input to a specific UI element. <br/>                                                                                                                                                                                               |
| [**ITableItemProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itableitemprovider)<br/>                 | Provides access to child controls of containers that implement [**ITableProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itableprovider). <br/>                                                                                                                                                                                         |
| [**ITableProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itableprovider)<br/>                         | Provides access to controls that act as containers for a collection of child elements. The children of this element must implement [**ITableItemProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itableitemprovider) and be organized in a two-dimensional logical coordinate system that can be traversed by using the keyboard. <br/> |
| [**ITextChildProvider**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-itextchildprovider)<br/>            | Provides access to a text-based control (or an object embedded in text) that is a child or descendant of another text-based control. <br/>                                                                                                                                                                    |
| [**ITextEditProvider**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-itexteditprovider)<br/>               | Extends the [**ITextProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextprovider) interface to enable UI Automation providers to expose programmatic text-edit actions.<br/>                                                                                                                                                          |
| [**ITextProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextprovider)<br/>                           | Provides access to controls that contain text. <br/>                                                                                                                                                                                                                                                          |
| [**ITextProvider2**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-itextprovider2)<br/>                     | Extends the [**ITextProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextprovider) interface to enable UI Automation providers to expose textual content that is the target of an annotation, and information about a caret that belongs to the provider.<br/>                                                                         |
| [**ITextRangeProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextrangeprovider)<br/>                 | Provides access to a span of continuous text in a text container that implements [**ITextProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextprovider) or [**ITextProvider2**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextprovider2).<br/>                                                                                                                       |
| [**ITextRangeProvider2**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextrangeprovider2)<br/>               | Extends the [**ITextRangeProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itextrangeprovider) interface to enable UI Automation providers to invoke context menus.<br/>                                                                                                                                                                 |
| [**IToggleProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itoggleprovider)<br/>                       | Provides access to controls that can cycle through a set of states and maintain a state after it is set.<br/>                                                                                                                                                                                                 |
| [**ITransformProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itransformprovider)<br/>                 | Provides access to controls that can be moved, resized, and/or rotated within a two-dimensional space. <br/>                                                                                                                                                                                                  |
| [**ITransformProvider2**](https://docs.microsoft.com/windows/desktop/api/uiautomationcore/nn-uiautomationcore-itransformprovider2)<br/>           | Extends the [**ITransformProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-itransformprovider) interface to enable UI Automation providers to expose properties to support the viewport zooming functionality of a control. <br/>                                                                                                        |
| [**IValueProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ivalueprovider)<br/>                         | Provides access to controls that have an intrinsic value that does not span a range, and that can be represented as a string. <br/>                                                                                                                                                                           |
| [**IVirtualizedItemProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-ivirtualizeditemprovider)<br/>     | Provides access to virtualized items, which are items that are represented by placeholder automation elements in the UI Automation tree.<br/>                                                                                                                                                                 |
| [**IWindowProvider**](/windows/desktop/api/UIAutomationCore/nn-uiautomationcore-iwindowprovider)<br/>                       | Provides access to the fundamental window-based functionality of a control.<br/>                                                                                                                                                                                                                              |



 

## Related topics

<dl> <dt>

[Control Pattern Interfaces for Providers](uiauto-cpinterfaces.md)
</dt> </dl>

 

 




