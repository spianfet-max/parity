# Parity

What everyday prices say a currency is worth. A Big Mac index extended to seven baskets, with live FX.

**Baskets**: Big Mac, Starbucks tall latte, Spotify Premium, 5 km taxi (services) · iPhone 17, Nintendo Switch 2, IKEA Billy (traded goods).

**Views**
- Valuation ladder, raw or GDP-adjusted, against USD / EUR / GBP / JPY / CNY / CHF
- One currency across all baskets, implied rates with a draggable spot, tradables gap (services vs goods)
- Does it work? Back-test of Big Mac gaps against subsequent 1/3/5-year FX moves (raw, vs own average, vs average to date)
- Minutes of income: tourist's price vs resident's effort
- Deserved or mispriced: valuation vs current-account balance
- Big Mac history since 2000, price vs GDP per person, editable price table

**Data**
- FX: ECB euro reference rates; other currencies from ExchangeRate-API. Refreshed daily into the artifact's database.
- Prices: apple.com, spotify.com, ikea.com, nintendo.com, Starbucks Japan/Taiwan menus; taxi and most latte prices are estimates (tagged in the table).
- Big Mac: The Economist, github.com/TheEconomist/big-mac-data (July 2026).
- Current accounts: World Bank (BN.CAB.XOKA.GD.ZS), latest year.

`index.html` is the self-contained build (data inlined). `app.html` + `data.js` + `snap.js` are the sources; `snap.json` is the feed snapshot.
