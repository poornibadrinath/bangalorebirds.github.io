<!DOCTYPE html>
<html>
<head>
    <meta charset='utf-8' />
    <title>Bangalore Birds</title>
    <meta name='viewport' content='initial-scale=1,maximum-scale=1,user-scalable=no' />
    <script src='https://api.tiles.mapbox.com/mapbox-gl-js/v0.21.0/mapbox-gl.js'></script>
    <link href='https://api.tiles.mapbox.com/mapbox-gl-js/v0.21.0/mapbox-gl.css' rel='stylesheet' />
    <style>
        body { margin:0; padding:0; }
        #map { position:absolute; top:0; bottom:0; width:100%; }
    </style>
</head>
<body>

<script src='https://api.mapbox.com/mapbox-gl-js/plugins/mapbox-gl-directions/v2.1.0/mapbox-gl-directions.js'></script>
<link rel='stylesheet' href='https://api.mapbox.com/mapbox-gl-js/plugins/mapbox-gl-directions/v2.1.0/mapbox-gl-directions.css' type='text/css' />
<style>
    .mapboxgl-popup {
        max-width: 400px;
        font: 12px/20px 'Helvetica Neue', Arial, Helvetica, sans-serif;
    }
</style>
<div id='map'></div>
<script>
mapboxgl.accessToken = 'pk.eyJ1IjoicG9vcm5pLWJhZHJpbmF0aCIsImEiOiJjaWVoOGFiNWUwMDl2c3JtMXBzcWluaDN5In0.uunHEpdx8grTpnmTwTwxHA';

var map = new mapboxgl.Map({
    container: 'map',
    style: 'mapbox://styles/poorni-badrinath/ciptdm1z6002kdbnnkdbz76p1',
    center: [77.6136,12.9946],
    dragPan: true,
    hash: true
});
var tourismgeojson = {
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "properties": {
        "name": "Lal Bagh",
        "leisure": "park",
          "image":"http://3.bp.blogspot.com/-lJpuxZfl6O0/VOm7ihU8PyI/AAAAAAAAAUI/d-nS2_s3FkU/s1600/kempe-gowda-tower-lalbagh1.jpg"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.5852, 
          12.94903
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/784255233",
      "properties": {
        "name": "Madivala Lake",
        "natural": "lake",
          "image":"http://2.bp.blogspot.com/-wst1EApb2lA/UmyZ2n0sewI/AAAAAAAAC3c/gXYar5CtISU/s1600/IMG_3310.JPG"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.6154, 
          12.9153
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/245641840",
      "properties": {
        "name": "Hebbal Lake",
        "natural": "Lake",
        "image":"https://static.strollup.in/image/location/Hebbal%20Lake/main-1347543.jpg"
        
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.5884, 
          13.0471
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/784234009",
      "properties": {
        "amenity": "school",
        "name": "Valley School",
          "image":"https://upload.wikimedia.org/wikipedia/commons/1/1e/Banyan_Tree_at_The_Valley_School_,_Bangalore.JPG"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.5065513,
          12.8535265
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/784255233",
      "properties": {
        "name": "Manchinabele",
        "tourism": "attraction",
          "image":"http://www.365hops.com/searching_files/timthumb.php?src=http://www.365hops.com/social/event_gallery/1459812634.Manchinbele-Dam-Bangalore2-e1420530455279.jpg&h=380&w=650&zc=1"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.3569, 
          12.885
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/784255233",
      "properties": {
        "name": "Hesaraghatta Grasslands",
        "tourism": "attraction",
          "image":"https://s-media-cache-ak0.pinimg.com/736x/df/54/78/df54789064c07a7c737c1c2b0f6ffc28.jpg"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.4849, 
          13.1574
        ]
      }
    },
     {
      "type": "Feature",
      "id": "node/784255233",
      "properties": {
        "name": "Devarayanadurga State Forest",
        "tourism": "attraction",
          "image":"http://1.bp.blogspot.com/-DP3x12GGYEM/TdZLNh3O_vI/AAAAAAAADnk/KtnIUGG-ZVM/s1600/220655_10150162552416207_675286206_7121753_4958175_o%25281%2529.jpg"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.200917, 
          13.3745789
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Tippagondanahalli Reservoir",
        "natural": "lake",
          "image":"http://1.bp.blogspot.com/-RJdZlf0mwxw/ViX17N79JuI/AAAAAAAAA9c/XFrjYdutgUU/s1600/tg%2Bdam2.JPG"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.2973099, 
          12.978683
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Bannerghatta National Park",
        "natural": "lake",
          "image":"https://media-cdn.tripadvisor.com/media/photo-s/08/7f/ac/72/bannerghatta-national.jpg"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.5713, 
          12.7782
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Indian Institute of Science",
        "amenity": "university",
          "image":"http://images.shiksha.com/mediadata/images/1452505221phpAuehqz.jpeg"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.5699, 
          13.0193
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Gulakmale Lake",
        "natural": "lake",
          "image":"https://i.ytimg.com/vi/PLc37vOysfY/maxresdefault.jpg"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.5260101, 
          12.8065567
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Nandi Hills",
        "tourism": "attraction",
          "image":"http://www.nikhilchandra.in/wp-content/uploads/2014/02/nandi-hills-bangalore.jpg"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.6807, 
          13.3749
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Puttenahalli Lake",
        "natural": "lake",
          "image":"http://s3-ap-southeast-1.amazonaws.com/media.thrillophilia.com/site/rich/rich_files/rich_files/000/009/836/original/puttenahalli-20lake-20by-20sandeep-20shande.jpg"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.58698, 
          12.8912
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Cubbon Park",
        "leisure": "park",
          "image":"http://www.miss-wanderlust.com/wp-content/uploads/2015/05/cubbon-park-1.jpg"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.5922, 
          12.9744
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Turahalli Forest",
        "tourism": "attraction",
          "image":"http://www.culturebowl.com/wp-content/uploads/2016/02/03.jpg"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.5161, 
          12.9056
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/1068785214",
      "properties": {
        "name": "Hosakote",
        "tourism": "attraction",
          "image":"https://static2.tripoto.com/media/filter/m/img/209106/TripDocument/1451469535_image.jpeg"

      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.7728, 
          13.0786 
        ]
      }
    },
    {
      "type": "Feature",
      "id": "node/2900563447",
      "properties": {
        "name": "Ulsoor Lake",
        "natural": "lake",
        "image":"https://c2.staticflickr.com/6/5216/5392925868_5cb5586c52_b.jpg"
      },
      "geometry": {
        "type": "Point",
        "coordinates": [
          77.6179, 
          12.9812
        ]
      }
    }
  ]
};



    map.on('load', function () {
    map.addSource("points", {
        "type": "geojson",
        "data": tourismgeojson


    });

    map.addLayer({
        "id": "points",
        "type": "symbol",
        "source": "points",
        "layout": {
            "icon-image": "garden-15",
            // "text-field": "{title}",
            "text-font": ["Open Sans Semibold", "Arial Unicode MS Bold"],
            "text-offset": [0, 0.6],
            "text-anchor": "top"
        }
    });
});
var popup = new mapboxgl.Popup({
    closeButton: false,
    closeOnClick: false
});


map.on('click', function(e) {
    var features = map.queryRenderedFeatures(e.point, { layers: ['points'] });
    // Change the cursor style as a UI indicator.
    map.getCanvas().style.cursor = (features.length) ? 'pointer' : '';

    if (!features.length) {
        popup.remove();
        return;
    }

    var popupLocation;
  var feature = features[0];
    //Get point location of feature
    if( feature.geometry.type == 'Polygon'){
      popupLocation = feature.geometry.coordinates[0][0];
    }else{
      popupLocation = feature.geometry.coordinates
    }



    // Populate the popup and set its coordinates
    // based on the feature found.
    if(feature.properties["name"]!=undefined){

      popup.setLngLat(popupLocation)
          .setHTML(feature.properties["name"]+' <br> <img src="' + feature.properties["image"] + '"style="height:100px;">')
          .addTo(map);


    } else {
      popup.setLngLat(popupLocation)
          .setHTML(feature.properties.name)
          .addTo(map);

    }
  });
  map.addControl(new mapboxgl.Navigation());
  map.addControl(new mapboxgl.Directions());
</script>

</body>
</html>