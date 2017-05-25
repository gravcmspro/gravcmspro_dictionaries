[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Parallax" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

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

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      image: The image name with the extension. Set a blank value for no image
      image-path: The image directory
      blurred-image: Defines the blurred images name with the extension, which takes place of main one when user scrolls down the page. Set a blank value for no image
      height: Defines the jumbotrn height. This property accepts the following values: 'full, three-quarters, half'
      background-attached: When true sets the background as attached
    [/m-help]
    [m-jumbotron image="image.jpg" blurred-image="image_blurred.jpg" height="full"  attributes="class: vertical-align"]
      [m-grid]
        [m-grid-row]
          [m-grid-col attributes="class: s12 m12 l12 text-white"]
            ### Title
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
          [/m-grid-col]
        [/m-grid-row]
      [/m-grid]
    [/m-jumbotron]    
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
