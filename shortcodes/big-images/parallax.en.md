[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Parallax" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
    D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      image: The image name with the extension. Set a blank value for no image
      image-path: The image directory
      image-title: The image title attribute
      image-alt: The image alt attribute. This parameter is mandatory and cannot be blank
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-parallax image="image.jpg" image-title="Title" image-alt="Alt"]
      [m-tag tag="div"]
        ### Lorem ipsum dolor sit amet, consectetur adipiscing elit
      [/m-tag]
    [/m-parallax]    
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
