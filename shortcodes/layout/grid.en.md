[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Materializer Grid" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  D_GRID_SHORTCODE_DESCRIPTION
  
  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m6 l6"]
        ## Column 1
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m6 l6"]
        ## Column 2
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
     Grid shortcode represent a Materializer grid and always requires both a "m-grid-row" and "m-grid-col" shortcodes. Please notice the "m-grid-col" does not require the "col" class.
    m-grid shortcode properties:
      container: When true contains and centers the component grid
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"

    m-grid-row shortcode properties:
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"

    m-grid-col shortcode properties:
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-grid container="true"]
      [m-grid-row]
        [m-grid-col attributes="class:s12 m6 l6"]
          ## Column 1
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        [/m-grid-col]
        [m-grid-col attributes="class:s12 m6 l6"]
          ## Column 2
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]    
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
