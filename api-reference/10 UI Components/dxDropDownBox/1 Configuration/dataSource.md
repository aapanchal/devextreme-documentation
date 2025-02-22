---
id: dxDropDownBox.Options.dataSource
type: Store | DataSource | DataSource_Options | String | Array<any> | null
default: null
---
#include common-dataSource-description with {
    widget_works_with: "The DropDownBox works with collections of objects or `string`, `number`, or `boolean` values. ",

    object_structure_notes: "In each case, also specify the [valueExpr](/api-reference/10%20UI%20Components/DataExpressionMixin/1%20Configuration/valueExpr.md '/Documentation/ApiReference/UI_Components/dxDropDownBox/Configuration/#valueExpr') and [displayExpr](/api-reference/10%20UI%20Components/DataExpressionMixin/1%20Configuration/displayExpr.md '/Documentation/ApiReference/UI_Components/dxDropDownBox/Configuration/#displayExpr') properties if the data source provides objects. ",

    additional_data_binding_actions: "If the element embedded in the DropDownBox UI component is another DevExtreme UI component, their data sources should be interrelated. Refer to the [Synchronize with the Embedded Element](/concepts/05%20UI%20Components/DropDownBox/15%20Synchronize%20with%20the%20Embedded%20Element.md '/Documentation/Guide/UI_Components/DropDownBox/Synchronize_with_the_Embedded_Element/') article for more information.",

    dataSource_items_note: "- Do not specify the [items](/api-reference/10%20UI%20Components/dxDropDownBox/1%20Configuration/items.md '{basewidgetpath}/Configuration/items/') property if you specified the **dataSource**, and vice versa."
}