---
EventForAction: ..\4 Events\contextMenuPreparing.md
default: null
type: function(e)
---
---
##### shortDescription
A function that is executed before the context menu is rendered.

##### param(e): Object
Information about the event.

##### field(e.component): {WidgetName}
The widget's instance.

##### field(e.element): dxElement
The widget's container. It is an [HTML Element](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement) or a [jQuery Element](https://api.jquery.com/Types/#jQuery) when you use jQuery.

##### field(e.model): Object
The model data. Available only if Knockout is used.

##### field(e.items): Array<Object>
An array of items to be displayed by the context menu. The item objects must have the fields that are used by the **ContextMenu** [default item template](/api-reference/10%20UI%20Widgets/dxContextMenu/5%20Default%20Item%20Template '/Documentation/ApiReference/UI_Widgets/dxContextMenu/Default_Item_Template').

##### field(e.area): String
The clicked [area's](/api-reference/30%20Data%20Layer/PivotGridDataSource/1%20Configuration/fields/area.md '/Documentation/ApiReference/Data_Layer/PivotGridDataSource/Configuration/fields/#area') type.

##### field(e.cell): dxPivotGridPivotGridCell
The cell that has been clicked to invoke the context menu.    
Unavailable for fields in the [field panel](/concepts/05%20Widgets/PivotGrid/010%20Visual%20Elements/15%20Field%20Panel.md '/Documentation/Guide/Widgets/PivotGrid/Visual_Elements/#Field_Panel').

##### field(e.cellElement): dxElement
The clicked cell's container. It is an [HTML Element](https://developer.mozilla.org/en-US/docs/Web/API/HTMLElement) or a [jQuery Element](https://api.jquery.com/Types/#jQuery) when you use jQuery.  
Unavailable for fields in the [field panel](/concepts/05%20Widgets/PivotGrid/010%20Visual%20Elements/15%20Field%20Panel.md '/Documentation/Guide/Widgets/PivotGrid/Visual_Elements/#Field_Panel').

##### field(e.columnIndex): Number
The index of the column to which the clicked cell belongs.    
Unavailable for fields in the [field panel](/concepts/05%20Widgets/PivotGrid/010%20Visual%20Elements/15%20Field%20Panel.md '/Documentation/Guide/Widgets/PivotGrid/Visual_Elements/#Field_Panel').

##### field(e.rowIndex): Number
The index of the row to which the clicked cell belongs.    
Unavailable for fields in the [field panel](/concepts/05%20Widgets/PivotGrid/010%20Visual%20Elements/15%20Field%20Panel.md '/Documentation/Guide/Widgets/PivotGrid/Visual_Elements/#Field_Panel').

##### field(e.dataFields): Array<PivotGridDataSource_Options_fields>
Fields in the "data" area.

##### field(e.rowFields): Array<PivotGridDataSource_Options_fields>
Fields in the "row" area.

##### field(e.columnFields): Array<PivotGridDataSource_Options_fields>
Fields in the "column" area.

##### field(e.field): PivotGridDataSource_Options_fields
This field's [configuration](/api-reference/30%20Data%20Layer/PivotGridDataSource/1%20Configuration/fields '/Documentation/ApiReference/Data_Layer/PivotGridDataSource/Configuration/fields/').    
Available for fields in the [field panel](/concepts/05%20Widgets/PivotGrid/010%20Visual%20Elements/15%20Field%20Panel.md '/Documentation/Guide/Widgets/PivotGrid/Visual_Elements/#Field_Panel') only.

---