[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "3 boxed images" component (PRO)
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="3-boxed-images" folder="boxed-images" M_CONTAINER="false" M_COLUMNS="s12 m12 l4" M_PADDING_COLUMN="small" M_IMAGE_SIZE="box-tiny" M_IMAGE_SCALE="true" M_ATTRIBUTES="" M_ROW_ATTRIBUTES=""]
    [m-component-item name="M_BOX_1" M_IMAGE_SRC="image.jpg" M_URL=""]
        #### Lorem ipsum
    [/m-component-item]
    [m-component-item name="M_BOX_2" M_IMAGE_SRC="image.jpg" M_URL=""]
        #### Lorem ipsum
    [/m-component-item]
    [m-component-item name="M_BOX_3" M_IMAGE_SRC="image.jpg" M_URL=""]
        #### Lorem ipsum
    [/m-component-item]
  [/m-component]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_CONTAINER: When true contains and centers the component grid
      M_COLUMNS: Defines the size for all the item's columns
      M_PADDING_COLUMN: Defined the columns padding
      M_IMAGE_SIZE: Defines the size for all the images
      M_IMAGE_SCALE: Scales the image when the cursor is placed hover it

      Item component properties
      M_IMAGE_SRC: The image name with the extension. Set a blank value for no image
      M_URL: The url to link the image. Leave it empty to leave the image unlinked
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
    [/m-help]
    [m-component component="3-boxed-images" folder="boxed-images" M_CONTAINER="true" M_COLUMNS="s12 m12 l4" M_PADDING_COLUMN="small" M_IMAGE_SIZE="box-tiny" M_IMAGE_SCALE="true" M_ATTRIBUTES="" M_ROW_ATTRIBUTES=""]
      [m-component-item name="M_BOX_1" M_IMAGE_SRC="image.jpg" M_URL=""]
          #### Lorem ipsum
      [/m-component-item]
      [m-component-item name="M_BOX_2" M_IMAGE_SRC="image.jpg" M_URL=""]
          #### Lorem ipsum
      [/m-component-item]
      [m-component-item name="M_BOX_3" M_IMAGE_SRC="image.jpg" M_URL=""]
          #### Lorem ipsum
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
    [m-grid container="M_CONTAINER" attributes="M_ATTRIBUTES"]
      [m-grid-row attributes="M_ROW_ATTRIBUTES"]
        [m-grid-col attributes="class:M_COLUMNS padding-M_PADDING_COLUMN"]
          [m-rich-image container-attributes="class:M_IMAGE_SIZE" content-attributes="class:text-white padding-small" image="M_BOX_1.M_IMAGE_SRC" image-attributes="class:image-cover" scale="M_IMAGE_SCALE" url="M_BOX_1.M_URL"]
            M_BOX_1.M_CONTENT
          [/m-rich-image]
        [/m-grid-col]
        [m-grid-col attributes="class:M_COLUMNS padding-M_PADDING_COLUMN"]
          [m-rich-image container-attributes="class:M_IMAGE_SIZE" content-attributes="class:text-white padding-small" image="M_BOX_2.M_IMAGE_SRC" image-attributes="class:image-cover" scale="M_IMAGE_SCALE" url="M_BOX_1.M_URL"]
            M_BOX_2.M_CONTENT
          [/m-rich-image]
        [/m-grid-col]
        [m-grid-col attributes="class:M_COLUMNS padding-M_PADDING_COLUMN"]
          [m-rich-image container-attributes="class:M_IMAGE_SIZE" content-attributes="class:text-white padding-small" image="M_BOX_3.M_IMAGE_SRC" image-attributes="class:image-cover" scale="M_IMAGE_SCALE" url="M_BOX_1.M_URL"]
            M_BOX_3.M_CONTENT
          [/m-rich-image]
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
