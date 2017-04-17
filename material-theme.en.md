[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # Material a Grav CMS simple theme to build websites using shortcodes and markdown
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  |==
  ## Build sites in a different way using shortcodes and markdown

  **Centre** comes with a very basic and simple theme, that contains only two usable templates:

  - [m-icon icon="fa-check"][/m-icon] default.html.twig
  - [m-icon icon="fa-check"][/m-icon] modules/default.html.twig

  Though this theme might looks so poor, it has all you need to build your website because you will not define your templates using twig but using **shortcodes**, **components** and **markdown** directly into the website pages.
  ==|
  
  According to that configuration you will use the **default.md** page to define a standard page and the **_default.md** page to define a modular page.

  [Learn more about how to build layouts using shortcodes and markdown](/centre/material-design-made-easy-with-grav-cms-pro#shortcodes).

  ### Additional assets

  The Material theme comes with full Materialize framework assets. It extends those framework classes and build several new stylesheets different than the standard ones distributed with Materialize. This results in a set of ready stylesheets using different color schemes, build according with Material design colors, which can be used out of the box.

  Each stylesheets name follows the following rule **material-{primary color}-{secondary color}.scss**, so to use one of these stylesheets just add the following configuration to **site.yaml configuration file**:

  [raw]
  ```
  material:
    css_theme: teal-pink
  ```
  [/raw]

  to use the **material-teal-pink.scss**.

  ### Customizations

  When you need to create a customize something you must create a new theme that inherits from the Material theme, as well explained [in this article](), then you can customize evrything.

  #### Add a custom stylesheet

  The simple customization you can do is adding a new **css/custom.css** file under your custom theme. Materialize theme looks for that file by default and loads it when it is found, so you do not need to change anything in theme's templates.

  > we strongly suggest to use sass/scss in your theme and configure them to create the custom.css file in the correct lacation.

  #### Customize Materialize framework assets

  When you start building your site it could happen you need to use a Materialize customized stylesheet, mainly to create a custom colors combination different than the bounded ones or just to change other framework settings. Let's see how you can easily create your customized Materialize framework assets.

  > Please consider we use Compass to compile our sass/scss files, so the following instructions refers to that application.

  Let's say we want to create a new custom stylesheet to use green as primary color of our website and orange as secondary one. To accomplish this s task, we need to work on two source files:

  - [m-icon icon="fa-check"][/m-icon] The main stylesheet file
  - [m-icon icon="fa-check"][/m-icon] The file that contains the variables

  To get started, please reproduce the **material-theme/sass/lib** folder structure in your custom theme, then copy the **config.rb** file from the **material-theme/sass** directory, into the **sass** folder of your custom theme.

  Create a **material** folder under the **sass/lib** folder of your custom theme, then copy the **material-blue-pink.scss** and the **variables/_material_blue_pink_variables.scss** files, both into the **material** folder of your custom theme.

  > It is not mandatory to start from those files, so feel free to start from the files you prefer.

  Next, you must rename the **material-blue-pink.scss** as **material-green-orange.scss** and the **_material_blue_pink_variables.scss** as **_material_green_orange_variables.scss**.

  Open your stylesheet file and change the

  [raw]
  ```
  **@import "variables/material_blue_pink_variables";**  
  ```
  [/raw]

  directive to reflect the name and the path of your variables file:

  [raw]
  ```
  @import "material_green_orange_variables";
  ```
  [/raw]

  then fix the relative paths to point the material theme folder as follows:

  [raw]
  ```
  @charset "UTF-8"; // Mixins
  @import "./../../../material-theme/vendor/materialize-src/sass/components/mixins";
  @import "./../../../material-theme/vendor/materialize-src/sass/components/color";
  @import "material_green_orange_variables";
  @import "./../../../material-theme/sass/lib/material/variables/material_base";
  ```
  [/raw]

  Try to compile your new stylesheet to check if everything is fine.

  Now you can start to change the parameters you want in your variables file, so open the **_material_green_orange_variables.scss** and customize the colors section as follows:

  [raw]
  ```
  $primary-color: color("green", "darken-2");
  $primary-color-light: color("green", "lighten-3");
  $primary-color-dark: color("green", "darken-4");

  $secondary-color: color("orange", "accent-3");
  ```
  [/raw]

  At last, to use your stylesheet, change the material configuration in the **site.yaml** file as follows:

  [raw]
  ```
  material:
    css_theme: green-orange
  ```
  [/raw]

  and you are done.  
[/m-dictionary-item]
