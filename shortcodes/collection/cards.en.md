[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Cards collection" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE_TITLE
  This shortcode renders a collection of pages as cards. Let's see an example:

  [m-card-collection page-name="/centre" card-type="card" container-attributes="class:box-medium s-margin-bottom-small m-margin-bottom-medium" column-attributes="class:col s12 m6 l6" container="false"]
  [/m-card-collection]

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
      [m-help]
        Main component properties
        image: The image name with the extension. Set a blank value for no image
        image-path: The image directory
        size: defines the card size. This parameters accepts "small, medium, large" values. When size is not defined the card displays the whole content
        card-type: Defines the card type to display. It accept the following values: card, horizontal, simple, links
        card-attributes: Adds html attributes to card element. Example card-attributes="class: blue-grey darken-1"
        card-content-attributes: Adds html attributes to the div that contains the content. Example attributes="class: foo, rel=bar"
      [/m-help]
      [m-card-collection page-name="/shop" card-type="card" container-attributes="class:box-medium s-margin-bottom-small m-margin-bottom-medium" column-attributes="class:col s12 m6 l6"]
      [/m-card-collection]      
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  Each published page under the **centre folder** is represented by a Materialize basic card.

  ### Extra single card configuration
  Each configuration for a card is made into the page itself, adding the following configuration.

  [m-tag tag="div" attributes="id:card-code"]
    [raw]
    ```
      card:
        image: 'material-header.jpg'
        #image: '/images'
        action:
          url: self
          label: 'Read'
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="card-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  ### Add content to card
  Due to page structure, to define the content displayed on the catrd, you must use the dictionary key that handles the contet you want to display. You just need to add the following option to **card** value:

  [m-tag tag="div" attributes="id:dictionary-code"]
    [raw]
    ```
      dictionary_item: D_MAIN_CONTENT
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="dictionary-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  To display just a part of the content you can delimit the code using the | == == | markers, as follows:

  [m-tag tag="div" attributes="id:dictionary-code"]
    [raw]
    ```
      [m-dictionary-item name="D_MAIN_CONTENT"]
        | ==
        ## Material design like a breeze with Material plugin

        **Material plugin** is the core of [Grav Cms Pro system](/#gravcmspro). This micro application provides several shortcodes to handle the powerful [Materialize framework](http://materializecss.com/) in your [Grav](https://getgrav.org) application. The combination of all these elements results in an easy introduction of **[Material Design](https://material.io/guidelines/)** for your website.
        == |

        Basically, Material plugin does two things tied together:
      [/m-dictionary-item]
    ```
    [/raw]
  [/m-tag]

  ### Available types
  The cards collection handles the following card types and can be activated just changing the **card-type**:

  - [m-icon icon="fa-check"][/m-icon] card
  - [m-icon icon="fa-check"][/m-icon] horizontal
  - [m-icon icon="fa-check"][/m-icon] simple
  - [m-icon icon="fa-check"][/m-icon] links

  #### Horizontal cards collection
  [m-card-collection page-name="/centre" card-type="horizontal" container-attributes="class:box-medium s-margin-bottom-small m-margin-bottom-medium" column-attributes="class:col s12 m6 l6" container="false"]
  [/m-card-collection]

  #### Simple cards collection
  [m-card-collection page-name="/centre" card-type="simple" container-attributes="class:box-medium s-margin-bottom-small m-margin-bottom-medium" column-attributes="class:col s12 m6 l6" container="false"]
  [/m-card-collection]

  #### Links cards collection
  [m-card-collection page-name="/shortcodes" card-type="links" container-attributes="class:box-medium s-margin-bottom-small m-margin-bottom-medium" column-attributes="class:col s12 m4 l4" container="false"]
  [/m-card-collection]


[/m-dictionary-item]
