[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Footer top menu one column" component
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="footer-top-menu-1-columns" folder="footer" M_EXTRA_ATTRIBUTES="text-full-white"]
    [m-component-item name="M_NAVIGATION"]
      [m-menu name="menu1" template="menu/menu"]
        [m-menu-item position="after" menu="Cookies" url="cookies-policy" ][/m-menu-item]
      [/m-menu]
    [/m-component-item]
    [m-component-item name="M_COLUMN" M_ATTRIBUTES="class:s12 offset-m2 l8 offset-l2 center"]
      #### Lorem ipsum dolor sit amet
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
    [/m-component-item]
    [m-component-item name="M_COPYRIGHT"]
      &copy; 2016 Acme ltd.
      [m-tag tag="div" attributes="class:author"]
      Powered by [Grav CMS Pro](https://gravcmspro.com "Grav Cms Professional Websites")
      [/m-tag]
    [/m-component-item]
  [/m-component]

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_EXTRA_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar

      Item component properties
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-component component="footer-top-menu-1-columns" folder="footer" M_EXTRA_ATTRIBUTES="text-full-white"]
      [m-component-item name="M_NAVIGATION"]
        [m-menu name="menu1" template="menu/menu"]
          [m-menu-item position="after" menu="Cookies" url="cookies-policy" ][/m-menu-item]
        [/m-menu]
      [/m-component-item]
      [m-component-item name="M_COLUMN" M_ATTRIBUTES="class:s12 offset-m2 l8 offset-l2 center"]
        #### Lorem ipsum dolor sit amet
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
      [/m-component-item]
      [m-component-item name="M_COPYRIGHT"]
        &copy; 2016 Acme ltd.
        [m-tag tag="div" attributes="class:author"]
        Powered by [Grav CMS Pro](https://gravcmspro.com "Grav Cms Professional Websites")
        [/m-tag]
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
    [m-tag tag="footer" name="M_NAME" render="M_RENDER" attributes="class:page-footer M_EXTRA_ATTRIBUTES"]
      [m-grid attributes="class:margin-top-medium"]
        [m-grid-row]
          [m-grid-col attributes="class:s12 m12 l12 center inline-navigation M_NAVIGATION.M_EXTRA_ATTRIBUTES"]
            M_NAVIGATION.M_CONTENT
          [/m-grid-col]
        [/m-grid-row]
        [m-grid-row]
          [m-grid-col attributes="M_COLUMN.M_ATTRIBUTES"]
            M_COLUMN.M_CONTENT
          [/m-grid-col]
        [/m-grid-row]
        [m-grid-row]
          [m-grid-col attributes="class:l12 m12 s12 center footer-copyright"]
            M_COPYRIGHT.M_CONTENT
          [/m-grid-col]
        [/m-grid-row]
      [/m-grid]
    [/m-tag]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
