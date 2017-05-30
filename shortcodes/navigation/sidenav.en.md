[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Sidenav" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  Renderes a sidenav menu placed on the left of the page.

  > Each page already can contain only and instance for this element, so an example that replects the code cannot be rendered. To watch it in action just look the rendered one in the page.

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      PROPERTIES
      sidebar-id: defines the id of the sidebar opened for small screens
      visible: shows the sidebar only in the specified pages, listed by menu name
    [/m-help]
    [m-sidenav sidebar-id="sidenav-services"]
      [m-menu template="sidenav/sidenav_menu" sidebar-id="sidenav-mobile" root-page="page_path"]
        [m-menu-item position="before"]
          [m-tag tag="div" attributes="class:userView"]
            ![Image](/images/home2.jpg) {.background .responsive-img}
            ### Company name
          [/m-tag]
        [/m-menu-item]
      [/m-menu]
    [/m-sidenav]       
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

[/m-dictionary-item]
