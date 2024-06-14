# wiki-maps

## .wikinode file format:
- URL: `char[], NULL`
- Neighbour URLS: `char[], NULL` repeated until EOF

## wikinode_staging struct format:
- URL: `std::string`
- Neighbour URLs: `stl::dynamic_array<std::string>`

## wiknode struct format:
- URL: `std::string`
- Neighbours: `stl::dynamic_array<wikinode*>`

## Initial Load Procedure:
- Load all .wikinode files into a `std::unordered_map<std::string, wikinode_staging>` staging map. The key is the node' URL. Assume no changes have been made to the wiki pages during the downtime