[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Google map" shortcode
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_SHORTCODE

  [m-google-map id="map" zoom="10" center="41.895639,12.493415"]
    [m-google-map-marker location="41.895639,12.493415" title="Google map"]
      **Meet Us**
      We are there!
    [/m-google-map-marker]
  [/m-google-map]

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
      [m-help]
        Main component properties
        id: Defines the html id attribute
        zoom: Google map zoom attribute
        center: Google map center attribute
        Google map marker attributes
        location: Google map marker location attribute
        title: Google map marker title attribute
      [/m-help]
      [m-google-map id="map" zoom="10" center="41.895639,12.493415"]
        [m-google-map-marker location="41.895639,12.493415" title="Google map"]
          **Meet Us**
          We are there!
        [/m-google-map-marker]
      [/m-google-map]     
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

[/m-dictionary-item]
