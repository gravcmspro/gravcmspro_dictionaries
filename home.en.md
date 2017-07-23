[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # Grav CMS Pro, probably the best solution to design professional websites
[/m-dictionary-item]

[m-dictionary-item name="D_INTRO_1"]
  ### Build on the shoulder of giants
  **Grav CMS Pro** provides the best solutions to develop professional websites based on [Grav Content Management System application](https://getgrav.org), nomined as [best Open Source CMS](https://www.cmscritic.com/awards/) in 2016, and [Materialize](http://materializecss.com/), the modern responsive front-end framework based on [Google Material Design](https://material.io/guidelines/) guidelines.
[/m-dictionary-item]

[m-dictionary-item name="D_INTRO_2"]
  ### Rapid Website Development
  Build a website has never been so easy thanks to **Centre**, not a simple application but a 360° system that provides several tools to manage the website from the design to the deployment.

  [Whatch Centre in action](#screencast) to learn how it is powerful.
[/m-dictionary-item]

[m-dictionary-item name="D_INTRO_3"]
  ### Affordable price
  We studied a balanced offer to fit the needs of everyone, from the guy, who just need to handle a personal website, to a professional agency who requires to develop several websites for its customers. [Discover our incredible offer](#prices) and get the best plan for you!
[/m-dictionary-item]


[m-dictionary-item name="D_CENTRE_TITLE"]
  ## Grav CMS Pro presents Centre [m-link link-attributes="class: opaque opaque-reveal, name:gravcmspro" icon="fa-link fa-flip-horizontal"][/m-link]

  ---

  Discover **Centre** the solution we developed to build the websites for our customers and we decided to share to simpify the life of other web developers.
[/m-dictionary-item]

[m-dictionary-item name="D_CENTRE_BOX_1"]
  #### [Material plugin](/centre/material-design-made-easy-with-grav-cms-pro)
  Material plugin implements the shortcodes that handle the Materialize framework components.
[/m-dictionary-item]

[m-dictionary-item name="D_CENTRE_BOX_2"]
  #### [Material theme](/centre/material-simple-grav-cms-theme-to-build-websites-using-markdown-and-shortcodes)
  The theme bound with Centre has few basic templates but comes with powerful assets.
[/m-dictionary-item]

[m-dictionary-item name="D_CENTRE_BOX_3"]
  #### [Gravitom Atom plugin](/centre/gravitom-atom-plugin-to-manage-material-plugin-shortcodes)
  Gravitom is an Atom editor plugin to handle Material shortcodes with a nice interface.
[/m-dictionary-item]

[m-dictionary-item name="D_CENTRE_BOX_4"]
  #### [Rocketeer and Website warmup](/centre/website-deployment-made-easy-with-rocketeer)
  Deploy with Rocketeer and cache all website pages with Website warmup package to always load it fast.
[/m-dictionary-item]

[m-dictionary-item name="D_FEATURES_TITLE"]
  ### Centre Features
  ---
[/m-dictionary-item]

[m-dictionary-item name="D_FEATURE_1"]
  #### Materialize framework
  We natively implement [Google Material Design protocol](https://material.io/guidelines/) for our websites, leveraging and extending awesome [Materialize framework](http://materializecss.com/).
[/m-dictionary-item]

[m-dictionary-item name="D_FEATURE_2"]
  #### Powered by Atom
  We developed an Atom package to provide a wonderful interface to handle our shortcodes and components. [Atom](https://atom.io/) is an awesome text editor developed by [Github](https://github.com).
[/m-dictionary-item]

[m-dictionary-item name="D_FEATURE_3"]
  #### Powerful sites design
  **Centre** let's you write all your website just using [shortcodes and markdown](/centre/material-design-made-easy-with-grav-cms-pro). Shortcodes can be packed as components to easily share them through your websites.
[/m-dictionary-item]

[m-dictionary-item name="D_FEATURE_4"]
  #### Extendable
  [Write your own shortcodes and components](/centre/material-design-made-easy-with-grav-cms-pro#components) from the scratch is really as easy as extending the ready ones that comes with **Centre**.
[/m-dictionary-item]

[m-dictionary-item name="D_FEATURE_5"]
  #### Deploy with Rocketeer
  [Rocketeer](http://rocketeer.autopergamene.eu/) is a modern PHP task runner and deployment package to send your website from your laptop to your deployment server just running a command.
[/m-dictionary-item]

[m-dictionary-item name="D_FEATURE_6"]
  #### Cache whole website
  A website that loads fast is a foundamental key for SEO. The [Warmup service](/centre/website-deployment-made-easy-with-rocketeer) parses all website pages caching them and having the website always fast to open.  
[/m-dictionary-item]

[m-dictionary-item name="D_CENTRE_REQUIREMENTS_TITLE"]
  ### Requirements
  ---
[/m-dictionary-item]

[m-dictionary-item name="D_CENTRE_REQUIREMENTS_1"]
  **Centre** is build on top of awesome Grav Content Management System, so, you need to meet that application demand. The only real required feature is **PHP 5.5.9 or higher**. You should keep yourself updated at [official documentation](https://learn.getgrav.org/basics/requirements).
[/m-dictionary-item]

[m-dictionary-item name="D_CENTRE_REQUIREMENTS_2"]
  You must maintain your website using [Git](https://git-scm.com) because it is used to deploy your website. An account at [Github](https://github.com/) or [Bitbucket](https://bitbucket.org/) is required., though this last one is probably the more indicated, because it offers private repositories for free.
[/m-dictionary-item]

[m-dictionary-item name="D_CENTRE_REQUIREMENTS_3"]
  The hoster where your website lives must provide a **SSH hosting**. This is also required for the website deploying. While there are tons of hosters out there, we are [Dreamhost](https://www.dreamhost.com/r.cgi?356893) satisfied customers, so we strongly encourage you to use their services.
[/m-dictionary-item]

[m-dictionary-item name="D_EXAMPLE_BOX_1"]
  ### An awesome jumbotron component {.h1-size}
  Scroll a little bit down and look how simple is adding a complex jumbotron like the one you see on the right to your web page.
[/m-dictionary-item]

[m-dictionary-item name="D_EXAMPLE_BOX_3"]
  ### Component frontend
  The following code renders a jumbotron with a nice black panel in the center that contains an intro text.
  [raw]
  ```
  [m-component
    component="jumbotron"
    folder="jumbotron"
    M_IMAGE="demo-image.jpg"
    M_PATH="images"
    M_HEIGHT="three-quarters"
    M_ATTRIBUTES="class:l10 offset-l1 m12 s12 opaque-panel-shades-black-medium padding-medium rounded text-full-white center"
  ]
    ### Anim pariatur
    Anim pariatur cliche reprehenderit enim eiusmod high life accusamus
  [/m-component]
  ```
  [/raw]
[/m-dictionary-item]

[m-dictionary-item name="D_EXAMPLE_BOX_4"]
  ### Component backend
  The component is simply a shortcode, you can use as it is or customize generating a new one.
  [raw]
  ```
  [m-jumbotron
    image-path="M_PATH"
    image="M_IMAGE"
    blurred-image="M_BLURRED_IMAGE"
    height="M_HEIGHT"
  ]
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
[/m-dictionary-item]

[m-dictionary-item name="D_EXAMPLE"]
  ### Centre in detail {.h1-size}
  Follows an example to show a real **Centre** component when it is rendered and the code used to generate it.
[/m-dictionary-item]

[m-dictionary-item name="D_INTERLUDE_1"]
  ### “Don't stand still! Come and find a powerful way to build websites” {.h1-size}
[/m-dictionary-item]

[m-dictionary-item name="D_SCREENCAST"]
  [m-link link-attributes="class: opaque opaque-reveal, name:screencast" icon="fa-link fa-flip-horizontal"][/m-link]
  ### Watch Centre in action {.h1-size }
  Watch the video to see what you can get from this application.
[/m-dictionary-item]

[m-dictionary-item name="D_VIDEO_1"]
  ### Build a website with Centre
[/m-dictionary-item]

[m-dictionary-item name="D_VIDEO_2"]
  ### Deploy a website with Centre  
[/m-dictionary-item]

[m-dictionary-item name="D_PRICE_TITLE"]
  [m-link link-attributes="class: opaque opaque-reveal, name:prices" icon="fa-link fa-flip-horizontal"][/m-link]
  ## Prices
  You can choose from several offers the best one to fit your needs. Feel free to try our application getting the Free Plan: you can upgrade to next paid plan any time.
[/m-dictionary-item]

[m-dictionary-item name="D_PRICES_TITLE_1"]
  FREE
[/m-dictionary-item]

[m-dictionary-item name="D_FREE_FOR_PERSONAL_USE"]
  **Free for personal use**. This license can be applied only to personal websites without any form of money entrance and cannot be used to sell a website created with our application. This plan is perfect both to try our application and to develop a personal website.
[/m-dictionary-item]

[m-dictionary-item name="D_PRICES_TITLE_2"]
  PERSONAL
[/m-dictionary-item]

[m-dictionary-item name="D_PRICES_TITLE_3"]
  ADVANCED
[/m-dictionary-item]

[m-dictionary-item name="D_PRICES_TITLE_4"]
  DEVELOPER
[/m-dictionary-item]

[m-dictionary-item name="D_BACKLINK_REQUIRED"]
  Backlink required
[/m-dictionary-item]

[m-dictionary-item name="D_NO_BACKLINK"]
  Backlink not required
[/m-dictionary-item]

[m-dictionary-item name="D_MONTH"]
  month
[/m-dictionary-item]

[m-dictionary-item name="D_YEAR"]
  year
[/m-dictionary-item]

[m-dictionary-item name="D_MEMBERSHIP"]
  months membership
[/m-dictionary-item]

[m-dictionary-item name="D_SITE_LICENSE"]
  site license
[/m-dictionary-item]

[m-dictionary-item name="D_UNLIMITED_LICENSE"]
  Unlimited licenses
[/m-dictionary-item]

[m-dictionary-item name="D_PREMIUM_THEMES"]
  Premium themes
[/m-dictionary-item]

[m-dictionary-item name="D_MATERIAL_PLUGIN"]
  Material plugin
[/m-dictionary-item]

[m-dictionary-item name="D_FULL_SHORTCODES"]
  Full shortcodes and components availability
[/m-dictionary-item]

[m-dictionary-item name="D_WARMUP"]
  Website warmup package
[/m-dictionary-item]

[m-dictionary-item name="D_ROCKETEER"]
  Rocketeer configuration
[/m-dictionary-item]

[m-dictionary-item name="D_ATOM"]
  Atom plugin
[/m-dictionary-item]

[m-dictionary-item name="D_ACCESS_ITEM_1"]
  Regular Plugin Release
[/m-dictionary-item]

[m-dictionary-item name="D_ACCESS_ITEM_2"]
  Regular Theme Release
[/m-dictionary-item]

[m-dictionary-item name="D_ACCESS_ITEM_3"]
  Regular Updates
[/m-dictionary-item]

[m-dictionary-item name="D_ACCESS_ITEM_4"]
  Full theme skeleton
[/m-dictionary-item]

[m-dictionary-item name="D_ACCESS_ITEM_5"]
  PHP, Sass javascript source files
[/m-dictionary-item]

[m-dictionary-item name="D_ACCESS_ITEM_6"]
  Email support
[/m-dictionary-item]

[m-dictionary-item name="D_ACCESS"]
  ### Membership provide access to:
[/m-dictionary-item]

[m-dictionary-item name="D_RELEASE"]
  ### Centre PRO release date November 2017{.h1-size}
  **Centre** free version will be released on July 2017, while Centre Pro will be released approximately on November 2017. Subscribe now and **get a 40% discount for the first year**, when it will be distributed.     
[/m-dictionary-item]

[m-dictionary-item name="D_JOB"]
  ### Get Centre for developers for free{.h1-size}
  ---
  We need some English mother language persons to hep us elaborating and proofreading all the contents of this website. You can apply for this position and, if you will get the job, you can get a **free Centre for developers copy**.

  Write us to **j.ob.s -at- gr.avc.ms.pro dot c.om** to get more details. (Please remove the dots)
[/m-dictionary-item]

[m-dictionary-item name="D_INTERLUDE_2"]
  ### “Take it easy and build websites like you've never done before” {.h1-size}
[/m-dictionary-item]
