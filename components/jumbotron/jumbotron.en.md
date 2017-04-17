[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Jumbotron" component
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="jumbotron" folder="jumbotron" M_IMAGE="image.jpg" M_IMAGE_BLURRED="image-blurred.jpg" M_PATH="images" M_HEIGHT="full" M_ATTRIBUTES="class:l10 offset-l1 m12 s12 opaque-panel-shades-black-low rounded text-full-white center padding-medium"]
    ### Anim pariatur cliche reprehenderit
    Anim pariatur cliche reprehenderit enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch.
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
    [m-component component="jumbotron" folder="jumbotron" M_IMAGE="image.jpg" M_IMAGE_BLURRED="image-blurred.jpg" M_PATH="images" M_HEIGHT="full" M_ATTRIBUTES="class:l10 offset-l1 m12 s12 opaque-panel-shades-black-low rounded text-full-white center padding-medium"]
      ### Anim pariatur cliche reprehenderit
      Anim pariatur cliche reprehenderit enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch.
    [/m-component]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  D_THE_CODE_COMPONENT

  [m-tag tag="div" attributes="id:component-code"]
    [raw]
    ```
    [m-jumbotron image-path="M_PATH" image="M_IMAGE" blurred-image="M_BLURRED_IMAGE" height="M_HEIGHT" background-attached="M_BACKGROUND_ATTACHED" attributes="class:vertical-align"]
      [m-grid container="M_CONTAINER"]
        [m-grid-row]
          [m-grid-col attributes="M_ATTRIBUTES"]
            M_CONTENT
          [/m-grid-col]
        [/m-grid-row]
        [m-grid-row attributes="class:hide-on-med-and-down"]
          [m-grid-col attributes="class:s12 m12 l12"]
            [m-tag tag="div" attributes="class:jumbotron-scrolldown" ignore-items="true"]
              [m-link url="#main" link-attributes="class:smoothscroll" icon="keyboard_arrow_down"][/m-link]
            [/m-tag]
          [/m-grid-col]
        [/m-grid-row]
      [/m-grid]
    [/m-jumbotron]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
