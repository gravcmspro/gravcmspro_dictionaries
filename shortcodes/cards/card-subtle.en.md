[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Card subtle" shortcode (PRO)
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l6"]
        [m-subtle-card effect="effect-4" image="image.jpg" card-title="Effect 4" card-subtitle="Product subtitle" card-button-url="#" card-button-label="More"]
        [/m-subtle-card]               
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      image: The image name with the extension. Set a blank value for no image
      image-path: The image directory
      image-title: The image title attribute
      image-alt: The image alt attribute. This parameter is mandatory and cannot be blank
      effect: The effect to apply to subtle card.  here are are seven effects available you can choose from: effect-[1-7]
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"
    [/m-help]
    [m-subtle-card effect="effect-4" image="image.jpg" card-title="Product name" card-subtitle="Product subtitle" card-button-url="#" card-button-label="More"]
    [/m-subtle-card]          
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  ## Other effects
  Please watch all the awesome available effects for this component. Just change the **effect** property to apply the best one for your needs.
  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l6"]
        ### Effect 1
        [m-subtle-card effect="effect-1" image="image.jpg" card-title="Effect 1" card-subtitle="Product subtitle" card-button-url="#" card-button-label="More"]
        [/m-subtle-card]                  
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m12 l6"]
        ### Effect 2
        [m-subtle-card effect="effect-2" image="image.jpg" card-title="Effect 2" card-subtitle="Product subtitle" card-button-url="#" card-button-label="More"]
        [/m-subtle-card]                
      [/m-grid-col]      
    [/m-grid-row]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l6"]
        ### Effect 3
        [m-subtle-card effect="effect-3" image="image.jpg" card-title="Effect 3" card-subtitle="Product subtitle" card-button-url="#" card-button-label="More"]
        [/m-subtle-card]
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m12 l6"]
        ### Effect 5
        [m-subtle-card effect="effect-5" image="image.jpg" card-title="Effect 5" card-subtitle="Product subtitle" card-button-url="#" card-button-label="More"]
        [/m-subtle-card]                  
      [/m-grid-col]
    [/m-grid-row]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m12 l6"]
        ### Effect 6
        [m-subtle-card effect="effect-6" image="image.jpg" card-title="Effect 6" card-subtitle="Product subtitle" card-button-url="#" card-button-label="More"]
        [/m-subtle-card]                  
      [/m-grid-col]
      [m-grid-col attributes="class:s12 m12 l6"]
        ### Effect 7
        [m-subtle-card effect="effect-7" image="image.jpg" card-title="Effect 7" card-subtitle="Product subtitle" card-button-url="#" card-button-label="More"]
        [/m-subtle-card]                
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  
[/m-dictionary-item]
