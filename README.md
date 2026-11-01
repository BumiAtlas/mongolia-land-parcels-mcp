# Mongolia Land Parcels MCP (eGazar cadastre · Газрын нэгж талбар)

[Монгол хэлээр](#монгол-хэлээр)

Connect your AI assistant (Claude, ChatGPT, Cursor) to [BumiAtlas](https://bumiatlas.com) for Mongolian land research through the Model Context Protocol (MCP).

This listing is a focused entry point for:

- All ~1.37M current land parcels from ALAMGaC's eGazar cadastre (Agency for Land Administration and Management, Geodesy and Cartography): Ulaanbaatar and aimag centres, ger districts, summer-house (dacha) areas, farmland and herders' winter and spring camps
- Parcel lookup by 10-digit parcel id (old ids from before a split or merge work too), by address in Mongolian Cyrillic (street, khashaa number, neighbourhood), or by coordinates
- The national land-use class (in Mongolian, with English names for the common classes), recorded area, address, district code and the date the parcel took effect
- Satellite and street map images of a parcel and its neighbours, labelled by parcel id

Parcels have no owner, title or price information. Open pasture is mostly not parcelled.

## Connect

```
https://bumiatlas.com/mcp/mongolia
```

Add it as a custom connector in any MCP client and sign in with Google. Tools, examples and data notes: [bumiatlas.com/mcp-docs/mongolia](https://bumiatlas.com/mcp-docs/mongolia).

- **Claude:** Settings → Connectors → Add custom connector, paste the URL, then Connect.
- **ChatGPT:** Settings → Apps & Connectors → Advanced → Developer mode, then Create with the URL and OAuth authentication.

## Tools

| Tool | Description |
|---|---|
| `MN_parcel_search` | Find parcels by parcel id, Cyrillic address words (street, khashaa, neighbourhood; narrow by district code), or `latitude, longitude`; each result is the whole record, with the boundary as GeoJSON on request |
| `MN_parcel_image` | Satellite or street map image of a parcel or point, with every parcel in view outlined and labelled with its parcel id |

## Example prompts

- *"What parcels are at 47.9186, 106.9177 in Ulaanbaatar, and what are they used for?"*
- *"Find the parcel on Гүш street, khashaa 102."*
- *"Look up parcel 4101020014 and show it on satellite imagery."*
- *"Is the land at this point a ger yard, a summer-house plot or farmland?"*

## Data source

Parcels © ALAMGaC (Agency for Land Administration and Management, Geodesy and Cartography), Mongolia, from the public eGazar map. A copy of public data for research, not a legal land record.

## Монгол хэлээр

Хиймэл оюуны туслахаа (Claude, ChatGPT, Cursor) Model Context Protocol (MCP)-оор [BumiAtlas](https://bumiatlas.com)-тай холбож, Монгол Улсын газрын нэгж талбарын мэдээллийг хайна.

- ГЗБГЗЗГ-ын eGazar кадастрын одоо хүчинтэй ~1.37 сая нэгж талбар: Улаанбаатар болон аймгийн төвүүд, гэр хороолол, зуслан, тариалангийн газар, өвөлжөө, хаваржаа
- Нэгж талбарын дугаар (10 оронтой), хаяг (гудамж, хашааны дугаар, хороолол) эсвэл солбицлоор хайх
- Газрын зориулалт, талбай, хаяг, хүчинтэй болсон огноо; хиймэл дагуулын зураг дээр хөрш талбаруудын хамт

Өмчлөгч, гэрчилгээ, үнийн мэдээлэл агуулаагүй.

**Холбох:** `https://bumiatlas.com/mcp/mongolia` хаягийг MCP дэмждэг программд custom connector болгон нэмээд Google-ээр нэвтэрнэ. Хэрэгслийн нэр англиар байсан ч туслах монголоор хариулж чадна.

Жишээ асуултууд:

- *"Улаанбаатарт 47.9186, 106.9177 солбицолд ямар нэгж талбар байна, ямар зориулалттай вэ?"*
- *"Гүш гудамж, 102 тоот хашааны нэгж талбарыг ол."*
- *"4101020014 дугаартай нэгж талбарыг хиймэл дагуулын зураг дээр харуул."*
