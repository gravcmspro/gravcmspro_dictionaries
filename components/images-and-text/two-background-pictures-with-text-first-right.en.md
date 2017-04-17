[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Two background pictures with text first left" component
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-help]
    Main component properties
    M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
    Item component properties
    M_IMAGE_NAME: The image name with the extension. Set a blank value for no image
    M_IMAGE_PATH: The image directory
    M_BOX_SIZE: Defines the size for all the item's boxes. This property accepts the following values:box-ultra-tiny, box-tiny, box-small, box-medium, box-large, box-huge
    M_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar
    M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
    M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
    M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
  [/m-help]
  [m-component component="two-background-pictures-with-text-first-right" folder="images-and-text" M_ATTRIBUTES=""]
    [m-component-item name="M_ITEM_1" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white l-vertical-align flex-s" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 box-inverted"]
      [m-tag tag="div" attributes="class:padding-left-right-large"]
        ### Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-tag]
    [/m-component-item]
    [m-component-item name="M_ITEM_2" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white l-vertical-align" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
      [m-tag tag="div" attributes="class:padding-left-right-large"]
        ### Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-tag]
    [/m-component-item]
  [/m-component]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      Item component properties
      M_IMAGE_NAME: The image name with the extension. Set a blank value for no image
      M_IMAGE_PATH: The image directory
      M_BOX_SIZE: Defines the size for all the item's boxes. This property accepts the following values:box-ultra-tiny, box-tiny, box-small, box-medium, box-large, box-huge
      M_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="two-background-pictures-with-text-first-right" folder="images-and-text" M_ATTRIBUTES=""]
      [m-component-item name="M_ITEM_1" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white l-vertical-align flex-s" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 box-inverted"]
        [m-tag tag="div" attributes="class:padding-left-right-large"]
          ### Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-tag]
      [/m-component-item]
      [m-component-item name="M_ITEM_2" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white l-vertical-align" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6"]
        [m-tag tag="div" attributes="class:padding-left-right-large"]
          ### Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-tag]
      [/m-component-item]
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
      [m-grid-row attributes="M_ITEM_1.M_ROW_ATTRIBUTES"]
        [m-grid-col attributes="M_ITEM_1.M_RIGHT_COLUMN_ATTRIBUTES"]
          M_ITEM_1.M_CONTENT
        [/m-grid-col]
        [m-grid-col attributes="M_ITEM_1.M_LEFT_COLUMN_ATTRIBUTES"]
          [m-tag tag="div" image="M_ITEM_1.M_IMAGE_NAME" image-path="M_ITEM_1.M_IMAGE_PATH" attributes="class:M_ITEM_1.M_BOX_SIZE image-cover"][/m-tag]
        [/m-grid-col]
      [/m-grid-row]
      [m-grid-row attributes="M_ITEM_2.M_ROW_ATTRIBUTES"]
        [m-grid-col attributes="M_ITEM_2.M_LEFT_COLUMN_ATTRIBUTES"]
          [m-tag tag="div" image="M_ITEM_2.M_IMAGE_NAME" image-path="M_ITEM_2.M_IMAGE_PATH" attributes="class:M_ITEM_2.M_BOX_SIZE image-cover"][/m-tag]
        [/m-grid-col]
        [m-grid-col attributes="M_ITEM_2.M_RIGHT_COLUMN_ATTRIBUTES"]
          M_ITEM_2.M_CONTENT
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  D_NO_VERTICAL_ALIGNMENT

  [m-component component="two-background-pictures-with-text-first-right" folder="images-and-text" M_ATTRIBUTES=""]
    [m-component-item name="M_ITEM_1" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white flex-s" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-medium box-inverted"]
      ### Title
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-component-item]
    [m-component-item name="M_ITEM_2" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-medium"]
      ### Title
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-component-item]
  [/m-component]  

  [m-tag tag="div" attributes="id:code-no-vertical-align"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar
      Item component properties
      M_IMAGE_NAME: The full image path
      M_IMAGE_PATH: The image directory
      M_IMAGE_ALT: The image alt attribute. This parameter is mandatory and cannot be blank
      M_IMAGE_TITLE: The image title attribute
      M_IMAGE_CLASSES: CSS classes added to the image
      M_IMAGE_ACTIONS: Grav image actions added to the image. Action and values are separated by a colon and properties are separated by a semi-colon. Example="lightbox:600,800;resize:200,200"
      M_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="two-background-pictures-with-text-first-right" folder="images-and-text" M_ATTRIBUTES=""]
      [m-component-item name="M_ITEM_1" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white flex-s" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-medium box-inverted"]
        ### Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-component-item]
      [m-component-item name="M_ITEM_2" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-secondary text-full-white" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-medium"]
        ### Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-component-item]
    [/m-component]   
    ```
    [/raw]
  [/m-tag]

  [m-clipboard target-id="code-no-vertical-align" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]  

  D_CELL_COLOR

  [m-component component="two-background-pictures-with-text-first-right" folder="images-and-text" M_ATTRIBUTES=""]
    [m-component-item name="M_ITEM_1" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-primary text-full-white flex-s" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-medium box-inverted"]
      ### Title
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-component-item]
    [m-component-item name="M_ITEM_2" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-primary text-full-white" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-medium"]
      ### Title
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-component-item]
  [/m-component]  

  [m-tag tag="div" attributes="id:code-cell-color"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar
      Item component properties
      M_IMAGE_NAME: The full image path
      M_IMAGE_PATH: The image directory
      M_IMAGE_ALT: The image alt attribute. This parameter is mandatory and cannot be blank
      M_IMAGE_TITLE: The image title attribute
      M_IMAGE_CLASSES: CSS classes added to the image
      M_IMAGE_ACTIONS: Grav image actions added to the image. Action and values are separated by a colon and properties are separated by a semi-colon. Example="lightbox:600,800;resize:200,200"
      M_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
      M_LEFT_COLUMN_ATTRIBUTES: Adds html attributes to the left grid column
      M_RIGHT_COLUMN_ATTRIBUTES: Adds html attributes to the right grid column
    [/m-help]
    [m-component component="two-background-pictures-with-text-first-right" folder="images-and-text" M_ATTRIBUTES=""]
      [m-component-item name="M_ITEM_1" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-primary text-full-white flex-s" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-medium box-inverted"]
        ### Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-component-item]
      [m-component-item name="M_ITEM_2" M_IMAGE_NAME="image.jpg" M_IMAGE_PATH="/images" M_BOX_SIZE="box-medium" M_ATTRIBUTES="" M_ROW_ATTRIBUTES="class:box-bg-primary text-full-white" M_LEFT_COLUMN_ATTRIBUTES="class: s12 m12 l6 no-padding no-line-height"  M_RIGHT_COLUMN_ATTRIBUTES="class: s12 m12 l6 padding-medium"]
        ### Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-component-item]
    [/m-component]
    ```
    [/raw]
  [/m-tag]

  [m-clipboard target-id="code-cell-color" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
