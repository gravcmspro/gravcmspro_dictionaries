[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "3x1 Services table grid" component
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="3x1-grid" folder="services-table" M_CONTAINER="false" M_EXTRA_ATTRIBUTES=""]
    [m-component-item name="M_MAIN_CONTENT" M_EXTRA_ATTRIBUTES="h1-small"]
      ### Lorem ipsum dolor sit amet
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    [/m-component-item]
    [m-component-item name="M_PROMO_ITEM_1" M_ICON="fa-lightbulb-o" M_ATTRIBUTES="class:box-ultra-tiny"]
      ### Lorem ipsum dolor sit amet
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    [/m-component-item]
    [m-component-item name="M_PROMO_ITEM_2" M_ICON="fa-lightbulb-o" M_ATTRIBUTES="class:box-ultra-tiny"]
      ### Lorem ipsum dolor sit amet
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    [/m-component-item]
    [m-component-item name="M_PROMO_ITEM_3" M_ICON="fa-lightbulb-o" M_ATTRIBUTES="class:box-ultra-tiny"]
      ### Lorem ipsum dolor sit amet
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    [/m-component-item]
  [/m-component]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_CONTAINER: When true contains and centers the component grid
      M_EXTRA_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar

      Item component properties
      M_ICON: Defines the jumbotrn height. This property accepts the following values: 'full, three-quarters, half'
      M_ATTRIBUTES: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      M_EXTRA_ATTRIBUTES: The image directory
    [/m-help]
    [m-component component="3x1-grid" folder="services-table" M_CONTAINER="true" M_EXTRA_ATTRIBUTES=""]
      [m-component-item name="M_MAIN_CONTENT" M_EXTRA_ATTRIBUTES="h1-small"]
        ### Lorem ipsum dolor sit amet
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-component-item]
      [m-component-item name="M_PROMO_ITEM_1" M_ICON="fa-lightbulb-o" M_ATTRIBUTES="class:box-small"]
        ### Lorem ipsum dolor sit amet
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-component-item]
      [m-component-item name="M_PROMO_ITEM_2" M_ICON="fa-lightbulb-o" M_ATTRIBUTES="class:box-small"]
        ### Lorem ipsum dolor sit amet
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-component-item]
      [m-component-item name="M_PROMO_ITEM_3" M_ICON="fa-lightbulb-o" M_ATTRIBUTES="class:box-small"]
        ### Lorem ipsum dolor sit amet
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
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
    [m-grid container="M_CONTAINER" attributes="class:icons-promo M_EXTRA_ATTRIBUTES"]
      [m-grid-row attributes="class:center" ]
        [m-grid-col attributes="class:s12 m12 l12 M_MAIN_CONTENT.M_EXTRA_ATTRIBUTES"]
          M_MAIN_CONTENT.M_CONTENT
        [/m-grid-col]
      [/m-grid-row]
      [m-grid-row attributes="class:center"]
        [m-grid-col attributes="class:s12 m12 l4"]
          [m-promo-table-item icon="M_PROMO_ITEM_1.M_ICON" attributes="M_PROMO_ITEM_1.M_ATTRIBUTES"]
            M_PROMO_ITEM_1.M_CONTENT
          [/m-promo-table-item]
        [/m-grid-col]
        [m-grid-col attributes="class:s12 m12 l4"]
          [m-promo-table-item icon="M_PROMO_ITEM_2.M_ICON" attributes="M_PROMO_ITEM_2.M_ATTRIBUTES"]
            M_PROMO_ITEM_2.M_CONTENT
          [/m-promo-table-item]
        [/m-grid-col]
        [m-grid-col attributes="class:s12 m12 l4 highligthed1"]
          [m-promo-table-item icon="M_PROMO_ITEM_3.M_ICON" attributes="M_PROMO_ITEM_3.M_ATTRIBUTES"]
            M_PROMO_ITEM_3.M_CONTENT
          [/m-promo-table-item]
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
