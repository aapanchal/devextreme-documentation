---
id: dxDiagram.Options.onItemDblClick
type: function(e)
default: null
---
---
##### shortDescription
A function that is executed after a shape or connector is double-clicked.

##### param(e): Object
Information about the event.

##### field(e.component): dxDiagram
The UI component instance's name.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.item): dxDiagramItem
A **dxDiagramItem** object descendant (dxDiagramShape or dxDiagramConnector) related to the event.

##### field(e.model): any
Model data. Available only if you use Knockout.

---
