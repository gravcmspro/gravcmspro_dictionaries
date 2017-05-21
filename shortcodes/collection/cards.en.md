[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Modular collection" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-help]
    Main component properties
    image: The image name with the extension. Set a blank value for no image
    image-path: The image directory
    card-attributes: Adds html attributes to card element. Example card-attributes="class: blue-grey darken-1"
    content-attributes: Adds html attributes to the div that contains the content. Example attributes="class: foo, rel=bar"
  [/m-help]
  [m-card-collection page-name="/shortcodes/basic" card-type="card" container-attributes="class:box-medium s-margin-bottom-small m-margin-bottom-medium" column-attributes="class:col s12 m6 l6" content_attributes="class:h4-size center"]
  [/m-card-collection]  

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
