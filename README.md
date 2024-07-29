## Folder structure

- "Redrawn" covers both Vanilla and SVE games
- "Expanded" covers SVE files only
- "East Scarp" covers East Scarp files for Vanilla and SVE games

## UniqueIDs
- Main: `grapeponta.VibrantPastoralRecolor`
- C# config: `VibrantPastoral.C`
- SVE: `VibrantPastoral.Expanded`
- East Scarp: `VibrantPastoral.EastScarp`

## Documentations

- [ ] i18n description for the settings in game
- [ ] Write down which setting change what (preferably with images for easier navigation)
- [ ] Since we are changing global option to C#, write instruction to reload asset when user change it (either by sleeping for a day or use patch update/patch reload)

## Assets
- [ ] Merge original VPR assets to "Redrawn".
- [ ] Add the temp fix edits to the main mod assets

## Coding and Configurations
- [ ] Change priority to Early and test with other retexture mods.
- [ ] Adjust some settings listed below with Early priority:
- [ ] "Flowering Bushes", "Terrain Flowers", "Forageable Trees", "Decorative Trees", "Bushes" and "Fruit Trees", combine them into "Vegetation" or at least make them a sub category of "Vegetation". If you disable "Vegetation" (C#) the sub categories are ignored (like with farm buildings)
- [ ] "Snow-covered Bushes" will definitely be removed in favour of a query for "has config:Bushes AND has config:SnOverlay" or "has config:Vegetation AND has config:SnOverlay" 
- [ ] "Iridium Oasis" for main mod instead of just SVE
- [ ] "Shipping Bin" move to buildings:farm config
- [ ] "Big Craftables"
- [ ] Remove "Seasonal Maps"
```
C#
  "Grass Type"
  "Water Type"
  "Holiday Overlays"
  
Main  
  "Artifact Spot" EARLY?
  "Hoed Dirt"
  "Fertilizer"
  "Craftable Paths" just do it
  "Fences"
```
