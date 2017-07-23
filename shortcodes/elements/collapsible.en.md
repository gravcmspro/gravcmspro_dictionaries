[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Collapsible" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-collapsible popout="true" expandable="true"]
    [m-collapsible-item title="First" icon="cloud"]
      Lorem ipsum dolor sit amet.
    [/m-collapsible-item]
    [m-collapsible-item active="true" title="Second" icon="cloud"]
      Lorem ipsum dolor sit amet.
    [/m-collapsible-item]
    [m-collapsible-item title="Third" icon="cloud"]
      Lorem ipsum dolor sit amet.
    [/m-collapsible-item]
  [/m-collapsible]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
      [m-help]
       Main component properties
      popout Renders the collapsible as a popout:
      expandable: Changes the collapsible behaviour from accordion to expandable
      title: Defines the collapsible title
        Item component properties
      title: Defines the collapsible title
      icon: Defines the icon. You can choose from several kind of icons: material icons, fontawesome, material and glyphicon
      active: Activates the selected item when the collapsible is rendered
      [/m-help]
      [m-collapsible popout="true" expandable="true"]
        [m-collapsible-item title="First" icon="cloud"]
          Lorem ipsum dolor sit amet.
        [/m-collapsible-item]
        [m-collapsible-item active="true" title="Second" icon="cloud"]
          Lorem ipsum dolor sit amet.
        [/m-collapsible-item]
        [m-collapsible-item title="Third" icon="cloud"]
          Lorem ipsum dolor sit amet.
        [/m-collapsible-item]
      [/m-collapsible]  
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
