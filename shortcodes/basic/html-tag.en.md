[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Html tag" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  This shortcode renders an arbitrary html tag.

  [m-tag tag="div"]
    ### Title
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
  [/m-tag]  

  D_CODE

  [m-tag tag="div" attributes="id:material-code"]
    [raw]
    ```
    [m-help]
      Main component properties
      tag: the html tag to display. Accepts all html tags. Example tag="div"
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      image: The image name with the extension. Set a blank value for no image
      image-path: The image directory
    [/m-help]
    [m-tag tag="div"]
      ### Title
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-tag]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="material-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
