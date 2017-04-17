[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # Gravitom, the Atom plugin to manage Material plugin shortcodes
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  |==
  ## An Atom plugin to manage Material plugin shortcodes

  Grav CMS is a flat-file Content Management System, which means website contents are saved into markdown files, instead of saving them in a database.

  Due to the nature of this kind of application, we though the best way to have the real control on the website is working directly on the files and not using web interfaces.

  For this reason we choose **[Atom](https://atom.io/)**, an awesome editor from Github developers, to manage all our websites.
  ==|
  The main reason of this choice is the great extensibility it offers. In fact we developed an **Atom plugin**, called **Gravitom**, to insert all the shortcodes in our website pages from a nice and usable interface.

  ### The interface

  The interface has two different modes, one used to configure the Grav header section and the second one used to manage contents.

  ![Gravitom Atom plugin interface](/user/pages/images/atom-plugin.jpg "Gravitom Atom plugin"){.responsive-img}

  #### Header mode

  When you work on the header section, the interface let you add several kind of headers and to optimize existing ones. You can choose between three header:

  - [m-icon icon="fa-check"][/m-icon] Base
  - [m-icon icon="fa-check"][/m-icon] Optimized
  - [m-icon icon="fa-check"][/m-icon] Rich

  Next, you can easily add Grav page collection configuration. As bonus, you can have the guide taken from official Grav's documentation, when you put the cursor on a known property.

  #### Content mode

  In content mode you can format the content in markdown through the interface and insert the shortcodes from the toolbar. Intead of classic markdown files where contents starts from the beginning of each line, you can indent the shortcodes as you prefer, to get more readibility.

  Normally you should write your shortcodes as follow to get their contents parsed correctly in markdown:

  [raw]
  ```
  [m-grid]
  [m-grid-row]
  [m-grid-col attributes="class:s12 m12 l12"]
  ## Title
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
  [/m-grid-col]
  [/m-grid-row]
  [m-grid-row]
  [m-grid-col attributes="class:s12 m6 l6"]
  ### Subtitle 1
  Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
  [/m-grid-col]        
  [m-grid-col attributes="class:s12 m6 l6"]
  ### Subtitle 2
  Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
  [/m-grid-col]
  [/m-grid-row]
  [/m-grid]
  ```
  [/raw]

Thanks to our Material plugin, you can write the same shortcode indenting as you prefer, because it is normalized when Grav renders the page. The same shortcode can be written as follows:

  [raw]
  ```
  [m-grid]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l12"]
        ## Title
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-grid-col]
    [/m-grid-row]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m6 l6"]
        ### Subtitle 1
        Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
      [/m-grid-col]        
      [m-grid-col attributes="class:s12 m6 l6"]
        ### Subtitle 2
        Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  
  ```
  [/raw]

  Another important aspect we covered to lift up readability, was code highlighting, to give you the best experience when you work on your website.

  ### Inline help

  Each shortcode has an handy inline help description where are well explained all the properties that can be used with the shortcode itself.

  [raw]
  ```
  [m-help]
    image: defines the image to render
    blurred-image: defines the blurred image which progressively replaces the original one, when page is scrolled down, Remove this property to add just the image.
    image-path: defines the images path. By default images are placed into the "images" page and "images" is default value for this property.
    height: sets the jumbotron height. Accepted values are "full, three-quarters, half"
    attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"
  [/m-help]
  [m-jumbotron image="image.jpg" blurred-image="image_blurred.jpg" height="full"]
    [m-grid]
      [m-grid-row]
        [m-grid-col attributes="col s12 m8 l8"]
          # Title
          Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
  [/m-jumbotron]  
  ```
  [/raw]

  > The **m-help** shortcode is not rendered

[/m-dictionary-item]
