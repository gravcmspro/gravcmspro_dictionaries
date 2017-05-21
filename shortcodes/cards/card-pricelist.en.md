[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Pricelist card" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-grid container="false"]
    [m-grid-row]
      [m-grid-col attributes="class:s12 m4 l4"]
        [m-card-pricelist title="BASIC" subtitle="99 €/year" price="8,25 €/month*"]
          [m-card-pricelist-item]Feature 1[/m-card-pricelist-item]
          [m-card-pricelist-item]Feature 2[/m-card-pricelist-item]
          [m-card-pricelist-item]Feature 3[/m-card-pricelist-item]
          [m-card-pricelist-item]Feature 4[/m-card-pricelist-item]
          [m-card-pricelist-item]Feature 5[/m-card-pricelist-item]
        [/m-card-pricelist]        
      [/m-grid-col]
    [/m-grid-row]
  [/m-grid]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      title: sets the card's title
      subtitle: sets the card's subtitle
      price: sets the card's price
      attributes: Adds html attributes to element. Example attributes="class: foo, rel=bar"
      button-url: defines the button url
      button-label: defines the button label
    [/m-help]
    [m-card-pricelist title="BASIC" subtitle="99 €/year" price="8,25 €/month*"]
      [m-card-pricelist-item]Feature 1[/m-card-pricelist-item]
      [m-card-pricelist-item]Feature 2[/m-card-pricelist-item]
      [m-card-pricelist-item]Feature 3[/m-card-pricelist-item]
      [m-card-pricelist-item]Feature 4[/m-card-pricelist-item]
      [m-card-pricelist-item]Feature 5[/m-card-pricelist-item]
    [/m-card-pricelist]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
