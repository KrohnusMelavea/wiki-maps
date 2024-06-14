# wiki-maps

## .wikinode file format:
- Node URL: char[], NULL
- Neighbour URLS: char[], NULL, repeated until EOF

## wikinode_intermediate struct format:
- Node URL: stl::dynamic_array<char>
- Neighbour URLs: stl::dynamic_array<stl::dynamic_array<char>>