---
Description: The topics contained in this section provide the reference specifications for Direct Manipulation interfaces.
ms.assetid: 03680CE5-A858-4876-B41C-6F2E08C02C22
title: Direct Manipulation Interfaces
ms.technology: desktop
ms.prod: windows
ms.author: windowssdkdev
ms.topic: article
ms.date: 05/31/2018
---

# Direct Manipulation Interfaces

The topics contained in this section provide the reference specifications for [Direct Manipulation](direct-manipulation-portal.md) interfaces.

> [!Note]  
> When implementing a [Direct Manipulation](direct-manipulation-portal.md) object, ensure that the [**IUnknown**](https://msdn.microsoft.com/windows/desktop/33f1d79a-33fc-4ce5-a372-e08bda378332) implementation supports multithreading through thread-safe reference counting. For more information, see [**InterlockedIncrement**](https://msdn.microsoft.com/windows/desktop/87eda7fb-966d-4630-9da6-8933b53daadd) and [**InterlockedDecrement**](https://msdn.microsoft.com/windows/desktop/d6ed6cb1-aa10-48f4-9b62-73708ff4d1e3).

 

## In this section



| Topic                                                                                                       | Description                                                                                                                                                                                                                                                                  |
|-------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| [**IDirectManipulationAutoScrollBehavior**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationautoscrollbehavior)<br/>           | Represents the auto-scroll animation behavior of content as it approaches the boundary of a given axis or axes.<br/>                                                                                                                                                   |
| [**IDirectManipulationCompositor**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationcompositor)<br/>                           | Represents a compositor object that associates manipulated content with a drawing surface, such as [**canvas**](https://www.bing.com/search?q=**canvas**) (Windows app using JavaScript) or [**Canvas**](https://www.bing.com/search?q=**Canvas**) (Windows Store app using C++, C\#, or Visual Basic).<br/> |
| [**IDirectManipulationCompositor2**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationcompositor2)<br/>                         | Represents a compositor object that associates manipulated content with drawing surfaces across multiple processes.<br/>                                                                                                                                               |
| [**IDirectManipulationContent**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationcontent)<br/>                                 | Encapsulates content inside a viewport, where content represents a visual surface clipped inside the viewport.<br/>                                                                                                                                                    |
| [**IDirectManipulationDeferContactService**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationdefercontactservice)<br/>         | Represents a service for managing associations between a contact and a viewport.<br/>                                                                                                                                                                                  |
| [**IDirectManipulationDragDropBehavior**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationdragdropbehavior)<br/>               | Represents behaviors for drag and drop interactions, which are triggered by cross-slide or press-and-hold gestures. <br/>                                                                                                                                              |
| [**IDirectManipulationDragDropEventHandler**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationdragdropeventhandler)<br/>       | Defines methods to handle drag-drop behavior events.<br/>                                                                                                                                                                                                              |
| [**IDirectManipulationFrameInfoProvider**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationframeinfoprovider)<br/>             | Represents a time-keeping object that measures the latency of the composition infrastructure used by the application and provides this data to [Direct Manipulation](direct-manipulation-portal.md). <br/>                                                            |
| [**IDirectManipulationInteractionEventHandler**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationinteractioneventhandler)<br/> | Defines methods to handle interactions when they are detected.<br/>                                                                                                                                                                                                    |
| [**IDirectManipulationManager**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationmanager)<br/>                                 | Provides access to all the [Direct Manipulation](direct-manipulation-portal.md) features and APIs available to the client application.<br/>                                                                                                                           |
| [**IDirectManipulationManager2**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationmanager2)<br/>                               | Extends the [**IDirectManipulationManager**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationmanager) interface that provides access to all the [Direct Manipulation](direct-manipulation-portal.md) features and APIs available to the client application. <br/>                              |
| [**IDirectManipulationManager3**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationmanager3)<br/>                               | Extends the [**IDirectManipulationManager2**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationmanager2) interface that provides access to all the [Direct Manipulation](direct-manipulation-portal.md) features and APIs available to the client application. <br/>                            |
| [**IDirectManipulationPrimaryContent**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationprimarycontent)<br/>                   | Encapsulates the primary content inside a viewport.<br/>                                                                                                                                                                                                               |
| [**IDirectManipulationUpdateHandler**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationupdatehandler)<br/>                     | Defines methods for handling manipulation update events.<br/>                                                                                                                                                                                                          |
| [**IDirectManipulationUpdateManager**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationupdatemanager)<br/>                     | Manages how compositor updates are sent to [Direct Manipulation](direct-manipulation-portal.md).<br/>                                                                                                                                                                 |
| [**IDirectManipulationViewport**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationviewport)<br/>                               | Defines a region within a window (referred to as a viewport) that is able to receive and process input from user interactions. <br/>                                                                                                                                   |
| [**IDirectManipulationViewport2**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationviewport2)<br/>                             | Provides management of behaviors on a viewport. A behavior affects the functionality of a particular part of the [Direct Manipulation](direct-manipulation-portal.md) workflow. <br/>                                                                                 |
| [**IDirectManipulationViewportEventHandler**](/previous-versions/windows/desktop/api/DirectManipulation/nn-directmanipulation-idirectmanipulationviewporteventhandler)<br/>       | Defines methods for handling status and update events for the viewport.<br/>                                                                                                                                                                                           |



 

 

 



