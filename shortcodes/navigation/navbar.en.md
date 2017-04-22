[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Navbar" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  Renderes the website menu parsing site pages.

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l12"]
        [m-navbar brand-name="ACME ltd." sidebar-id="nav-mobile-id" extended="true"]
          [m-menu template="menu/menu" alignment="right" sidebar-id="nav-mobile"][/m-menu]
        [/m-navbar]         
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties

      sidebar-id: defines the id of the sidebar opened for small screens
      transparent: renders the navbar transparent for the given menu pages, comma separated or for the whole pages, when the "all" param is given. Usage navbar-transparent="all" or transparent="menu page1,menu page2,menu page3"
      brand-url: Defines the brand element url. When empty link to website homepage
      brand-link-attributes: adds html attributes to brand link. Example attributes="class: foo, rel=bar"
      brand-image: defines the brand image
      brand-image-attributes: adds html attributes to element. Example attributes="class: foo, rel=bar". This property works only when brand_image property is defined
      brand-image-path: defines the brand image path
      brand-name: defines the brand as a text
      brand-icon: defines an icon placed an the left of the brand
      brand-align: defines the brand alignment. It accepts the left, center or right values

      By default the navbar shortcode just requires the m-menu shortcode to render the site navigation menu. Optionally, it accepts the m-navbar-item, to render complex navbars. See components section to
      Here it is an example:
      [m-navbar-item attributes="class:navbar-top-content"]
        [m-grid container="false"]
          [m-grid-row]
            [m-grid-col attributes="class:s12 m6 l6"]
              Call us today: 555.555.555555 | info@yourdomain.com
            [/m-grid-col]
            [m-grid-col attributes="class:s12 m6 l6 right-align"]
              [m-tag tag="ul" attributes="class:right padding-left-small"]
                [m-tag tag="li"][m-icon icon="fa-facebook-official"][/m-icon][/m-tag]
                [m-tag tag="li"][m-icon icon="fa-twitter"][/m-icon][/m-tag]
                [m-tag tag="li"][m-icon icon="fa-google-plus"][/m-icon][/m-tag]
              [/m-tag]
            [/m-grid-col]
          [/m-grid-row]
        [/m-grid]
      [/m-navbar-item]
      [m-navbar-item type="menu"]
        [m-menu name="menu0" template="menu/menu" alignment="right" sidebar-id="nav-mobile" submenu="centre,documentation"][/m-menu]
      [/m-navbar-item]
      Do not forget to specify the type="menu" property for the item that handles the navigation menu
    [/m-help]
    [m-navbar name="navbar" brand-name="ACME ltd." transparent="all" sidebar-id="nav-mobile"]
      [m-menu template="menu/menu" alignment="right" sidebar-id="nav-mobile"][/m-menu]
    [/m-navbar]    
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  ## Navbar items
  Navbar can be riched using navbar item. Here we used two items, the first one to render both company address and social buttons and the second one to render the company logo and the site navigation menu.

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l12"]
        [m-navbar brand-url="#" brand-name="ACME ltd." sidebar-id="nav-mobile"]
          [m-navbar-item attributes="class:navbar-top-content"]
            [m-grid container="false"]
              [m-grid-row attributes="class:padding-left-right-small"]
                [m-grid-col attributes="class:s12 m6 l6"]
                  Call us today: 555.555.555555 | info@yourdomain.com
                [/m-grid-col]
                [m-grid-col attributes="class:s12 m6 l6 right-align"]
                  [m-tag tag="ul" attributes="class:right padding-left-small"]
                    [m-tag tag="li"][m-icon icon="fa-facebook-official"][/m-icon][/m-tag]
                    [m-tag tag="li"][m-icon icon="fa-twitter"][/m-icon][/m-tag]
                    [m-tag tag="li"][m-icon icon="fa-google-plus"][/m-icon][/m-tag]
                  [/m-tag]          
                [/m-grid-col]
              [/m-grid-row]
            [/m-grid]
          [/m-navbar-item]

          [m-navbar-item type="menu"]
            [m-menu name="menu0" template="menu/menu" alignment="right" sidebar-id="nav-mobile" submenu="centre,documentation"][/m-menu]
          [/m-navbar-item]
        [/m-navbar]
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]

  > When using navbar items, do not forget to tell the shortcode which is the item that handles the navigation menu, defining the **type="menu"** property.

  D_CODE

  [m-tag tag="div" attributes="id:navbar_items_code"]
    [raw]
    ```
    [m-help]
      Main component properties

      sidebar-id: defines the id of the sidebar opened for small screens
      transparent: renders the navbar transparent for the given menu pages, comma separated or for the whole pages, when the "all" param is given. Usage navbar-transparent="all" or transparent="menu page1,menu page2,menu page3"
      brand-url: Defines the brand element url. When empty link to website homepage
      brand-link-attributes: adds html attributes to brand link. Example attributes="class: foo, rel=bar"
      brand-image: defines the brand image
      brand-image-attributes: adds html attributes to element. Example attributes="class: foo, rel=bar". This property works only when brand_image property is defined
      brand-image-path: defines the brand image path
      brand-name: defines the brand as a text
      brand-icon: defines an icon placed an the left of the brand
      brand-align: defines the brand alignment. It accepts the left, center or right values

      By default the navbar shortcode just requires the m-menu shortcode to render the site navigation menu. Optionally, it accepts the m-navbar-item, to render complex navbars. See components section to
      Here it is an example:
      [m-navbar-item attributes="class:navbar-top-content"]
        [m-grid container="false"]
          [m-grid-row]
            [m-grid-col attributes="class:s12 m6 l6"]
              Call us today: 555.555.555555 | info@yourdomain.com
            [/m-grid-col]
            [m-grid-col attributes="class:s12 m6 l6 right-align"]
              [m-tag tag="ul" attributes="class:right padding-left-small"]
                [m-tag tag="li"][m-icon icon="fa-facebook-official"][/m-icon][/m-tag]
                [m-tag tag="li"][m-icon icon="fa-twitter"][/m-icon][/m-tag]
                [m-tag tag="li"][m-icon icon="fa-google-plus"][/m-icon][/m-tag]
              [/m-tag]
            [/m-grid-col]
          [/m-grid-row]
        [/m-grid]
      [/m-navbar-item]
      [m-navbar-item type="menu"]
        [m-menu name="menu0" template="menu/menu" alignment="right" sidebar-id="nav-mobile" submenu="centre,documentation"][/m-menu]
      [/m-navbar-item]
      Do not forget to specify the type="menu" property for the item that handles the navigation menu
    [/m-help]
    [m-navbar brand-url="#" brand-name="ACME ltd." sidebar-id="nav-mobile"]
      [m-navbar-item attributes="class:navbar-top-content"]
        [m-grid container="false"]
          [m-grid-row]
            [m-grid-col attributes="class:s12 m6 l6"]
              Call us today: 555.555.555555 | info@yourdomain.com
            [/m-grid-col]
            [m-grid-col attributes="class:s12 m6 l6 right-align"]
              [m-tag tag="ul" attributes="class:right padding-left-small"]
                [m-tag tag="li"][m-icon icon="fa-check"][/m-icon][/m-tag]
                [m-tag tag="li"][m-icon icon="fa-check"][/m-icon][/m-tag]
                [m-tag tag="li"][m-icon icon="fa-check"][/m-icon][/m-tag]
              [/m-tag]          
            [/m-grid-col]
          [/m-grid-row]
        [/m-grid]
      [/m-navbar-item]

      [m-navbar-item type="menu"]
        [m-menu name="menu0" template="menu/menu" alignment="right" sidebar-id="nav-mobile" submenu="centre,documentation"][/m-menu]
      [/m-navbar-item]
    [/m-navbar]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="navbar_items_code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

[/m-dictionary-item]
