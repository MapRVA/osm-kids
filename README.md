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

https://osm.kids/


### Build the map from the Ultra query
```
npm i
npm run build
```

### Build tiles
```
npm run build:tiles
```

If you need `sudo` to run docker:
```
npm run build:tiles:sudo
```

### Adding a new type of place to the map

To add a new type of place:

* Edit [`osm-kids.planetiler.yml`](./osm-kids.planetiler.yml) to add a secion in `features`.
    * Use the `include_when` section to define what OSM objects to include
    * Include a sprite attribute in the form `emoji:short_name` where `short_name` is an emoji
      short name. See http://projects.iamcal.com/emoji-data/table.htm for short names.
    * Choose `min_zoom` and `sort` that is appropriate.
    * If it has a name, include the `- key: name` attribute,
* Add it to this README
* Update the legend in [`osm-kids.ultra`](./osm-kids.ultra)
