<!DOCTYPE html>
<html>
<head>
    <title>Peta Magelang</title>
    <meta charset="utf-8" />
    <link rel="stylesheet" href="https://unpkg.com/leaflet/dist/leaflet.css" />
    <script src="https://unpkg.com/leaflet/dist/leaflet.js"></script>

    <style>
        .legend {
            background: white;
            padding: 10px;
            line-height: 20px;
            color: #333;
            border-radius: 6px;
            box-shadow: 0 0 15px rgba(0,0,0,0.2);
            font-size: 14px;
            max-height: 350px;
            overflow-y: auto;
        }
        .legend i {
            width: 18px;
            height: 18px;
            float: left;
            margin-right: 8px;
            opacity: 0.85;
        }
        .legend h4 {
            margin: 0 0 10px 0;
            font-size: 15px;
            text-align: left;
        }
    </style>
</head>
<body>

<div id="map" style="width:100%; height:650px;"></div>

<script>
// MAP
var map = L.map("map").setView([-7.47, 110.21], 11);

// ======================================================
// BASEMAPS
// ======================================================

// OpenStreetMap
var osm = L.tileLayer("https://{s}.tile.openstreetmap.org/{z}/{x}/{y}.png", {
    maxZoom: 19
}).addTo(map);

// Esri World Imagery (Satelit)
var esri = L.tileLayer(
    "https://server.arcgisonline.com/ArcGIS/rest/services/World_Imagery/MapServer/tile/{z}/{y}/{x}"
);

// Google Maps - Road ONLY
var gRoad = L.tileLayer(
    "http://{s}.google.com/vt/lyrs=m&x={x}&y={y}&z={z}",
    { maxZoom: 20, subdomains: ['mt0','mt1','mt2','mt3'] }
);

// ======================================================
// WMS LAYERS
// ======================================================

// Kecamatan
var kecamatan = L.tileLayer.wms("http://localhost:8080/geoserver/pg_web/wms", {
    layers: "pg_web:Magelang_Kecamatan",
    format: "image/png",
    transparent: true
}).addTo(map);

// Jalan
var jalan = L.tileLayer.wms("http://localhost:8080/geoserver/pg_web/wms", {
    layers: "pg_web:Magelang_Jalan",
    format: "image/png",
    transparent: true
}).addTo(map);

// Sungai
var sungai = L.tileLayer.wms("http://localhost:8080/geoserver/pg_web/wms", {
    layers: "pg_web:Magelang_Sungai",
    format: "image/png",
    transparent: true
}).addTo(map);

// Titik Kecamatan
var titik = L.tileLayer.wms("http://localhost:8080/geoserver/pg_web/wms", {
    layers: "pg_web:data_kecamatan_magelang",
    format: "image/png",
    transparent: true
});

// ======================================================
// CONTROL LAYERS
// ======================================================
L.control.layers(
    {
        "OpenStreetMap": osm,
        "Esri World Imagery (Satelit)": esri,
        "Google Maps - Road": gRoad
    },
    {
        "Kecamatan": kecamatan,
        "Jalan": jalan,
        "Sungai": sungai,
        "Titik Kecamatan": titik
    }
).addTo(map);

// ======================================================
// LEGEND FINAL
// ======================================================
var legend = L.control({ position: "bottomleft" });

legend.onAdd = function (map) {
    var div = L.DomUtil.create("div", "legend");
    div.innerHTML += "<h4>Legenda</h4>";

    // Kecamatan colors
    var kecItems = [
        {color:"#37A6D7", name:"Bandongan"},
        {color:"#5E33BF", name:"Borobudur"},
        {color:"#17D84F", name:"Candimulyo"},
        {color:"#9FEA73", name:"Dukun"},
        {color:"#C76C6A", name:"Grabag"},
        {color:"#B0663D", name:"Kajoran"},
        {color:"#46F7E1", name:"Kaliangkrik"},
        {color:"#1E2CBF", name:"Mertoyudan"},
        {color:"#6AC523", name:"Mungkid"},
        {color:"#8BE2C2", name:"Muntilan"},
        {color:"#9BA83C", name:"Ngablak"},
        {color:"#9B0FAF", name:"Ngluwar"},
        {color:"#213DBF", name:"Pakis"},
        {color:"#0600B4", name:"Salam"},
        {color:"#CC4F76", name:"Salaman"},
        {color:"#F51AD1", name:"Sawangan"},
        {color:"#DF8B7A", name:"Secang"},
        {color:"#8AE537", name:"Srumbung"},
        {color:"#C9A24E", name:"Tegalrejo"},
        {color:"#C79F0A", name:"Tempuran"},
        {color:"#D819CB", name:"Windusari"}
    ];

    div.innerHTML += "<b>Kecamatan:</b><br>";
    kecItems.forEach(function(item){
        div.innerHTML +=
            '<i style="background:' + item.color + ';"></i> ' +
            item.name + "<br>";
    });

    // Jalan
    div.innerHTML += "<br>";
    div.innerHTML +=
        '<i style="background:#f7e72b; width:25px; height:4px; margin-top:8px;"></i> ' +
        'Magelang_Jalan<br>';

    // Sungai
    div.innerHTML +=
        '<i style="background:#4c4fb9; width:25px; height:4px; margin-top:8px;"></i> ' +
        'Magelang_Sungai<br>';

    // Titik Kecamatan
    div.innerHTML +=
        '<i style="background:#ff0000; width:10px; height:10px; margin-top:4px;"></i> ' +
        'Titik Kecamatan<br>';

    return div;
};

legend.addTo(map);

</script>

</body>
</html>
