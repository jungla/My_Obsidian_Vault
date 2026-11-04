---
publish: true
created: <% tp.date.now('YYYY-MM-DD HH:mm') %>
modified: 2026-09-04T09:05:56.386Z
published: <% tp.date.now('YYYY-MM-DD HH:mm') %>
category:
  - work
  - research
date: <% tp.date.now('YYYY-MM-DD HH:mm') %>
people:
country:
  - Tanzania
topic:
  - coral reefs
  - small scale fisheries
  - governance
  - climate change
status:
  - idea
  - incomplete draft
  - full draft
  - final
---

In TUMCA, I have 136 fishing grounds with different names. Unfortunately, the total number of grounds is larger

IF name\_1 = name\_2 AND overlap > 10% -> MERGE
IF name\_1 != name\_2 AND overlap > 50% -> MERGE

IF name\_1 = name\_2 AND overlap <10% -> FLAGGED (this is to be field validated)
IF name\_1 != name\_2 AND overlap < 50% -> KEEP SEPARATE

If ONLY 1 GROUP and 1 GEAR havename\_1 = name\_2 AND overlap <10% => REMOVE # I can do this from the list of flagged layers

SIMPLE (this one works!)

Another approach is to merge all layers with same fishing ground name (regardless of % of overlap). IF the resulting layer is still multiple features, then we flag this. IF NOT, we keep.

I can also calculate the degree of overlap of each layer with the same name and average all the overlaps to get an overall overlap score. This is helpful for validation.

we might not need to merge overlapping layers with different names. Effort on an area would be integrated over multiple layers anyway.

Boma Mahandakini S - Subutuni, Kichakamiba, Mwamboza\
Boma Mahandakini Mid- Moa, Zingibari
Boma Mahandakini N - Ndumbani, Jasini
Tawalani Kizingani N - Mtundani, Mwandusi, Tawalani
Tawalani Kizingani Mid - Kichalikani, Mongavyeru
Tawalani Kizingani S - Kwale, Kizingani
Mchomapunda W - Putini, Chongoleani
Mchomapunda E - Mabokweni, Mpirani, Ndaoya
PAMBWEBO W - Pangani Mashariki, Pangani magharibi
PAMBWEBO E - Msaraza, Bweni, Boza
Ustasaki N - Ushongo, Stahabu
Ustasaki S - Sange, Kipumbwi
Mkwami - Mikocheni, Mkwaja
