---
EventForAction: ..\4 Events\selectionChanged.md
default: null
type: function(e)
---
---
##### notUsedInTheme

##### shortDescription
A function that is executed when a node is selected or the selection is canceled.

##### param(e): Object
Information about the event.

##### field(e.component): {WidgetName}
The widget's instance.

##### field(e.element): dxElement
The widget's container. It is an [HTML Element](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement) or a [jQuery Element](https://api.jquery.com/Types/#jQuery) when you use jQuery.

##### field(e.model): Object
The model data. Available only if you use Knockout.

##### field(e.node): dxTreeMapNode
The node whose selection state has been changed; described in the [Node](/api-reference/20%20Data%20Visualization%20Widgets/dxTreeMap/6%20Node '/Documentation/ApiReference/Data_Visualization_Widgets/dxTreeMap/Node/') section.

---
To identify whether the selection has been applied or canceled, call the node's [isSelected()](/api-reference/20%20Data%20Visualization%20Widgets/dxTreeMap/6%20Node/3%20Methods/isSelected().md '/Documentation/ApiReference/Data_Visualization_Widgets/dxTreeMap/Node/Methods/#isSelected') method. To identify whether the clicked node is a single tile or a group of tiles, use the node's [isLeaf()](/api-reference/20%20Data%20Visualization%20Widgets/dxTreeMap/6%20Node/3%20Methods/isLeaf().md '/Documentation/ApiReference/Data_Visualization_Widgets/dxTreeMap/Node/Methods/#isLeaf') method.