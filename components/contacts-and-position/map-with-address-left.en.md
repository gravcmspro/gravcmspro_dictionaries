[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Map with address left" component
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="map-with-address-left" folder="contacts-and-position" M_CONTAINER="false"]
    [m-component-item name="M_INCIPIT" M_COLUMNS="s12 m12 l12" M_CENTER="center" M_EXTRA_ATTRIBUTES=""]
      ### Come and find us
      ---
      Anim pariatur cliche reprehenderit enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch.
    [/m-component-item]
    [m-component-item name="M_ADDRESS" M_COLUMNS="s12 m12 l4"]
    Company Name  
    lorem ipsum  
    12345  
    Lorem ipsum  
    Telephone: 555-555555  
    Fax: 555-556666  
  [/m-component-item]
    [m-component-item name="M_MAP" M_COLUMNS="s12 m12 l8" M_API_KEY="999999999-999999999" M_ZOOM="10" M_POINT_CENTER="41.895639,12.493415" M_POINT_LOCATION="41.895639,12.493415" M_TITLE="Marker title"]
      Add a content for the marker
    [/m-component-item]
  [/m-component]
  
  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_CONTAINER: When true contains and centers the component grid

      Item component properties
      M_COLUMNS: Defines the size for all the item's columns
      M_CENTER: Sets the text alignment. This parameter accepts the following values: left, center, right
      M_EXTRA_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar

      Recaptcha form component properties
      M_SITE_KEY: Site key provided by Google
      M_SITE_SECRET: Site secret key provided by Google
      M_NAME_PLACEHOLDER: Name field placeholder
      M_MAIL_PLACEHOLDER: Email field placeholder
      M_SUBMIT_TEXT: The submit button text
    [/m-help]
    [m-component component="contact-form-with-address-left" folder="contacts-and-position" M_CONTAINER="true"]
      [m-component-item name="M_INCIPIT" M_COLUMNS="s12 m12 l12" M_CENTER="center" M_EXTRA_ATTRIBUTES=""]
        ### Get in touch with us [m-link link-attributes="name:contact-up,class: opaque opaque-reveal" icon="fa-link fa-flip-horizontal"][/m-link]
        ---
        Anim pariatur cliche reprehenderit enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch.
      [/m-component-item]
      [m-component-item name="M_ADDRESS" M_COLUMNS="s12 m12 l4"]
      Company Name  
      lorem ipsum  
      12345  
      Lorem ipsum  
      Telephone: 555-555555  
      Fax: 555-556666  
    [/m-component-item]
      [m-component-item name="M_FORM" M_COLUMNS="s12 m12 l8" M_SITE_KEY="999999999" M_SITE_SECRET="999999999" M_NAME_PLACEHOLDER="Please insert your name here" M_MAIL_PLACEHOLDER="Please insert a valid email address here" M_SUBMIT_TEXT="Send"]
        Add here and optional precompiled text or leave it blank
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
    [m-grid container="M_CONTAINER" attributes="M_ATTRIBUTES"]
      [m-grid-row]
        [m-grid-col attributes="class:M_INCIPIT.M_COLUMNS M_INCIPIT.M_CENTER M_INCIPIT.M_EXTRA_ATTRIBUTES"]
          M_INCIPIT.M_CONTENT
        [/m-grid-col]
      [/m-grid-row]

      [m-grid-row]
        [m-grid-col attributes="class:M_ADDRESS.M_COLUMNS"]
          M_ADDRESS.M_CONTENT
        [/m-grid-col]

        [m-grid-col attributes="class:M_MAP.M_COLUMNS"]
          [m-google-map id="M_MAP.M_ID" zoom="M_MAP.M_ZOOM" center="M_MAP.M_POINT_CENTER" api-key="M_MAP.M_API_KEY"]
            [m-google-map-marker location="M_MAP.M_POINT_LOCATION" title="M_MAP.M_TITLE"]
              M_MAP.M_CONTENT
            [/m-google-map-marker]
          [/m-google-map]
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
