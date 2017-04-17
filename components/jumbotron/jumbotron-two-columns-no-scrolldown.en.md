[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Jumbotron two columns no scrolldown" component
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="jumbotron-two-columns-no-scrolldown" folder="jumbotron" M_NAME="jumbotron" M_IMAGE="image.jpg" M_IMAGE_BLURRED="image-blurred.jpg" M_PATH="images" M_HEIGHT="full"]
    [m-component-item name="M_HEADER_LEFT" M_ATTRIBUTES="class:offset-l1 l6 m6 s12 margin-top-large"]
      ### Lorem ipsum dolor sit amet{.h1-size}
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
      [m-link url="http://example.com" menu="Learn more" icon="code" icon-attributes="class:left" link-attributes="class:btn"][/m-link]
    [/m-component-item]]
    [m-component-item name="M_HEADER_RIGHT" M_ATTRIBUTES="class:l4 m4 s12 margin-top-large opaque-panel-shades-black-low rounded text-full-white padding-medium"]
      #### Sed ut perspiciati
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
      [m-link url="http://example.com" menu="Learn more" icon="code" icon-attributes="class:left" link-attributes="class:btn"][/m-link]
    [/m-component-item]
  [/m-component]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_CONTAINER: When true contains and centers the component grid
      M_IMAGE: The image name with the extension. Set a blank value for no image
      M_IMAGE_BLURRED: Defines the blurred images name with the extension, which takes place of main one when user scrolls down the page. Set a blank value for no image
      M_PATH: The image directory
      M_HEIGHT: Defines the jumbotrn height. This property accepts the following values: 'full, three-quarters, half'
      M_BACKGROUND_ATTACHED: When true sets the background as attached
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-component component="jumbotron-two-columns-no-scrolldown" folder="jumbotron" M_NAME="jumbotron" M_IMAGE="image.jpg" M_IMAGE_BLURRED="image-blurred.jpg" M_PATH="images" M_HEIGHT="full"]
      [m-component-item name="M_HEADER_LEFT" M_ATTRIBUTES="class:offset-l1 l6 m6 s12 margin-top-large"]
        ### Lorem ipsum dolor sit amet{.h1-size}
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
        [m-link url="http://example.com" menu="Learn more" icon="code" icon-attributes="class:left" link-attributes="class:btn"][/m-link]
      [/m-component-item]]
      [m-component-item name="M_HEADER_RIGHT" M_ATTRIBUTES="class:l4 m4 s12 margin-top-large opaque-panel-shades-black-low rounded text-full-white padding-medium"]
        #### Sed ut perspiciati
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
        [m-link url="http://example.com" menu="Learn more" icon="code" icon-attributes="class:left" link-attributes="class:btn"][/m-link]
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
    [m-jumbotron image="M_IMAGE" image-path="M_PATH" blurred-image="M_BLURRED_IMAGE" render="M_RENDER" height="M_HEIGHT" background-attached="M_BACKGROUND_ATTACHED" attributes="class:vertical-align"]
      [m-grid container="M_CONTAINER"]
        [m-grid-row attributes="class:m-vertical-align"]
          [m-grid-col attributes="M_HEADER_LEFT.M_ATTRIBUTES"]
            M_HEADER_LEFT.M_CONTENT
          [/m-grid-col]
          [m-grid-col attributes="M_HEADER_RIGHT.M_ATTRIBUTES"]
            M_HEADER_RIGHT.M_CONTENT
          [/m-grid-col]
        [/m-grid-row]
      [/m-grid]
    [/m-jumbotron]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
