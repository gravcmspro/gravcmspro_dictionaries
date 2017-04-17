[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # How to handle website shared contents
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  |==
  ## Share website contents through components

  A website has some parts which must be shared through pages. In **Centre**, contents are shared through the website using components.

  In order, to share a content through the website, you must create a component file into a subdirectory placed under the **user/components** folder. The folder name is not mandatory.
  ==|
  ### Share the website navbar for the whole site

  One of the most common element to share though the whole website is the navbar. So create a **navbar.component** file under the **user/components/shared** folder, then paste inside a navbar shortcode like this one:

  [raw]
  ```
  [m-navbar brand-name="D_BRAND" transparent="all" sidebar-id="nav-mobile" render="true"]
    [m-menu name="menu0" template="menu/menu" alignment="right" sidebar-id="nav-mobile" submenu="centre,documentation"][/m-menu]
  [/m-navbar]
  ```
  [/raw]

  Next, to use the component in your pages just call it as follows:

  [raw]
  ```
  <| SHARED.NAVBAR |>
  ```
  [/raw]

  where **SHARED** is the folder name and **NAVBAR** is the file name without extension.

  ### Create a two columns layout

  Let's suppose the internal pages of your website requires a two columns layout, the bigger one to show main contents, while the smaller used to render a sidebar.

  To handle that layout simple add a new **grid_two_columns.component** under the **user/components/shared** folder, then paste inside this code:

  [raw]
  ```
  [m-component component="grid-two-columns" folder="content" M_ATTRIBUTES="class:margin-top-large"]
    [m-component-item name="COLUMN_1" M_ATTRIBUTES="class:s12 m9 l9"]
      D_MAIN_CONTENT
    [/m-component-item]
    [m-component-item name="COLUMN_2" M_ATTRIBUTES="class:s12 m3 l3"]
      [m-component component="sidebar"] [/m-component]
    [/m-component-item]
  [/m-component]
  ```
  [/raw]

  Each page that uses this component will declare the **D_MAIN_CONTENT** dictionary item into his own dictionary to handle the main contents, then will use the **sidebar** component to handle the sidebar.

  The **sidebar** component lives under the **user/components** folder and might look like this one:

  [raw]
  ```
  [m-tag tag="div"]
    [m-google-adsense style="display:block" data-ad-client="xxxxxxxx" data-ad-slot="xxxxxxxx" data-ad-format="auto"][/m-google-adsense]
  [/m-tag]
  ```
  [/raw]

[/m-dictionary-item]
