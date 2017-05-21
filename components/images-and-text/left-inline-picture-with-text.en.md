[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Left inline picture with text" component (PRO)
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="left-inline-picture-with-text" folder="images-and-text" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="" M_IMAGE_ALT="Image alt" M_IMAGE_TITLE="Image title" M_IMAGE_CLASSES="responsive-img"  M_IMAGE_ACTIONS="" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white l-vertical-align" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
    [m-tag tag="div" attributes="class:padding-left-right-medium"]
      ### Lorem ipsum dolor
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet
    [/m-tag]
  [/m-component]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_IMAGE_NAME: The full image path
      M_IMAGE_PATH: The image directory
      M_IMAGE_ALT: The image alt attribute. This parameter is mandatory and cannot be blank
      M_IMAGE_TITLE: The image title attribute
      M_IMAGE_CLASSES: CSS classes added to the image
      M_IMAGE_ACTIONS: Grav image actions added to the image. Action and values are separated by a colon and properties are separated by a semicolon. Example="lightbox:600,800;resize:200,200"
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="left-inline-picture-with-text" folder="images-and-text" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="" M_IMAGE_ALT="Image alt" M_IMAGE_TITLE="Image title" M_IMAGE_CLASSES="responsive-img"  M_IMAGE_ACTIONS="" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white l-vertical-align" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
      [m-tag tag="div" attributes="class:padding-left-right-medium"]
        ### Lorem ipsum dolor
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet
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
        [m-grid-col attributes="M_LEFT_COLUMN_ATTRIBUTES"]![M_ALT](M_IMAGE "M_TITLE") {.responsive-img}[/m-grid-col]
        [m-grid-col attributes="M_RIGHT_COLUMN_ATTRIBUTES"]
          M_CONTENT
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  D_NO_VERTICAL_ALIGNMENT

  [m-component component="left-inline-picture-with-text" folder="images-and-text" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="" M_IMAGE_ALT="Image alt" M_IMAGE_TITLE="Image title" M_IMAGE_CLASSES="responsive-img"  M_IMAGE_ACTIONS="" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
    ### Lorem ipsum dolor
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet
  [/m-component]  

  [m-tag tag="div" attributes="id:code-no-vertical-align"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_IMAGE_NAME: The full image path
      M_IMAGE_PATH: The image directory
      M_IMAGE_ALT: The image alt attribute. This parameter is mandatory and cannot be blank
      M_IMAGE_TITLE: The image title attribute
      M_IMAGE_CLASSES: CSS classes added to the image
      M_IMAGE_ACTIONS: Grav image actions added to the image. Action and values are separated by a colon and properties are separated by a semicolon. Example="lightbox:600,800;resize:200,200"
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="left-inline-picture-with-text" folder="images-and-text" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="" M_IMAGE_ALT="Image alt" M_IMAGE_TITLE="Image title" M_IMAGE_CLASSES="responsive-img"  M_IMAGE_ACTIONS="" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
      ### Lorem ipsum dolor
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet
    [/m-component]  
    ```
    [/raw]
  [/m-tag]

  [m-clipboard target-id="code-no-vertical-align" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]  

  D_CELL_COLOR

  [m-component component="left-inline-picture-with-text" folder="images-and-text" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="" M_IMAGE_ALT="Image alt" M_IMAGE_TITLE="Image title" M_IMAGE_CLASSES="responsive-img"  M_IMAGE_ACTIONS="" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-primary text-full-white l-vertical-align" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
    [m-tag tag="div" attributes="class:padding-left-right-medium"]
      ### Lorem ipsum dolor
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet
    [/m-tag]
  [/m-component]

  [m-tag tag="div" attributes="id:code-cell-color"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_IMAGE_NAME: The full image path
      M_IMAGE_PATH: The image directory
      M_IMAGE_ALT: The image alt attribute. This parameter is mandatory and cannot be blank
      M_IMAGE_TITLE: The image title attribute
      M_IMAGE_CLASSES: CSS classes added to the image
      M_IMAGE_ACTIONS: Grav image actions added to the image. Action and values are separated by a colon and properties are separated by a semicolon. Example="lightbox:600,800;resize:200,200"
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="left-inline-picture-with-text" folder="images-and-text" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="" M_IMAGE_ALT="Image alt" M_IMAGE_TITLE="Image title" M_IMAGE_CLASSES="responsive-img"  M_IMAGE_ACTIONS="" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-primary text-full-white l-vertical-align" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
      [m-tag tag="div" attributes="class:padding-left-right-medium"]
        ### Lorem ipsum dolor
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet
      [/m-tag]
    [/m-component]
    ```
    [/raw]
  [/m-tag]

  [m-clipboard target-id="code-cell-color" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
