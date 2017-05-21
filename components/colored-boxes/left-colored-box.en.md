[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Left colored box" component (PRO)
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="colored-box" folder="colored-boxes" M_COLOR="blue-grey" M_ATTRIBUTES=""]
    [m-component-item name="M_BOX_1" M_ATTRIBUTES="class:l5 m5 s12 box-large center text-white vertical-align"]
      [m-tag tag="div"]
        # An awesome title
      [/m-tag]
    [/m-component-item]
    [m-component-item name="M_BOX_2" M_ATTRIBUTES="class:l7 m7 s12 box-large padding-large white"]
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
    [/m-component-item]
  [/m-component]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_COLOR: Defines the size for all the item's columns
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"

      Item component properties
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-component component="colored-box" folder="colored-boxes" M_COLOR="blue-grey" M_ATTRIBUTES=""]
      [m-component-item name="M_BOX_1" M_ATTRIBUTES="class:l5 m5 s12 box-large center text-white vertical-align"]
        [m-tag tag="div"]
          # An awesome title
        [/m-tag]
      [/m-component-item]
      [m-component-item name="M_BOX_2" M_ATTRIBUTES="class:l7 m7 s12 box-large padding-large white"]
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
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
    [m-grid container="false"]
      [m-grid-row attributes="class:no-margin M_COLOR"]
        [m-grid-col attributes="M_BOX_1.M_ATTRIBUTES"]
          M_BOX_1.M_CONTENT
        [/m-grid-col]
        [m-grid-col attributes="M_BOX_2.M_ATTRIBUTES"]
          M_BOX_2.M_CONTENT
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
