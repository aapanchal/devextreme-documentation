---
default: undefined
type: animationConfig
---
---
##### shortDescription
Specifies the animation to be used to show the rendered content.

---
You can pass a [configuration object](/api-reference/50%20Common/Object%20Structures/animationConfig '/Documentation/ApiReference/Common/Object_Structures/animationConfig/') defining the required animation or the name of one of the [registered animations](/api-reference/50%20Common/utils/animationPresets '/Documentation/ApiReference/Common/Utils/animationPresets/').

Note that you can specify a staggered animation so that content elements with a similar [selector](/api-reference/10%20UI%20Widgets/dxDeferRendering/1%20Configuration/staggerItemSelector.md '/Documentation/ApiReference/UI_Widgets/dxDeferRendering/Configuration/#staggerItemSelector') are animated using the specified animation one after another with a specified delay. For details, refer to the [Animate the Content Appearance](/concepts/05%20Widgets/DeferRendering/10%20Animate%20the%20Content%20Appearance.md '/Documentation/Guide/Widgets/DeferRendering/Animate_the_Content_Appearance/') article.