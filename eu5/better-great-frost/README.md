# Better Great Frost

For EU5 1.4.7. In November 1708, the event fires for each country that owns at least one location in an area with extended winter, regardless of its capital. It applies one year of local food, population growth and army attrition penalties to owned locations in areas with extended winter. The grain output penalty applies to wheat, rice and maize locations in those areas. The extra local land attrition uses the same value as ordinary normal winter. The event has no naval attrition penalty.

Each affected province loses food once, using the harshest winter among its eligible owned locations: 15% severe, 10% normal, 5% mild or 3% if none has an active winter level. A mixed province still shares one food stockpile. The event keeps the vanilla stability choice. Hover over the event option to see how many locations and provinces were affected, along with linked names for the affected locations.

## Local testing

Link this folder into the game's `Documents\Paradox Interactive\Europa Universalis V\mod\` directory and enable it in a playset. Use a save from before November 1708 so that the old country modifier has not already been applied. Mods that override `little_ice_age.16` or the `little_ice_age` situation need a merged definition.

Launch with `-debug_mode` and tick a pre-event Ottoman save into November 1708. Use a Cairo capital with holdings in the Balkans or Anatolia to verify the country receives the event once and the northern holdings get the penalties. Compare with an unaffected Egyptian location. A country with no holdings in areas with extended winter should receive no event. Check grain and non-grain output, province stockpiles, modifier expiration after one year, and `logs\error.log` for parse or scope errors. Verify the counts and linked location names in the event option tooltip, check whether hovering a name highlights its location, and confirm the vanilla country modifier is absent.

The scripts were checked against the installed game files. The dispatch, event override and balance still need an in-game test.
