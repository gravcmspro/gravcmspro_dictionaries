[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Link with Icon" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-link url="http://example.com" menu="Settings" icon="code" icon-attributes="class:left"][/m-link]  

  D_CODE

  [m-tag tag="div" attributes="id:material-code"]
    [raw]
    ```
    [m-help]
      Main component properties
      url: The url to link the image. Leave it empty to leave the image unlinked
      menu: undefined
      link-attributes: Adds html attributes to link element. Example attributes="class: foo, rel=bar"
      icon: Defines the icon. You can choose from several kind of icons: material icons, fontawesome, material and glyphicon
      icon-container: Works only when the icon is stacked. Defines the stacked icon container. Usage icon-container="circle"
      icon-attributes: Adds html attributes to icon element. Example attributes="class: foo, rel=bar"
      stacked: Works only for fontawesome icon. Displays a stacked icon. Usage: stacked="true"
      large-icon: Displays the icon large
    [/m-help]
    [m-link url="http://example.com" menu="Settings" icon="code" icon-attributes="class:left"][/m-link]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="material-code" button-label="Copy to clipboard" icon="content_copy"][/m-clipboard]

  ### Link with stacked icon

  Renders a stacked icon using the Fontawesome provider.

  [m-link url="http://example.com" menu="Settings" icon="fa-twitter" icon-attributes="class:left" icon-attributes="class:left" stacked="true" icon-container="fa-circle-o"][/m-link]  

  [m-tag tag="div" attributes="id:stacked-icon-code"]
    [raw]
    ```
    [m-help]
      Main component properties
      url: The url to link the image. Leave it empty to leave the image unlinked
      menu: undefined
      link-attributes: Adds html attributes to link element. Example attributes="class: foo, rel=bar"
      icon: Defines the icon. You can choose from several kind of icons: material icons, fontawesome, material and glyphicon
      icon-container: Works only when the icon is stacked. Defines the stacked icon container. Usage icon-container="circle"
      icon-attributes: Adds html attributes to icon element. Example attributes="class: foo, rel=bar"
      stacked: Works only for fontawesome icon. Displays a stacked icon. Usage: stacked="true"
      large-icon: Displays the icon large
    [/m-help]
    [m-link url="http://example.com" menu="Settings" icon="fa-twitter" icon-attributes="class:left" icon-attributes="class:left" stacked="true" icon-container="fa-circle-o"][/m-link]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="stacked-icon-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

[/m-dictionary-item]
