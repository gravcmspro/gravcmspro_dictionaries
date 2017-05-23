[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Modular collection" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  This shortcode adds Google's analytics code to the website page. It requires a valid user id you will get from Google's services.

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
      [m-help]
        Main component properties
        user-id: The user id provided with Google's code
      [/m-help]
      [m-google-analytics user-id="xxxxxxxxx"][/m-google-analytics]      
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

[/m-dictionary-item]
