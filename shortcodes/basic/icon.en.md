[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Icon" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-icon icon="code" icon-attributes="class:foo"][/m-icon]  

  D_CODE

  [m-tag tag="div" attributes="id:material-code"]
    [raw]
    ```
    [m-help]
      Main component properties
      icon: Defines the icon. You can choose from several kind of icons: material icons, fontawesome, material and glyphicon
      icon-attributes: Adds html attributes to icon element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-icon icon="code" icon-attributes="class:foo"][/m-icon]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="material-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  This shortcode supports several icons providers you can use out of the box:

  1. Google Material icons
  2. Fontawesome
  3. MDI Material icons

  ### Google Material icons
  All those icons have no prefix.

  [m-icon icon="group_work" icon-attributes="class:medium"][/m-icon]  

  [m-tag tag="div" attributes="id:material-1-code"]
    [raw]
    ```
    [m-help]
      Main component properties
      icon: Defines the icon. You can choose from several kind of icons: material icons, fontawesome, material and glyphicon
      icon-attributes: Adds html attributes to icon element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-icon icon="group_work" icon-attributes="class:medium"][/m-icon]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="material-1-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  ### Font Awesome icons
  Icons have the **fa** prefix.

  [m-icon icon="fa-grav" icon-attributes="class:fa-3x"][/m-icon]  

  [m-tag tag="div" attributes="id:fontawesome-code"]
    [raw]
    ```
    [m-help]
      Main component properties
      icon: Defines the icon. You can choose from several kind of icons: material icons, fontawesome, material and glyphicon
      icon-attributes: Adds html attributes to icon element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-icon icon="fa-grav" icon-attributes="class:fa-3x"][/m-icon] 
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="fontawesome-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  ### MDI Material icons
  Icons have the **mdi** prefix.

  [m-icon icon="mdi-alert-octagram" icon-attributes="class:fa-3x"][/m-icon]  

  [m-tag tag="div" attributes="id:mdi-code"]
    [raw]
    ```
    [m-help]
      Main component properties
      icon: Defines the icon. You can choose from several kind of icons: material icons, fontawesome, material and glyphicon
      icon-attributes: Adds html attributes to icon element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-icon icon="mdi-alert-octagram" icon-attributes="class:fa-3x"][/m-icon]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="mdi-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]


[/m-dictionary-item]
