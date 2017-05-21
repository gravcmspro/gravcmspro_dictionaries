[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Right background picture with text" component (PRO)
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="right-background-picture-with-text" folder="images-and-text" M_IMAGE="image.jpg" M_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-medium box-bg-secondary text-full-white l-vertical-align"  M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
    [m-tag tag="div" attributes="class:padding-left-right-medium"]
      ### Lorem ipsum dolor
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-tag]
  [/m-component]

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_IMAGE: The image name with the extension. Set a blank value for no image
      M_PATH: The image directory
      M_BOX_SIZE: Defines the size for all the item's boxes. This property accepts the following values:box-ultra-tiny, box-tiny, box-small, box-medium, box-large, box-huge
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="right-background-picture-with-text" folder="images-and-text" M_IMAGE="image.jpg" M_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-medium box-bg-secondary text-full-white l-vertical-align"  M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
      [m-tag tag="div" attributes="class:padding-left-right-medium"]
        ### Lorem ipsum dolor
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-tag]
    [/m-component]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  D_THE_CODE_COMPONENT

  [m-tag tag="div" attributes="id:component-code"]
    [raw]
    ```
    [m-grid container="false" attributes="M_ATTRIBUTES"]
      [m-grid-row attributes="M_ROW_ATTRIBUTES"]
        [m-grid-col attributes="M_RIGHT_COLUMN_ATTRIBUTES"]
          M_CONTENT
        [/m-grid-col]
        [m-grid-col attributes="M_LEFT_COLUMN_ATTRIBUTES"]
          [m-tag tag="div" image="M_IMAGE" image-path="M_PATH" attributes="class:M_BOX_SIZE image-cover"][/m-tag]
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  D_NO_VERTICAL_ALIGNMENT

  [m-component component="right-background-picture-with-text" folder="images-and-text" M_IMAGE="image.jpg" M_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-medium box-bg-secondary text-full-white"  M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-left-right-medium"]
    ### Lorem ipsum dolor
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
  [/m-component]

  [m-tag tag="div" attributes="id:code-no-vertical-align"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_IMAGE: The image name with the extension. Set a blank value for no image
      M_PATH: The image directory
      M_BOX_SIZE: Defines the size for all the item's boxes. This property accepts the following values:box-ultra-tiny, box-tiny, box-small, box-medium, box-large, box-huge
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="right-background-picture-with-text" folder="images-and-text" M_IMAGE="image.jpg" M_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-medium box-bg-secondary text-full-white"  M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-left-right-medium"]
      ### Lorem ipsum dolor
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-component]
    ```
    [/raw]
  [/m-tag]

  [m-clipboard target-id="code-no-vertical-align" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]  

  D_CELL_COLOR

  [m-component component="right-background-picture-with-text" folder="images-and-text" M_IMAGE="image.jpg" M_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-medium box-bg-primary text-full-white l-vertical-align"  M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
    [m-tag tag="div" attributes="class:padding-left-right-medium"]
      ### Lorem ipsum dolor
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-tag]
  [/m-component]

  [m-tag tag="div" attributes="id:code-cell-color"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_IMAGE: The image name with the extension. Set a blank value for no image
      M_PATH: The image directory
      M_BOX_SIZE: Defines the size for all the item's boxes. This property accepts the following values:box-ultra-tiny, box-tiny, box-small, box-medium, box-large, box-huge
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="right-background-picture-with-text" folder="images-and-text" M_IMAGE="image.jpg" M_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-medium box-bg-primary text-full-white l-vertical-align"  M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
      [m-tag tag="div" attributes="class:padding-left-right-medium"]
        ### Lorem ipsum dolor
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-tag]
    [/m-component]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code-cell-color" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
