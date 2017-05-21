[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "3 full boxed images" component (PRO)
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="3-full-boxed-images" folder="boxed-images" M_COLUMNS="s12 m12 l4" M_IMAGE_SIZE="box-medium" M_IMAGE_SCALE="true" M_ATTRIBUTES="" M_ROW_ATTRIBUTES=""]
    [m-component-item name="M_BOX_1" M_IMAGE_SRC="image.jpg"]
        #### Lorem ipsum
    [/m-component-item]
    [m-component-item name="M_BOX_2" M_IMAGE_SRC="image.jpg"]
        #### Lorem ipsum
    [/m-component-item]
    [m-component-item name="M_BOX_3" M_IMAGE_SRC="image.jpg"]
        #### Lorem ipsum
    [/m-component-item]
  [/m-component]

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_COLUMNS: Defines the size for all the item's columns
      M_IMAGE_SIZE: Defines the size for all the images
      M_IMAGE_SCALE: Scales the image when the cursor is placed hover it

      Item component properties
      M_IMAGE_SRC: The image name with the extension. Set a blank value for no image
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_ROW_ATTRIBUTES: Adds html attributes to the item's grid row
    [/m-help]
    [m-component component="3-full-boxed-images" folder="boxed-images" M_COLUMNS="s12 m12 l4" M_IMAGE_SIZE="box-medium" M_IMAGE_SCALE="true" M_ATTRIBUTES="" M_ROW_ATTRIBUTES=""]
      [m-component-item name="M_BOX_1" M_IMAGE_SRC="image.jpg"]
          #### Lorem ipsum
      [/m-component-item]
      [m-component-item name="M_BOX_2" M_IMAGE_SRC="image.jpg"]
          #### Lorem ipsum
      [/m-component-item]
      [m-component-item name="M_BOX_3" M_IMAGE_SRC="image.jpg"]
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
    [m-grid container="false" attributes="M_ATTRIBUTES"]
      [m-grid-row attributes="M_ROW_ATTRIBUTES"]
        [m-grid-col attributes="class:M_COLUMNS no-padding"]
          [m-rich-image container-attributes="class:M_IMAGE_SIZE" content-attributes="class:text-white center" image-attributes="class:image-cover" image="M_BOX_1.M_IMAGE_SRC" scale="M_IMAGE_SCALE" url="M_BOX_1.M_URL"]
            M_BOX_1.M_CONTENT
          [/m-rich-image]
        [/m-grid-col]
        [m-grid-col attributes="class:M_COLUMNS no-padding"]
          [m-rich-image container-attributes="class:M_IMAGE_SIZE" content-attributes="class:text-white center" image-attributes="class:image-cover" image="M_BOX_2.M_IMAGE_SRC" scale="M_IMAGE_SCALE" url="M_BOX_2.M_URL"]
            M_BOX_2.M_CONTENT
          [/m-rich-image]
        [/m-grid-col]
        [m-grid-col attributes="class:M_COLUMNS no-padding"]
          [m-rich-image container-attributes="class:M_IMAGE_SIZE" content-attributes="class:text-white center" image-attributes="class:image-cover" image="M_BOX_3.M_IMAGE_SRC" scale="M_IMAGE_SCALE" url="M_BOX_3.M_URL"]
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
