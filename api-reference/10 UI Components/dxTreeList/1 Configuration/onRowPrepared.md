---
id: dxTreeList.Options.onRowPrepared
type: function(e)
default: null
---
---
##### shortDescription
A function that is executed after a row is created.

##### param(e): Object
Information about the event that caused the function's execution.

##### field(e.columns): Array<dxTreeListColumn>
All column [configurations](/api-reference/10%20UI%20Components/dxTreeList/1%20Configuration/columns '/Documentation/ApiReference/UI_Components/dxTreeList/Configuration/columns/').

##### field(e.component): dxTreeList
The UI component's instance.

##### field(e.data): Object
The row's data. Available if the **rowType** is *"data"*, *"detail"* or *"detailAdaptive"*.

##### field(e.element): DxElement
#include common-ref-elementparam with { element: "UI component" }

##### field(e.isExpanded): Boolean
<!-- %field(e.isExpanded)% -->

##### field(e.isNewRow): Boolean
Indicates that the row is added, but not yet saved. Available if **rowType** is *"data"*.

##### field(e.isSelected): Boolean
Indicates whether the row is selected. Available if **rowType** is *"data"* or *"detail"*.

##### field(e.key): any
The row's key. Available if the **rowType** is *"data"*, *"detail"* or *"detailAdaptive"*.      
For plain data, the value of the key depends on the [keyExpr](/api-reference/10%20UI%20Components/dxTreeList/1%20Configuration/keyExpr.md '/Documentation/ApiReference/UI_Components/dxTreeList/Configuration/#keyExpr') property. For hierarchical data, the key is generated automatically or set in the underlying **Store** of the [data source](/api-reference/10%20UI%20Components/dxTreeList/1%20Configuration/dataSource.md '/Documentation/ApiReference/UI_Components/dxTreeList/Configuration/#dataSource').

##### field(e.level): Number
The node's [hierarchical level](/api-reference/10%20UI%20Components/dxTreeList/4%20Node/level.md '/Documentation/ApiReference/UI_Components/dxTreeList/Node/#level').

##### field(e.model): any
Model data. Available only if you use Knockout.

##### field(e.node): dxTreeListNode
The row's node.

##### field(e.rowElement): DxElement
#include common-ref-elementparam with { element: "row" }

##### field(e.rowIndex): Number
The row's index. Refer to [Column and Row Indexes](/concepts/05%20UI%20Components/TreeList/10%20Columns/12%20Column%20and%20Row%20Indexes.md '/Documentation/Guide/UI_Components/TreeList/Columns/Column_and_Row_Indexes/') for more information.

##### field(e.rowType): String
The row's [type](/api-reference/10%20UI%20Components/dxTreeList/6%20Row/rowType.md '/Documentation/ApiReference/UI_Components/dxTreeList/Row/#rowType').

##### field(e.values): Array<any>
Values displayed in the row cells.

---

<!-- import { field(e.isExpanded) } from 'api-reference\10 UI Components\dxTreeList\1 Configuration\onRowClick.md' -->