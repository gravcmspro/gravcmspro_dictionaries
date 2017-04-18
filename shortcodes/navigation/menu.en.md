[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Menu" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  Renderes the website menu parsing site pages.

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l12"]
        [m-menu template="menu/menu" alignment="left" sidebar-id="nav-mobile"][/m-menu]  
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
      root-page: the name of the page which children will be rendered. By default it is the home page
      submenu: renders the given pages as a dropdown. Usage: submenu="page1,page2"
      template: defines the template to render. It renders the base menu when the property is not defined
      alignment: Sets the menu alignment. This parameter accepts the following values: left, center, right
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"

      Item component properties

      An arbitrary menu link not included in the processed page can be rendered, adding a m-menu-item shortcode:
        [m-menu-item position="before" url="#" menu="Label"][/m-menu-item]
      position: the menu position. This property accepts the "before,after" values and "after" is the default value used when the property is empty
      url: the url to render
      menu: th emenu label
    [/m-help]
    [m-menu template="menu/menu" alignment="left" sidebar-id="nav-mobile"][/m-menu]    
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  ## Inline menu
  To render the menu inline, just add the **inline-navigation** class to menu attributes.

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l12"]
        [m-menu template="menu/menu" alignment="left" sidebar-id="nav-mobile" attributes="class:inline-navigation"][/m-menu]  
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]

  D_CODE

  [m-tag tag="div" attributes="id:menu_code"]
    [raw]
    ```
    [m-help]
      Main component properties

      sidebar-id: defines the id of the sidebar opened for small screens
      root-page: the name of the page which children will be rendered. By default it is the home page
      submenu: renders the given pages as a dropdown. Usage: submenu="page1,page2"
      template: defines the template to render. It renders the base menu when the property is not defined
      alignment: Sets the menu alignment. This parameter accepts the following values: left, center, right
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"

      Item component properties

      An arbitrary menu link not included in the processed page can be rendered, adding a m-menu-item shortcode:
        [m-menu-item position="before" url="#" menu="Label"][/m-menu-item]
      position: the menu position. This property accepts the "before,after" values and "after" is the default value used when the property is empty
      url: the url to render
      menu: th emenu label
    [/m-help]
    [m-menu template="menu/menu" alignment="left" sidebar-id="nav-mobile" attributes="class:inline-navigation"][/m-menu]   
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="menu_code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  ## Add an extra link to the navigation menu
  To add an extra link to your navigation menu, simply add a **m-menu-item** to the menu shortcode.

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l12"]
        [m-menu template="menu/menu" alignment="left" sidebar-id="nav-mobile"]
          [m-menu-item position="before" url="#" menu="Extra navigation link"][/m-menu-item]
        [/m-menu]  
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]

  D_CODE

  [m-tag tag="div" attributes="id:extra_menu_link_code"]
    [raw]
    ```
    [m-help]
      Main component properties

      sidebar-id: defines the id of the sidebar opened for small screens
      root-page: the name of the page which children will be rendered. By default it is the home page
      submenu: renders the given pages as a dropdown. Usage: submenu="page1,page2"
      template: defines the template to render. It renders the base menu when the property is not defined
      alignment: Sets the menu alignment. This parameter accepts the following values: left, center, right
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"

      Item component properties

      An arbitrary menu link not included in the processed page can be rendered, adding a m-menu-item shortcode:
        [m-menu-item position="before" url="#" menu="Label"][/m-menu-item]
      position: the menu position. This property accepts the "before,after" values and "after" is the default value used when the property is empty
      url: the url to render
      menu: th emenu label
    [/m-help]
    [m-menu template="menu/menu" alignment="left" sidebar-id="nav-mobile"]
      [m-menu-item position="before" url="#" menu="Extra navigation link"][/m-menu-item]
    [/m-menu]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="extra_menu_link_code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
