[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Scroll to top button" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  Renderes a nice button on the bottom right corner of the page, which appears when the page is scrolled down.

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-scroll-to-top][/m-scroll-to-top]        
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
