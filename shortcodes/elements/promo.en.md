[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Modular collection" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-grid attributes="class:icons-promo" container="false"]
    [m-grid-row attributes="class:center"]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-promo-table-item icon="style" attributes="box-medium"]
          ## Item 1
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-promo-table-item]
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-promo-table-item icon="create" attributes="box-medium"]
          ## Item 2
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-promo-table-item]
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-promo-table-item icon="dvr" attributes="box-medium"]
          ## Item 3
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-promo-table-item]
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
      [m-grid attributes="class:icons-promo"]
        [m-grid-row attributes="class:center"]
          [m-grid-col attributes="class:s12 m4 l4"]
            [m-promo-table-item icon="style" attributes="box-medium"]
              ## Item 1
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            [/m-promo-table-item]
          [/m-grid-col]
          [m-grid-col attributes="class:s12 m4 l4"]
            [m-promo-table-item icon="create" attributes="box-medium"]
              ## Item 2
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            [/m-promo-table-item]
          [/m-grid-col]
          [m-grid-col attributes="class:s12 m4 l4"]
            [m-promo-table-item icon="dvr" attributes="box-medium"]
              ## Item 3
              Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
            [/m-promo-table-item]
          [/m-grid-col]
        [/m-grid-row]
      [/m-grid]  
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
