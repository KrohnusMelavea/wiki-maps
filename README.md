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