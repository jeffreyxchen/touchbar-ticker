<h1> Cryptocurrency Touchbar Ticker </h1>

This is a quick tutorial on how to add a crypto-currency ticker to your Macbook Pro's Touchbar. Ticker data is received from the CoinMarketCap API.

<h2> Instructions </h2>

Download BetterTouchTools from here: https://www.boastr.net/downloads/

In BetterTouchTools:
- Click "+ Widget"
- At "Select Touchbar Widget:", scroll through and click "Run Apple Script and Show Return Value"
- Click "Advanced Configuration"
  - Give your widget a name (e.g. "BTC" if the ticker is for Bitcoin)
  - Copy and paste the example script from btc_ticker.txt
  - Click save

After that, you're done! Different coins can be added by editing the url in the script (e.g. replace ...com/v1/ticker/bitcoin/ with ...com/v1/ticker/ethereum/ to go from BTC to ETH).
