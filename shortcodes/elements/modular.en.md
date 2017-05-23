[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Modular collection" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  This shortcode renders a Grav modular page.

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
      [m-modular-collection][/m-modular-collection]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  This shortcode requires the page header is properly configured to define a Grav modular page, as follows:
  [raw]
  ```
    content:
        items: @self.modular
        order:
            by: default
            dir: asc
            custom:
                - _module_1
                - _module_2
  ```
  [/raw]

[/m-dictionary-item]
