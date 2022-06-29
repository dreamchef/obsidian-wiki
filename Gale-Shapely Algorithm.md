---
id: 3njb5jhvl7090vjojhnxcj0
title: Gale-Shapely Algorithm
desc: ''
updated: 1656452435338
created: 1654530811868
---
#combinatorics  #method

*Input:* preference ordering with an equal number of heterosexual men and women

*Output:* a [[stable matching]]

**Stage 1**
1. Each man proposes to first preference
2. Each woman accepts any proposals from first preference

While not everyone is engaged...

**Stage** 2
1. Each free man proposes to his next preference (to whom he has not yet proposed)
2. Each woman compares her current proposal to her fiance and chooses whichever she most prefers.
