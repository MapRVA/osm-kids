# OSM Kids

An [OpenStreetMap](https://openstreetmap.org)-powered map for kids! Featuring:

 * 🐟 Aquariums
 * 📗 Book Shops
 * 🍬 Candy Shops
 * 🚒 Fire Stations
 * 🍦 Ice Cream Shops
 * 📙 Libraries
 * 📘 Little Libraries
 * 🛝 Playgrounds
 * 🏊 Pools
 * 🎡 Theme Parks
 * 🏫 Schools
 * 🧸 Toy Shops
 * 🚂 Train Stations
 * 🏛️ Museums
 * 🐯 Zoos

It is currently an [Ultra](https://overpass-ultra.us)-powered prototype.

### View the map!

https://dschep.github.io/osm-kids/

### Build tiles
```
docker run -v "$(pwd)":/data ghcr.io/onthegomap/planetiler:latest generate-custom --schema=/data/osm-kids.planetiler.yml
```
