Color swatches are secondary color schemes used alongside a primary color scheme. You can use them to stylize parts of your application differently, for instance, when the navigation sidebar should be dark and the content area light.

A color swatch is defined by scoped CSS rules that are prefixed with a specific selector: `dx-swatch-xxx` (for instance, `dx-swatch-green`). To apply a color swatch to a part of an HTML document, wrap this part as follows:

    <!--HTML-->
    <div>
        This content applies the primary color scheme

        <div class="dx-swatch-dark">
            This content applies the "dark" color scheme
        </div>
    </div>

[important] Color swatches should belong to the same theme as the main application theme (Generic, Generic Compact, or Material). For example, if the main application theme is Material, you can use only the color swatches that are based on the Material theme.

You can generate color swatches with the DevExtreme CLI or ThemeBuilder UI:

* **<a href="https://github.com/DevExpress/devextreme-cli/blob/master/README.md" target="_blank">DevExtreme CLI</a>**        

    The following command generates a new `custom` color swatch that uses Generic Dark as a base theme:

        > devextreme build-theme –-base-theme="generic.dark" --make-swatch --output-color-scheme="dark"
        // ===== or without installing DevExtreme CLI globally =====
        > npx -p devextreme-cli devextreme build-theme –-base-theme="generic.dark" --make-swatch --output-color-scheme="dark"

    The result of this command is a `dx.generic.dark.css` file in which every rule is prefixed with the `.dx-swatch-dark` CSS selector. Move the file to the application folder, [register it](/concepts/60%20Themes%20and%20Styles/05%20Predefined%20Themes/50%20Apply%20a%20Theme.md '/Documentation/Guide/Themes_and_Styles/Predefined_Themes/#Apply_a_Theme'), and add the swatch class to a page element.

    Refer to <a href="https://github.com/DevExpress/devextreme-cli/blob/master/README.md#themebuilder" target="_blank">DevExtreme CLI: ThemeBuilder</a> for more information about CLI commands and command line arguments.

* **[ThemeBuilder UI](/concepts/60%20Themes%20and%20Styles/08%20ThemeBuilder '/Documentation/Guide/Themes_and_Styles/ThemeBuilder/')**       

    Click **Export** on the toolbar to open the **Theme Export** pop-up dialog. Enter the color swatch's name, check the **Save as a color swatch** checkbox, and proceed to the last step.

    ![DevExtreme ThemeBuilder UI: Theme Export popup dialog, Enter Name](/images/Common/ThemeBuilder/themebuilder-themeexport-name.png)

    Click **Download CSS File** to save a CSS file on your computer.

    ![DevExtreme ThemeBuilder UI: Theme Export popup dialog, Choose Format](/images/Common/ThemeBuilder/themebuilder-themeexport-format.png)

    Move the resulting CSS file to the application folder, [register it](/concepts/60%20Themes%20and%20Styles/05%20Predefined%20Themes/50%20Apply%20a%20Theme.md '/Documentation/Guide/Themes_and_Styles/Predefined_Themes/#Apply_a_Theme'), and add the swatch class to a page element.

[note] Color swatches cannot be used to customize SVG-based UI components because the [UI component's themes are UI component configurations](/concepts/60%20Themes%20and%20Styles/20%20SVG-Based%20Components%20Customization/15%20Themes/00%20Themes.md '/Documentation/Guide/Themes_and_Styles/SVG-Based_Components_Customization/#Themes') that do not use CSS. With [predefined CSS themes](/concepts/60%20Themes%20and%20Styles/05%20Predefined%20Themes/00%20Predefined%20Themes.md '/Documentation/Guide/Themes_and_Styles/Predefined_Themes/'), SVG-based UI components detect which theme is used on the page and apply the corresponding UI component configuration. When an SVG-based UI component is within a color swatch, the detection is impossible. However, you can [create and apply a UI component configuration](/concepts/60%20Themes%20and%20Styles/20%20SVG-Based%20Components%20Customization/15%20Themes/30%20Create%20a%20Custom%20Theme.md '/Documentation/Guide/Themes_and_Styles/SVG-Based_Components_Customization/#Themes/Create_a_Custom_Theme') that visually fits the color swatch.
