[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # Material design made easy with Grav CMS Pro
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  |==
  ## Material design like a breeze with Material plugin

  **Material plugin** is the core of [Grav Cms Pro system](/#gravcmspro). This micro application provides several shortcodes to handle the powerful [Materialize framework](http://materializecss.com/) in your [Grav](https://getgrav.org) application. The combination of all these elements results in an easy introduction of **[Material Design](https://material.io/guidelines/)** for your website.
  ==|
  Basically, Material plugin does two things tied together:

  - [m-icon icon="fa-check"][/m-icon] Implements shortcodes to use Materialize components
  - [m-icon icon="fa-check"][/m-icon] Extends Materialize stylesheets adding several basilar and complex classes not provided by Materialize

  ### Shortcodes

  **Shortcodes** are small but powerful pieces of code used to render complex html components. For example, to render a Materialize card in your Grav CMS markdown page you will use the following shortcode:
  [raw]
  ```
  [m-card image="demo-image.jpg"]
    ## Title
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
    labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
    laboris nisi ut aliquip ex ea commodo consequat.
  [/m-card]
  ```
  [/raw]

  which will render the following card:

  [m-grid]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l12"]
        [m-card image="demo-image.jpg"]
          ## Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
          labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
          laboris nisi ut aliquip ex ea commodo consequat.
        [/m-card]
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  Is it cool, isn't it?

  ### Building layouts with shortcodes and markdown [m-link link-attributes="class: opaque opaque-reveal, name:shortcodes" icon="fa-link fa-flip-horizontal"][/m-link]

  You can also build complex layouts using the powerful **m-grid shortcode**, which handles the **Materialize grid component**:

  [raw]
  ```
  [m-grid]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m6 l6"]
        ## Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
        labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
        laboris nisi ut aliquip ex ea commodo consequat.
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m6 l6"]
        ## Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
        labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
        laboris nisi ut aliquip ex ea commodo consequat.
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  
  ```
  [/raw]

  ### More shortcodes than Materialize

  Material plugin is not only a Grav CMS Materialize framework implementation, in fact it adds several basic components like icons, rich links, rich images and more. Here you get the **m-tag shortcode**, which is the most powerful you can use, because you can add any html tag to your page. For example to render a div just add this shortcode to your page:

  [raw]
  ```
  [m-tag tag="div"]
    ## Title
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
    labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
    laboris nisi ut aliquip ex ea commodo consequat.
  [/m-tag]  
  ```
  [/raw]

  Next, you can do something like this to add a list of elements with some css classes applied:

  [raw]
  ```
  [m-tag tag="ul" attributes="class:foo"]
    [m-tag tag="li" attributes="class:bar"][m-icon icon="fa-check"][/m-icon] Item 1[/m-tag]
    [m-tag tag="li"][m-icon icon="fa-check"][/m-icon] Item 2[/m-tag]
    [m-tag tag="li"][m-icon icon="fa-check"][/m-icon] Item 3[/m-tag]
  [/m-tag]  
  ```
  [/raw]

  which results as:

  [m-tag tag="ul" attributes="class:foo"]
    [m-tag tag="li" attributes="class:bar"][m-icon icon="fa-check"][/m-icon] Item 1[/m-tag]
    [m-tag tag="li"][m-icon icon="fa-check"][/m-icon] Item 2[/m-tag]
    [m-tag tag="li"][m-icon icon="fa-check"][/m-icon] Item 3[/m-tag]
  [/m-tag]

  You can also nest shortcodes, for example nesting a **m-grid shortcode** into a **m-tag** one as follows:

  [raw]
  ```
  [m-tag tag="div" attributes="class:grey lighten-2"]
    [m-grid container="false"]
      [m-grid-row]
        [m-grid-col attributes="class:s12 m12 l12 padding-medium"]
          ## Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut
          labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco
          laboris nisi ut aliquip ex ea commodo consequat.
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]    
  [/m-tag]  
  ```
  [/raw]

  to get:

  [m-tag tag="div" attributes="class:grey lighten-2"]
    [m-grid container="false"]
      [m-grid-row]
        [m-grid-col attributes="class:s12 m12 l12 padding-medium"]
          ## Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]    
  [/m-tag]

  ### Stylesheets classes out of the box

  After you read the code just proposed, maybe you would have noticed the use of **padding-medium** class, one of the classed we implemented to save time and increment the productivity. For example you can add a nice colored transparent panel with text inside, as follows:

  [m-tag tag="div" image="demo-image.jpg" attributes="class:padding-top-bottom-large image-cover"]
    [m-grid]
      [m-grid-row]
        [m-grid-col attributes="class:s12 m12 l12 opaque-panel-red-darken-4-high padding-large text-full-white rounded"]
          ## Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
  [/m-tag]

  And this is the code:

  [raw]
  ```
  [m-tag tag="div" image="demo-image.jpg" attributes="class:padding-top-bottom-large image-cover"]
    [m-grid]
      [m-grid-row]
        [m-grid-col attributes="class:s12 m12 l12 opaque-panel-red-darken-4-high padding-large text-full-white rounded"]
          ## Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
  [/m-tag]
  ```
  [/raw]

  Here we used a lot of useful classes from our Materialize extension:

  - [m-icon icon="fa-check"][/m-icon] padding-top-bottom-large
  - [m-icon icon="fa-check"][/m-icon] image-cover
  - [m-icon icon="fa-check"][/m-icon] opaque-panel-red-darken-4-high
  - [m-icon icon="fa-check"][/m-icon] padding-large
  - [m-icon icon="fa-check"][/m-icon] text-full-white
  - [m-icon icon="fa-check"][/m-icon] rounded

  All classes names are quite self explaining, but the **opaque-panel-red-darken-4-high** class requires some words. In fact it adds a high opaque panel colored using Materialize red-darken-4 color. You can use the **opaque-panel-** class choosing colors from the whole Materialize framework and choose the opaque intensity from the **low, medium, high** values. For example you can render a medium opaque blue panel using the **opaque-panel-blue-base-medium** class.

  ### Components [m-link link-attributes="class: opaque opaque-reveal, name:components" icon="fa-link fa-flip-horizontal"][/m-link]
  Shortcodes can be packed in components to reuse complex structures within a websites. Let's see an example:

  [m-component component="3x1-grid" folder="promo-table"]
    [m-component-item name="M_MAIN_CONTENT" M_EXTRA_ATTRIBUTES=""]   
      ### Lorem ipsum
      Lorem ipsum dolor sit amet, consectetur adipiscing elit
    [/m-component-item]

    [m-component-item name="M_PROMO_ITEM_1" M_ICON="style" M_ATTRIBUTES=""]
      Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
    [/m-component-item]

    [m-component-item name="M_PROMO_ITEM_2" M_ICON="create" M_ATTRIBUTES=""]
      Ut enim ad minim veniam, quis nostrud exercitation ullamco
    [/m-component-item]

    [m-component-item name="M_PROMO_ITEM_3" M_ICON="dvr" M_ATTRIBUTES=""]
      laboris nisi ut aliquip ex ea commodo consequat
    [/m-component-item]
  [/m-component]

  That component is rendered by the following code:

[raw]
```
[m-component component="3x1-grid" folder="promo-table"]
  [m-component-item name="M_MAIN_CONTENT" M_EXTRA_ATTRIBUTES=""]   
    ### Lorem ipsum
    Lorem ipsum dolor sit amet, consectetur adipiscing elit
  [/m-component-item]

  [m-component-item name="M_PROMO_ITEM_1" M_ICON="style" M_ATTRIBUTES=""]
    Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua
  [/m-component-item]

  [m-component-item name="M_PROMO_ITEM_2" M_ICON="create" M_ATTRIBUTES=""]
    Ut enim ad minim veniam, quis nostrud exercitation ullamco
  [/m-component-item]

  [m-component-item name="M_PROMO_ITEM_3" M_ICON="dvr" M_ATTRIBUTES=""]
    laboris nisi ut aliquip ex ea commodo consequat
  [/m-component-item]
[/m-component]
```
[/raw]

  The backend code of that component is the following:

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
          <<m_promo_item_1.m_content>>
        [/m-promo-table-item]
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m4 l4 highligthed1"]
        [m-promo-table-item icon="M_PROMO_ITEM_3.M_ICON" attributes="M_PROMO_ITEM_3.M_ATTRIBUTES"]
          <<m_promo_item_1.m_content>>
        [/m-promo-table-item]
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]
  ```
  [/raw]

  You can create complex structures using shortcodes. Components are required when you need to [share contents](/documentation/how-to-share-contents-through-the-website-with-grav-cms-pro) between pages. then reuse them in all your websites

  ### More shortcodes
  Here you can give a look to some other sample components from our framework, just as a further demonstration:

  #### Rich image

  [m-rich-image container-attributes="class:box-medium" content-attributes="class:text-white padding-small" image-attributes="class:image-cover" image="demo-image.jpg" scale="true" ]
    #### Lorem ipsum
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
  [/m-rich-image]

  ##### The Code

  [raw]
  ```
  [m-rich-image container-attributes="class:box-medium" content-attributes="class:text-white padding-small" image-attributes="class:image-cover" image="demo-image.jpg" scale="true" ]
    #### Lorem ipsum
    Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt
  [/m-rich-image]
  ```
  [/raw]

  #### Subtle card

  [m-subtle-card effect="effect-4" image="demo-image.jpg"]
    ### Product name
    Product subtitle
    [Take a look](#){.btn}
  [/m-subtle-card]  

  ##### The Code

  [raw]
  ```
  [m-subtle-card effect="effect-4" image="demo-image.jpg"]
    ### Product name
    Product subtitle
    [Take a look](#){.btn}
  [/m-subtle-card]  
  ```
  [/raw]

  Enjoy Material plugin and Grav CMS Pro!
[/m-dictionary-item]
