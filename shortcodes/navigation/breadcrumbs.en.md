[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Breadcrumb" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l12 red"]
        [m-breadcrumb][/m-breadcrumb]
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Renders a breadcrumb navigation menu. This shortcode does not require parameters.
    [/m-help]
    [m-breadcrumb][/m-breadcrumb]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

[/m-dictionary-item]
