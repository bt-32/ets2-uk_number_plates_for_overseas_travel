# UK Number Plate Overhaul (ETS2 mod)

This mod for Euro Truck Simulator 2 overhauls the number (license) plates for the United Kingdom (UK) to be more realistic and true-to-life. It is perfect for anyone who likes realism, such as myself.

The features of this mod are:

- **Local memory tags (first two letters):** updated to be accurate across each UK city.
- **Age identifier (year in the middle):** expanded to include all combinations from 2001 ("51") to present ("75").
- **Three-letter sequence (final three letters):** updated to include "Z" per real life.
- **Country identifier:** changed from "GB" to "UK" and removed the blue flash.

This mod is also available on [Steam](https://steamcommunity.com/sharedfiles/filedetails/?id=3384424807).

## Local memory tags

These are the first two letters of the plate. They are based on the region where the vehicle was registered (e.g. "BT" is one of many tags for Birmingham). This mod updates the country and city definitions for the UK to generate accurate local memory tags for both generic UK traffic and city-specific UK traffic.

**With this mod:**

- AI traffic cars have a 50% chance to receive a local memory tag for the current in-game city, otherwise they will receive a random UK one.
- AI traffic trucks and trailers will always receive a random UK local memory tag.
- Truck and trailer purchases or relocations by the player will always receive a local memory tag for the target garage's city.

The mappings used by this mod are:

| In-game city | First letter | Real-life region used for first letter  | Real-life office(s) used for second letters | Second letters                                |
| ------------ | ------------ | --------------------------------------- | ------------------------------------------- | --------------------------------------------- |
| Aberdeen     | **S**        | **S**cotland                            | Aberdeen                                    | V W                                           |
| Birmingham   | **B**        | **B**irmingham                          | Birmingham                                  | A B C D E F G H J K L M N O P R S T U V W X   |
| Cambridge    | **A**        | **A**nglia                              | Peterborough                                | A B C D E F G J K M N                         |
| Cardiff      | **C**        | **C**ymru (Wales)                       | Cardiff                                     | A B C D E F G H J K L M N O                   |
| Carlisle     | **P**        | **P**reston                             | Carlisle                                    | U V W X Y                                     |
| Dover        | **G**        | **G**arden of England                   | Maidstone                                   | A B C D E F G H J K L M N                     |
| Edinburgh    | **S**        | **S**cotland                            | Edinburgh                                   | K L M N O                                     |
| Felixstowe   | **A**        | **A**nglia                              | Ipswich                                     | V W X Y                                       |
| Glasgow      | **S**        | **S**cotland                            | Glasgow                                     | A B C D E F G H J                             |
| Grimsby      | **F**        | **F**orest and **F**ens                 | Lincoln                                     | R S T V W X Y                                 |
| Harwich      | **A**        | **A**nglia                              | Ipswich                                     | V W X Y                                       |
| Hull         | **Y**        | **Y**orkshire                           | Beverley                                    | W X Y                                         |
| Liverpool    | **M**        | **M**anchester and **M**erseyside       | Manchester                                  | A B C D E F G H J K L M P T U V W X           |
| London       | **L**        | **L**ondon                              | Wimbledon + Borehamwood + Sidcup            | A B C D E F G H J K L M N O P R S T U V W X Y |
| Manchester   | **M**        | **M**anchester and **M**erseyside       | Manchester                                  | A B C D E F G H J K L M P T U V W X           |
| Newcastle    | **N**        | **N**ewcastle                           | Newcastle + Stockton                        | A B C D E G H J K L M N O P R S T U V W X Y   |
| Plymouth     | **W**        | **W**est of England                     | Exeter + Truro                              | A B D E F G H J K L                           |
| Sheffield    | **Y**        | **Y**orkshire                           | Sheffield                                   | M N O P R S T U V                             |
| Southampton  | **H**        | **H**ampshire, Dorset and Isle of Wight | Portsmouth                                  | K L M N P R S T U V X Y                       |
| Swansea      | **C**        | **C**ymru (Wales)                       | Swansea                                     | P R S T U V                                   |

Source: [Wikipedia](https://en.wikipedia.org/wiki/Vehicle_registration_plates_of_the_United_Kingdom#Local_memory_tags)

## Age identifier

These are the two numbers in the middle of the plate. They are the last two digits of the year itself (for registrations between March and August) or 50 added to that value (for registrations between September and February of the following year).

The default game limits the age identifiers to the range from "09" to "67". This mod extends age identifiers to the full set from 2001 ("51") to present ("75"). I will aim to update this mod as each new age identifier begins to be issued in reality, twice per year.

**With this mod:**

- AI traffic vehicles always receive a random age identifier.
- Truck and trailer purchases or relocations by the player will always receive the newest age identifier (currently "75").

The age identifiers used by this mod are:

```
51, 02, 52, 03, 53, 04, 54, 05, 55, 06, 56, 07, 57, 08, 58, 09, 59, 10, 60, 11, 61, 12, 62, 13, 63, 14, 64, 15, 65, 16, 66, 17, 67, 18, 68, 19, 69, 20, 70, 21, 71, 22, 72, 23, 73, 24, 74, 25, 75
```

In real life, vehicles can have a plate that is older than the vehicle but not one that is newer. In the game, plate generation cannot (that I am aware of) be based on vehicle age. Therefore, we will just have to collectively agree to suspend our disbelief (or modify our saves) when, for example, a 20 year old car model is assigned a plate from the 2020s, or our aging DAF gets a brand new plate because we moved it to another city.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Vehicle_registration_plates_of_the_United_Kingdom#Age_identifiers)

## Three-letter sequence

These are the final three letters of the plate. In real life, "I" and "Q" are not permitted. However, the default game also does not allow "Z" in this section, which is inaccurate.

**With this mod:**

- "Z" can be generated into the final three letters of UK number plates.
- "I" and "Q" remain not permitted.

Source: [Wikipedia](https://en.wikipedia.org/wiki/Vehicle_registration_plates_of_the_United_Kingdom#Characters)

## Country identifier

Since 28th September 2021, the country identifier "GB" on a blue background - while still legal within the UK on already-issued plates - is no longer valid for overseas travel.

The valid overseas specification is:

- The letters "UK" in royal blue, matching the blue in the Union Flag.
- The Union Flag (also known as the Union Jack) in landscape in specific colours.
- A background that is the same colour as the number plate (white for front, yellow for rear).
- Like all other flags and flashes, the flag must be positioned to the far-left side of the number plate.

**With this mod:**

- The country identifier is changed from "GB" to "UK".
- The blue flash (background on the left of the plate) is removed.

If you're SUPER keen for realism, remember that UK vehicles traveling in Spain, Cyprus and Malta must still show a UK sticker, regardless of what plate(s) they have.

Source: [British Number Plate Manufacturers Association](https://www.bnma.org/news/uk-flag-number-plate-design-confirmed-for-overseas-travel/)
