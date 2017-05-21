[m-dictionary-item name="D_HEADER_JUMBOTRON"]
  # "Map" component
[/m-dictionary-item]

[m-dictionary-item name="D_MAIN_CONTENT"]
  D_COMPONENT

  [m-component component="map" folder="contacts-and-position" M_CONTAINER="false"]
    [m-component-item name="M_INCIPIT" M_COLUMNS="s12 m12 l12" M_CENTER="center" M_EXTRA_ATTRIBUTES=""]
      ### Come and find us
      ---
      Anim pariatur cliche reprehenderit enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch.
    [/m-component-item]
    [m-component-item name="M_MAP" M_COLUMNS="s12 m12 l12" M_API_KEY="999999999-999999999" M_ZOOM="10" M_POINT_CENTER="41.895639,12.493415" M_POINT_LOCATION="41.895639,12.493415" M_TITLE="Marker title"]
      Add a content for the marker
    [/m-component-item]
  [/m-component]  

  D_CODE

  [m-tag tag="div" attributes="id:code"]
    [raw]
    ```
    [m-help]
      Main component properties
      M_CONTAINER: When true contains and centers the component grid

      Item component properties
      M_COLUMNS: Defines the size for all the item's columns
      M_CENTER: Sets the text alignment. This parameter accepts the following values: left, center, right
      M_EXTRA_ATTRIBUTES: Adds extra html attributes to class element. to add an extra foo class and a new rel attribute, you can define this parameter as follows: M_EXTRA_ATTRIBUTES="foo, rel=bar

      Google Map component properties
      M_API_KEY: Api key provided by Google
      M_ZOOM: Initial map zoom
      M_POINT_CENTER: Initial map point center
      M_POINT_LOCATION: Initial map point location
      M_TITLE: Map title displayed when the user clicks the marker
    [/m-help]
    [m-component component="map" folder="contacts-and-position" M_CONTAINER="true"]
      [m-component-item name="M_INCIPIT" M_COLUMNS="s12 m12 l12" M_CENTER="center" M_EXTRA_ATTRIBUTES=""]
        ### Come and find us
        ---
        Anim pariatur cliche reprehenderit enim eiusmod high life accusamus terry richardson ad squid. 3 wolf moon officia aute, non cupidatat skateboard dolor brunch.
      [/m-component-item]
      [m-component-item name="M_MAP" M_COLUMNS="s12 m12 l12" M_API_KEY="999999999-999999999" M_ZOOM="10" M_POINT_CENTER="41.895639,12.493415" M_POINT_LOCATION="41.895639,12.493415" M_TITLE="Marker title"]
        Add a content for the marker
      [/m-component-item]
    [/m-component]    
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]

  D_THE_CODE_COMPONENT

  [m-tag tag="div" attributes="id:component-code"]
    [raw]
    ```
    [m-grid container="M_CONTAINER" attributes="M_ATTRIBUTES"]
      [m-grid-row]
        [m-grid-col attributes="class:M_INCIPIT.M_COLUMNS M_INCIPIT.M_CENTER M_INCIPIT.M_EXTRA_ATTRIBUTES"]
          M_INCIPIT.M_CONTENT
        [/m-grid-col]
      [/m-grid-row]

      [m-grid-row]
        [m-grid-col attributes="class:M_MAP.M_COLUMNS"]
          [m-google-map id="M_MAP.M_ID" zoom="M_MAP.M_ZOOM" center="M_MAP.M_POINT_CENTER" api-key="M_MAP.M_API_KEY"]
            [m-google-map-marker location="M_MAP.M_POINT_LOCATION" title="M_MAP.M_TITLE"]
              M_MAP.M_CONTENT
            [/m-google-map-marker]
          [/m-google-map]
        [/m-grid-col]
      [/m-grid-row]
    [/m-grid]
    ```
    [/raw]
  [/m-tag]  

  [m-clipboard target-id="component-code" button-label="Copy to clipboard" icon="content_copy" icon-attributes="class:left"][/m-clipboard]
[/m-dictionary-item]
