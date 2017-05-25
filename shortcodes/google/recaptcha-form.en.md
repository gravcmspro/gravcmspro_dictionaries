[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Recaptcha form" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-recaptcha-form site-key="xxxxxxxxxxxxxxxxxxx" site-secret="xxxxxxxxxxxx"]
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
  [/m-recaptcha-form]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
      [m-help]
      action: The form action
      name-placeholder: Defines the name placeholder
      mail-placeholder: Defines the mail placeholder
      submit-text: Defines the text for the submit button
      site-key: The site key value got from Google's recaptcha service
      site-secret: The site secret key value got from Google's recaptcha service
      [/m-help]
      [m-recaptcha-form site-key="xxxxxxxxxxxxxxxxxxx" site-secret="xxxxxxxxxxxx"]
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-recaptcha-form]    
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

[/m-dictionary-item]
