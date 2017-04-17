[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Rich image" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l6"]
        [m-rich-image container-attributes="class:box-medium" content-attributes="class:text-white center" image="image.jpg" scale="true" image-attributes="class:image-cover"]
          #### Lorem ipsum
        [/m-rich-image]  
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  D_CODE

  [m-tag tag="div" attributes="id:material-code"]
    [raw]
    ```
    [m-help]
      Main component properties
      image: The image name with the extension. Set a blank value for no image
      image-path: The image directory
      image-attributes: Adds html attributes to image element. Example attributes="class: foo, rel=bar"
      content-attributes: Adds html attributes to the div that contains the content. Example attributes="class: foo, rel=bar"
      container-attributes: Adds html attributes to container element. Example container_attributes="class: foo, rel=bar"
      scale: When true the image scales to big, when the mouse cursor is placed over it
      url: The url of the page to go to. When you valorize this property, pay attention to not add another link in the content, otherwise the element is not properly rendered.
    [/m-help]
    [m-rich-image container-attributes="class:box-small" content-attributes="class:text-white center" image="home.jpg" scale="true"]
      #### Lorem ipsum
    [/m-rich-image]    
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="material-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
