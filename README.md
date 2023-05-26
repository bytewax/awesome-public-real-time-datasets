# Awesome Public Real-Time Datasets and Sources

[![Awesome](https://awesome.re/badge-flat.svg)](https://awesome.re)

This list is inspired by [awesome public datasets](https://github.com/awesomedata/awesome-public-datasets), but for real-time datasets and sources. Normally accessed via HTTP or Websockets.

The list is separated into Free and Paid and broken into subsections based on loose categories.

## Free

### Finance/Crypto
 - [Coinbase Market Data](https://docs.cloud.coinbase.com/exchange/docs/websocket-overview) - Coinbase websocket to market data including level 2 orderbook data.
 - [Blockchain transactions](https://www.blockchain.com/api/api_websocket) - Provides real-time notifications about new transactions and blocks.
 - [Yahoo Finance](https://finance.yahoo.com/quote/%5EGSPC?p=%5EGSPC)`wss://streamer.finance.yahoo.com/` - This is not advertised in developer documentation, but discoverable as the websocket is used to update their website.
 - [Finnhub](https://finnhub.io/docs/api/introduction) - Limited free usage with a premium data sources also available.
 - [CoinCheck](https://coincheck.com/documents/exchange/api#websocket) - a cryptocurrency API that has a WebSocket interface (in beta)
 - [Alpaca Markets](https://alpaca.markets/docs/market-data/) Real-Time and historical market data via HTTP and Websocket.

### Transportation
 - [Open Rail Data](https://wiki.openraildata.com/index.php/Rail_Data_FAQ) - A collection of APIs that provide data relating to the UK rail network, including reference data, train timetables, and live service updates. The live data is streamed using the STOMP protocol.
 - [GBFS New York](http://gbfs.citibikenyc.com/gbfs/gbfs.json) - GBFS is the standard for bike share data with many locations around the world. Find more information [here](https://github.com/MobilityData/gbfs/blob/master/gbfs.md)
 - [Open Sky Flight](https://openskynetwork.github.io/opensky-api/rest.html) - Data from Open Sky Api via HTTP endpoint. Supports real-time, but not streaming. Need to continually poll.
 - [MTA GTFS Feed](https://new.mta.info/developers) - Transit data in [GTFS format](https://developers.google.com/transit/gtfs-realtime/) for transit systems like NYC subway and Caltrain.

### Information
- [Wikimedia SSE](https://wikitech.wikimedia.org/wiki/Event_Platform/EventStreams) Event Stream of recent changes to the wikimedia foundation pages.
- [Seismic Data](https://www.seismicportal.eu/realtime.html) Seismic Portal provides a websocket interface to real-time seismic events.
- [Open Weather API](https://openweathermap.org/api) - Current weather data available free at rate of 1 request per second.
- [Clima Cell](https://docs.tomorrow.io/reference/realtime-weather) - Real-time weather data in a free or paid API.
- [NOAA Buoy Data](https://www.ndbc.noaa.gov/data/realtime2/) - Real-time buoy data from NOAA
- [NOAA Weather Data](https://www.weather.gov/documentation/services-web-api) - Live Weather Data API from NOAA
- [Redfin Realestate](https://github.com/ryansherby/RedfinScraper) - pull uptodate data from redfin unofficial API.
- [EPA Airnow data](https://docs.airnowapi.org/) - Air quality data hosted by the EPA.

### Other
- [GitHub Events](https://github.com/fastai/ghapi) - Use the GitHub API to consume public events happening on GitHub.
- [EventSim](https://github.com/viirya/eventsim) - Tool to simulate event data

## Paid

### Finance/Crypto
 - [IEX Trading](https://iextrading.com/developer/docs/) - IEX was created in response to questionable trading practices that had become widely used across traditional exhcanges! Their API provides streaming Stock market data.
 - [Twitter](https://developer.twitter.com/en/docs/tutorials/stream-tweets-in-real-time) - Twitter provides a streaming interface for research or enterprise. It is unknown what support will be post Twitter purchase in 2022. 

### Transportation
- [AIS Data](https://spire.com/developers/) Maritime, Aviation and weather data available via Spire. 

### Information
- [PurpleAir Air Quality Data](https://community.purpleair.com/t/new-api-dashboard/3981) - Developer API for accessing purple air sensor data.
