[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Anchor" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  Adds an invisible anchor placeholder, revealed when the maouse is placed over it. This element is very useful to link a specific page section, for example **https://example.com/#section**

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Adds an anchor placeholder. Change the attributes' name property, anchor_name in this example, to define your anchor

      link-attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      icon: Defines the icon. You can choose from several kind of icons: material icons, fontawesome, material and glyphicon
    [/m-help]
    [m-link link-attributes="class: opaque opaque-reveal, name:anchor_name" icon="fa-link fa-flip-horizontal"][/m-link]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
