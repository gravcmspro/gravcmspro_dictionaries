[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # Pack shortcodes into components to reuse them in your websites
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  |==
  ## Components are a combination of shortcodes

  Components are a convenient way to pack a combination of shortcodes, with the pourpose of building complex structures, you can reuse later in all your websites. For example we have a blurred jumbotron with a transparent panel placed into the middle center and a button to scroll down to a specific page section.
  ==|
  The required shortcodes to render an HTML component like that, is the following one:

  [raw]
  ```
  [m-jumbotron name="jumbotron" image="demo-image.jpg" image-path="images" height="full"]
    [m-grid]
      [m-grid-row]
        [m-grid-col attributes="class:l10 offset-l1 m12 s12 opaque-panel-shades-black-medium padding-medium rounded text-full-white center"]
          ### Anim pariatur
          Anim pariatur cliche reprehenderit enim eiusmod high life accusamus
        [/m-grid-col]
      [/m-grid-row]
      [m-grid-row]
        [m-grid-col attributes="class:s12 m12 l12"]
          [m-tag tag="div" attributes="class:jumbotron-scrolldown" ignore-items="true"]
            [m-link url="#main" link-attributes="class:smoothscroll" icon="keyboard_arrow_down"][/m-link]
          [/m-tag]
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
  [/m-jumbotron]
  ```
  [/raw]

  This combination of shortcodes works very well and you can copy and reuse it as it is but, with a minimum effort, you can convert it into a component and use it in a more easy and convenient way.

  ### Create a new component

  To create a new component you just need to create a simple file with the **component extension**, under one of this folders:

  - [m-icon icon="fa-check"][/m-icon] In the page folder where it is used
  - [m-icon icon="fa-check"][/m-icon] In the **user/components** folder
  - [m-icon icon="fa-check"][/m-icon] In the Material plugin

  Material plugin lookes for a component following the given order, so the first found wins.

  > Obviously you must not add a component of yours under the Material plugin, because it will be erased when a new release take place.

  Next, just add your code into that file and replace the properties you want to pass from the calling component. There are no limits to properties number. The shortcode content is always defined by the **<<m_content>>** placeholder.

  [raw]
  ```
  [m-jumbotron name="M_NAME" image="M_IMAGE" image-path="M_PATH" height="M_HEIGHT"]
    [m-grid]
      [m-grid-row]
        [m-grid-col attributes="M_ATTRIBUTES"]
          <<m_content>>
        [/m-grid-col]
      [/m-grid-row]
      [m-grid-row]
        [m-grid-col attributes="class:s12 m12 l12"]
          [m-tag tag="div" attributes="class:jumbotron-scrolldown" ignore-items="true"]
            [m-link url="#main" link-attributes="class:smoothscroll" icon="keyboard_arrow_down"][/m-link]
          [/m-tag]
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
  [/m-jumbotron]
  ```
  [/raw]

  When your component is ready, you can call it using the **m-component** shortcode:

  [raw]
  ```
  [m-component component="jumbotron" folder="jumbotron" M_NAME="jumbotron" M_IMAGE="demo-image.jpg" M_PATH="images" M_HEIGHT="full" M_ATTRIBUTES="class:l10 offset-l1 m12 s12 opaque-panel-shades-black-medium padding-medium rounded text-full-white center"]
    ### Anim pariatur
    Anim pariatur cliche reprehenderit enim eiusmod high life accusamus
  [/m-component]
  ```
  [/raw]

  The **m-component** shortcode defines a **component property** which requires the component file name without extension and a **folder property** which requires the directory name where the component lives.

  Next, you must provide a value for all the properties defined in the component.

  ### Component items

  Complex components might require to define more than one single item, for example look at this code to define a promo table, where are defined three items:

  [raw]
  ```
  [m-grid attributes="class:icons-promo"]
    [m-grid-row attributes="class:center" ]
      [m-grid-col attributes="class:s12 m12 l12"]
      ## Title
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-grid-col]
    [/m-grid-row]
    [m-grid-row attributes="class:center"]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-promo-table-item icon="style" attributes="box-medium"]
          ## Item 1
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-promo-table-item]
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-promo-table-item icon="create" attributes="box-medium"]
          ## Item 2
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-promo-table-item]
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m4 l4 highligthed1"]
        [m-promo-table-item icon="dvr" attributes="box-medium"]
          ## Item 3
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-promo-table-item]
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]
  ```
  [/raw]

  To handle a component like that, it is enough to define the required subitems, as follows:

  [raw]
  ```
  [m-grid attributes="class:icons-promo"]
    [m-grid-row attributes="class:center" ]
      [m-grid-col attributes="class:s12 m12 l12 M_MAIN_CONTENT.M_EXTRA_ATTRIBUTES"]
        <<m_main_content.m_content>>
      [/m-grid-col]
    [/m-grid-row]
    [m-grid-row attributes="class:center"]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-promo-table-item icon="M_PROMO_ITEM_1.M_ICON" attributes="M_PROMO_ITEM_1.M_ATTRIBUTES"]
          <<m_promo_item_1.m_content>>
        [/m-promo-table-item]
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-promo-table-item icon="M_PROMO_ITEM_2.M_ICON" attributes="M_PROMO_ITEM_2.M_ATTRIBUTES"]
          <<m_promo_item_2.m_content>>
        [/m-promo-table-item]
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m4 l4 highligthed1"]
        [m-promo-table-item icon="M_PROMO_ITEM_3.M_ICON" attributes="M_PROMO_ITEM_3.M_ATTRIBUTES"]
          <<m_promo_item_3.m_content>>
        [/m-promo-table-item]
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]
  ```
  [/raw]

  In this example, the defined subitems are the following:

  - [m-icon icon="fa-check"][/m-icon] M_MAIN_CONTENT
  - [m-icon icon="fa-check"][/m-icon] M_PROMO_ITEM_1
  - [m-icon icon="fa-check"][/m-icon] M_PROMO_ITEM_2
  - [m-icon icon="fa-check"][/m-icon] M_PROMO_ITEM_3

  To define each item property or content, you must define the item name and the property separed by a dot:

  - [m-icon icon="fa-check"][/m-icon] M_MAIN_CONTENT.M_EXTRA_ATTRIBUTES
  - [m-icon icon="fa-check"][/m-icon] M_MAIN_CONTENT.M_CONTENT

  Content is always defined by **<<m_content>>** placeholder and there is no limit to number of items defined, but every property must be declared in the calling shortcode. When you do not require to define a property just pass a blank string, for example **/m_extra_attributes/=""**.

  To call that component use the following shortcode:

  [raw]
  ```
  [m-component component="3x1-grid" folder="promo-table"]
    [m-component-item name="M_MAIN_CONTENT" M_EXTRA_ATTRIBUTES=""]      
      ## Title
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
    [/m-component-item]

    [m-component-item name="M_PROMO_ITEM_1" M_ICON="style" M_ATTRIBUTES=""]
      ## Item 1
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-component-item]

    [m-component-item name="M_PROMO_ITEM_2" M_ICON="create" M_ATTRIBUTES=""]
      ## Item 2
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-component-item]

    [m-component-item name="M_PROMO_ITEM_3" M_ICON="dvr" M_ATTRIBUTES=""]
      ## Item 3
      Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
    [/m-component-item]
  [/m-component]
  ```
  [/raw]

  So, every subitem is defined by the **m-component-item**.

  ### Customization

  A component is a static bunch of code, so, it could happen you need to customize something to better fit your needs.

  In this case, you just need copy the component file in one of the folders mentioned above and make your customizations.

[/m-dictionary-item]
