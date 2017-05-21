[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Navbar with address and social buttons" component (PRO)
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="navbar-address-and-social" folder="navbar" M_FIXED="false" M_BRAND_NAME="ACME ltd." M_BRAND_ALIGN="left" M_BRAND_URL="#" M_BRAND_URL_ATTRIBUTES="" M_BRAND_IMAGE="" M_BRAND_IMAGE_ATTRIBUTES=""]
    [m-component-item name="M_ADDRESS_ITEM" M_ATTRIBUTES="class:s12 m6 l6 padding-left-small"]
      Call us today: 555.555.555555 | info@yourdomain.com
    [/m-component-item]
    [m-component-item name="M_SOCIAL_ITEM"  M_ATTRIBUTES="class:s12 m6 l6 padding-left-small"]
      [m-tag tag="ul" attributes="class:right"]
        [m-tag tag="li"][m-icon icon="fa-facebook-official"][/m-icon][/m-tag]
        [m-tag tag="li"][m-icon icon="fa-twitter"][/m-icon][/m-tag]
        [m-tag tag="li"][m-icon icon="fa-google-plus"][/m-icon][/m-tag]
      [/m-tag]
    [/m-component-item]
    [m-component-item name="M_MENU_ITEM" M_ATTRIBUTES="class:s12 m6 l6 padding-left-small"]
      [m-menu template="menu/menu" alignment="right" sidebar-id="nav-mobile" submenu="centre,documentation"][/m-menu]
    [/m-component-item]
  [/m-component]

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_FIXED: When true contains and centers the component grid
      M_BRAND_NAME: defines the brand as a text
      M_BRAND_ALIGN: defines the brand alignment. It accepts the left, center or right values
      M_BRAND_URL: Defines the brand element url. When empty link to website homepage
      M_BRAND_URL_ATTRIBUTES: adds html attributes to brand link. Example attributes="class: foo, rel=bar"
      M_BRAND_IMAGE: defines the brand image
      M_BRAND_IMAGE_ATTRIBUTES: adds html attributes to element. Example attributes="class: foo, rel=bar". This property works only when brand_image property is defined

    Item component properties
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-component component="navbar-address-and-social" folder="navbar" M_FIXED="false" M_BRAND_NAME="ACME ltd." M_BRAND_ALIGN="left" M_BRAND_URL="#" M_BRAND_URL_ATTRIBUTES="" M_BRAND_IMAGE="" M_BRAND_IMAGE_ATTRIBUTES=""]
      [m-component-item name="M_ADDRESS_ITEM" M_ATTRIBUTES="class:s12 m6 l6 padding-left-small"]
        Call us today: 555.555.555555 | info@yourdomain.com
      [/m-component-item]
      [m-component-item name="M_SOCIAL_ITEM"  M_ATTRIBUTES="class:s12 m6 l6 padding-left-small"]
        [m-tag tag="ul" attributes="class:right"]
          [m-tag tag="li"][m-icon icon="fa-facebook-official"][/m-icon][/m-tag]
          [m-tag tag="li"][m-icon icon="fa-twitter"][/m-icon][/m-tag]
          [m-tag tag="li"][m-icon icon="fa-google-plus"][/m-icon][/m-tag]
        [/m-tag]
      [/m-component-item]
      [m-component-item name="M_MENU_ITEM" M_ATTRIBUTES="class:s12 m6 l6 padding-left-small"]
        [m-menu template="menu/menu" alignment="right" sidebar-id="nav-mobile" submenu="centre,documentation"][/m-menu]
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
    [m-navbar fixed="M_FIXED" brand-name="M_BRAND_NAME" brand-url="M_BRAND_URL" brand-image="M_BRAND_IMAGE" brand-link-attributes="M_BRAND_URL_ATTRIBUTES" brand-image-attributes="M_BRAND_IMAGE_ATTRIBUTES" sidebar-id="nav-mobile"]
      [m-navbar-item attributes="class:navbar-top-content"]
        [m-grid container="false"]
          [m-grid-row]
            [m-grid-col attributes="M_ADDRESS_ITEM.M_ATTRIBUTES"]
              M_ADDRESS_ITEM.M_CONTENT
            [/m-grid-col]
            [m-grid-col attributes="class:s12 m6 l6 right-align"]
              M_SOCIAL_ITEM.M_CONTENT     
            [/m-grid-col]
          [/m-grid-row]
        [/m-grid]
      [/m-navbar-item]

      [m-navbar-item type="menu"]
        M_MENU_ITEM.M_CONTENT
      [/m-navbar-item]
    [/m-navbar]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
