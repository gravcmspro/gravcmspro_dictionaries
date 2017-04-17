[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Jumbotron" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

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
