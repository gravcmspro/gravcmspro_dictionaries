[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # Keep content together and translate them easily using dictionaries
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  |==
  ## Dictionaries, a Material plugin bonus feature

  Dictionaries are a Material plugin bonus feature useful to keep contents together, instead of having them into pages shortcodes, as weel as translating them easily. Dictionaries are not bound to pages, so you can add as much content as needed. 
  ==|
  ### The dictionary file

  Dictionaries are simple markdown files that live into the **user/dictionaries** folder. To define a dictionary just name the dictionary file using the following scheme:

  [raw]
  ```
  dictionary-name.language.md
  ```
  [/raw]

  To create a dictionary entry item simply add a **m-dictionary-item** shortcode as follows:

  [raw]
  ```
  [m-dictionary-item name="/d_header_jumbotron/"]
    ### Anim pariatur
    Anim pariatur cliche reprehenderit enim eiusmod high life accusamus
  [/m-dictionary-item]
  ```
  [/raw]

  This shortcode defines a mandatory property name where you define the dictionary item placeholder, then the content lives inside the shortcode.

  ### Use the dictionary in your pages

  Using a dictionary is as simple as adding a **dictionaries** entry in **pages header**:

  [raw]
  ```
  ---
    ...

    dictionaries:
      - dictionary-name-1
      - dictionary-name-2
      ...
      - dictionary-name-n
  ---
  ```  
  [/raw]

  Next, to process the content, simply add the placeholder you defined:

  [raw]
  ```
  [m-component component="jumbotron" folder="jumbotron" M_NAME="jumbotron" M_IMAGE="demo-image.jpg" M_PATH="images" M_HEIGHT="full" M_ATTRIBUTES="class:l10 offset-l1 m12 s12 opaque-panel-shades-black-medium padding-medium rounded text-full-white center"]
    /d_header_jumbotrn/
  [/m-component]  
  ```  
  [/raw]

  You can define property values too:

  [raw]
  ```
  [m-navbar id="navbar" name="navbar" brand-name="<<d_brand>>" transparent="all" sidebar-id="nav-mobile" render="false"]
    [m-menu name="menu0" template="menu/menu" alignment="right" sidebar-id="nav-mobile" submenu="gravcmspro,documentation"][/m-menu]
  [/m-navbar]
  ```  
  [/raw]

  Here you can see the shortcode that defines the toolbar of this website and the brand property is handled by the **<<d_brand>>** placeholder.


  #### subfolders

  In order, to have a better dictionaries organization, you can save those files in a subfolder, placed under the main **dictionaries** folders. Next, in order to use those dictionaries, you just call them as follows:

  [raw]
  ```
  ---
    dictionaries:
      - subfolder1.dictionary-name-1
      - subfolder2.subfolder3.dictionary-name-2
  ---
  ```  
  [/raw]

  ### Multi language websites

  In multi languages websites, you might need to share the same content through the same pages for each language. In this situation, simply create a dictionary as usual but use the **all** token instead of the language name as follows:

  [raw]
  ```
  dictionary-name-1.all.md
  ```  
  [/raw]  
[/m-dictionary-item]
