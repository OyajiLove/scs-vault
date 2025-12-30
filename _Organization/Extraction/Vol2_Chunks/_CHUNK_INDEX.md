# VOL 2 CHUNK FILES - DOWNLOAD PACKAGE

All 10 Vol 2 chunk files have been prepared and are available for download.

## Chunk Content Map

| Chunk | Lines | Primary Content | Key Systems |
|-------|-------|-----------------|-------------|
| 01 | 1-89 | Session continuity, Embry promo, Vol 1 recap, Good Hand start | Good Hand archetype |
| 02 | 90-178 | King's Road subtypes finalized (12), KR tags, FS vs KR philosophy | King's Road archetype, Match DNA |
| 03 | 179-267 | Dark Weavers archetype creation, subtype naming | Dark Weavers archetype |
| 04 | 268-356 | Character tags (Heat Sponge, Silver Tongue, etc.), Booking Behavior tags | Character Tags, Booking Tags |
| 05 | 357-445 | Database/spreadsheet work, trait library compilation | Database structure |
| 06 | 446-534 | "tovarisch" origin, Scandal Shielding System intro | Scandal System |
| 07 | 535-623 | Scandal Fallout system, damage severity by response | Scandal Fallout mechanics |
| 08 | 624-712 | Hidden Tags system (traits hidden until exposed) | Hidden Tags system |
| 09 | 713-801 | Weather Risk system, Adaptability skill | Weather Risk, Adaptability |
| 10 | 802-887 | Match engine inputs, booking philosophy settings | Match Engine, Booking Philosophy |

## File Sizes
- chunk_01.txt: 72KB
- chunk_02.txt: 54KB
- chunk_03.txt: 67KB
- chunk_04.txt: 91KB
- chunk_05.txt: 92KB
- chunk_06.txt: 67KB
- chunk_07.txt: 77KB
- chunk_08.txt: 83KB
- chunk_09.txt: 75KB
- chunk_10.txt: 92KB

## Source Location
Full source: `C:\Users\Oyaji\Desktop\SCS\_Main Volume PDFs\txt_conversions\SCS Vol. 2.txt`

## Processing Instructions
Each chunk should be processed in a separate thread:
1. Pull chunk content using: `sed -n 'START,ENDp' "SCS Vol. 2.txt"`
2. Extract mechanics line-by-line
3. Update relevant Bible entries
4. Mark tracker complete

## Download
Files are available in the outputs folder for manual copy to vault if needed.
