# :world_map: OSM Kids

An [OpenStreetMap](https://openstreetmap.org)-powered map for kids! Featuring:

 * 🐟 Aquariums
 * 📗 Book Shops
 * 🌻 Botanic Gardens
 * 🍬 Candy Shops
 * 🚒 Fire Stations
 * ♟️ Game Shops
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
 * 🕹️ Video Game Shops
 * 🐯 Zoos

At middle zoom levels it shows cities 🏙️, and at low zooms it shows countries 🏙️🇫🇷🇨🇲🇨🇳.

### View the map!

https://dschep.github.io/osm-kids/

### Build tiles
```
docker run -v "$(pwd)":/data ghcr.io/onthegomap/planetiler:latest generate-custom --schema=/data/osm-kids.planetiler.yml
```
