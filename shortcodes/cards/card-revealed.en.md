[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Card revealed" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-card-revealed image="image.jpg"]
          ## Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
          [m-card-revealed-full-content]
            ## Title
            Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
          [/m-card-revealed-full-content]
          [m-card-action]
            [m-link url="#" menu="Action 1"][/m-link]
            [m-link url="#" menu="Action 2"][/m-link]
          [/m-card-action]
        [/m-card-revealed]        
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      image: The image name with the extension. Set a blank value for no image
      image-path: The image directory
      size: defines the card size. This parameters accepts "small, medium, large" values
      sticky: does not overly the action section. Usage: sticky="true"
      card-attributes: Adds html attributes to card element. Example card-attributes="class: blue-grey darken-1"
      content-attributes: Adds html attributes to the div that contains the content. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-card-revealed image="image.jpg"]
      ## Title
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [m-card-revealed-full-content]
        ## Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-card-revealed-full-content]
      [m-card-action]
        [m-link url="#" menu="Action 1"][/m-link]
        [m-link url="#" menu="Action 2"][/m-link]
      [/m-card-action]
    [/m-card-revealed]     
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
