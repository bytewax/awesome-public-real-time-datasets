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
 - [SEC EDGAR](https://www.sec.gov/search-filings/edgar-application-programming-interfaces) - The SEC offers real-time streaming access to regulatory filings (like 10-K, 10-Q, 8-K) as well as real-time XBRL financial data via RESTful APIs and RSS feeds.
 - [Binance](https://developers.binance.com/docs/binance-spot-api-docs/web-socket-streams) - WebSocket API that delivers real-time cryptocurrency trading data and order book updates
 - [OANDA](https://github.com/oanda/py-api-streaming) - HTTP based FOREX rates stream through the OANDA API.
 - [CoinCap](https://docs.coincap.io) - Provides real-time pricing and market activity for over 1,000 cryptocurrencies
 - [Polygon.io](https://polygon.io/docs/stocks/getting-started) - Provides real‑time stock market and cryptocurrency data from all US exchanges via REST and WebSocket endpoints.

### Transportation
 - [Open Rail Data](https://wiki.openraildata.com/index.php/Rail_Data_FAQ) - A collection of APIs that provide data relating to the UK rail network, including reference data, train timetables, and live service updates. The live data is streamed using the STOMP protocol.
 - [GBFS New York](http://gbfs.citibikenyc.com/gbfs/gbfs.json) - GBFS is the standard for bike share data with many locations around the world. Find more information [here](https://github.com/MobilityData/gbfs/blob/master/gbfs.md)
 - [Open Sky Flight](https://openskynetwork.github.io/opensky-api/rest.html) - Data from Open Sky Api via HTTP endpoint. Supports real-time, but not streaming. Need to continually poll.
 - [Open Glider Network](http://wiki.glidernet.org/) - The OGN provides real-time traffic for gliders and other light aircraft. You can use an OGN client like [python-ogn-client](https://github.com/glidernet/python-ogn-client) to connect to OGN servers, parse the APRS messages and push them to a broker like Kafka for streaming processing. 
 - [MTA GTFS Feed](https://new.mta.info/developers) - Transit data in [GTFS format](https://developers.google.com/transit/gtfs-realtime/) for transit systems like NYC subway and Caltrain.
 - [NY 511 live camera data](https://511ny.org/cctv) - This live camera data requires some scraping to use. From this list of cameras you can then source the individual camera id and then request the timestamped image or most recent image by building the url like - `https://511ny.org/map/Cctv/<image-id-goes-here>`
 - [Transport for London (TfL)](https://tfl.gov.uk/info-for/open-data-users/our-open-data) - live data about the tube, buses, and more
 - [Norwegian Coastal Administration](https://www.kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) - AIS data from vessels within the Norwegian economic zone and the protection zones off Svalbard and Jan Mayen.
 - [German Traffic Data](https://mobilithek.info/offers?categories=%5B%22https%3A%2F%2Fw3id.org%2Fmdp%2Fschema%2Fdata_categories%23REALTIME_TRAFFIC_DATA%22%5D) - German real-time traffic information
 - [Swiss Traffic & Public Transport Data](https://opentransportdata.swiss/en/group/api-group) - Various real-time transport data from Switzerland such road traffic, status of EV charging stations, shared mobility services and live arrivals/departures of public transport
 - [Transport for NSW API](https://api.nsw.gov.au/ProductCatalogue?apiCategoryId=2) - Real‑time public transport data (buses, trains, ferries) available for New South Wales, Australia
 - [Ireland National Transport Authority](https://developer.nationaltransport.ie/api-details#api=gtfsr&operation=gtfsr-v2) -  Real-time update stream for services provided by Dublin Bus, Bus Éireann, and Go-Ahead Ireland.

### Information
- [Wikimedia SSE](https://wikitech.wikimedia.org/wiki/Event_Platform/EventStreams) Event Stream of recent changes to the wikimedia foundation pages.
- [Seismic Data](https://www.seismicportal.eu/realtime.html) Seismic Portal provides a websocket interface to real-time seismic events.
- [Open Weather API](https://openweathermap.org/api) - Current weather data available free at rate of 1 request per second.
- [Clima Cell](https://docs.tomorrow.io/reference/realtime-weather) - Real-time weather data in a free or paid API.
- [NOAA Buoy Data](https://www.ndbc.noaa.gov/data/realtime2/) - Real-time buoy data from NOAA
- [NOAA Weather Data](https://www.weather.gov/documentation/services-web-api) - Live Weather Data API from NOAA
- [Redfin Realestate](https://github.com/ryansherby/RedfinScraper) - pull up to date data from redfin unofficial API.
- [EPA Airnow data](https://docs.airnowapi.org/) - Air quality data hosted by the EPA.
- [UK Flood Data](https://environment.data.gov.uk/flood-monitoring/doc/reference) - UK government real-time API for flood data.
- [US Energy Grid Data](https://www.gridstatus.io/datasets) - Real-time grid information for the US energy grid
- [USGS Earthquake Real-time Feed](https://earthquake.usgs.gov/fdsnws/event/1/) - Live seismological data feed to know about earthquakes as they happen
- [News API](https://newsapi.org) - Aggregator that pulls headlines and articles from dozens of news outlets worldwide in near real time via API. It offers a free tier (with rate limits)
- [New York Times Newswire API](https://developer.nytimes.com/docs/timeswire-product/1/overview) - The Times Newswire API provides an up-to-the-minute stream of articles published on NYTimes.com. 

### IoT
- [ThingSpeak IoT Public Channels](https://thingspeak.com/channels/public) - Crowdsourced IoT channels of users publishing various IoT sensor data in real-time. Accessible via REST API or MQTT API.

### Cybersecurity
- [Certstream](https://certstream.calidog.io) - Certstream provides a publicly accessible real‐time feed of certificate transparency logs, delivering live updates on SSL/TLS certificate issuance as it occurs.
- [URLhaus](https://urlhaus.abuse.ch/api/) - Community-driven repository for real-time malicious URL data, offering actionable threat intelligence to block phishing and malware.
- [CISA Automated Indicator Sharing (AIS)](https://www.cisa.gov/topics/cyber-threats-and-advisories/information-sharing/automated-indicator-sharing-ais) - US government-led service that enables public and private organizations to exchange machine-readable threat indicators in real time.
- [Open Threat Exchange (OTX)](https://otx.alienvault.com/api) - Community-driven threat intelligence platform that streams real-time data on malicious IPs, domains, and URL through the OTX DirectConnect API.

### Other
- [GitHub Events](https://github.com/fastai/ghapi) - Use the GitHub API to consume public events happening on GitHub.
- [EventSim](https://github.com/viirya/eventsim) - Tool to simulate event data
- [Formula 1 Stats & Telemetry](https://github.com/theOehrly/Fast-F1) - Python package that provides an easy-to-use API into live and historical F1 data.
- [International Space Station Live Data](https://iss-mimic.github.io/Mimic/) - More about the project on GitHub https://github.com/ISS-Mimic/Mimic
- [Live Satellite Positions](https://www.n2yo.com/api/) - N2YO.COM allows tracking of satellites through REST API with the NORAD catalog number assigned by the United States Space Command.
- [Hacker News](https://github.com/HackerNews/API) - Near real-time news feed from Hacker News for tech and startup-related topics.
- [Bluesky](https://docs.bsky.app/docs/advanced-guides/firehose) - Firehose is an authenticated stream of events on the protocol that underlies Bluesky, enabling efficient syncing of user updates via a WebSocket connection.

## Paid

### Finance/Crypto
 - [Data Bento](https://databento.com/live) - Data Bento provides low-latency market data from many exchanges in several schemas. Access over Raw API, which uses a binary protocol over TCP, and our HTTP API. They also provide client libraries for Rust, Python, and C++.
 - [IEX Trading](https://iextrading.com/developer/docs/) - IEX was created in response to questionable trading practices that had become widely used across traditional exhcanges! Their API provides streaming Stock market data.
 - [NYSE Cloud Streaming](https://www.nyse.com/data-products) - Provides real-time access to high-quality NYSE exchange data feeds, streaming directly in the cloud using Kafka format.
 - [Alpha Vantage Market News & Sentiment](https://www.alphavantage.co/documentation/) - Live market news & sentiment data from selected news outlets covering stocks, cryptocurrencies, forex, and a wide range of topics such as fiscal policy, mergers & acquisitions, IPOs, etc.
 - [Bloomberg](https://developer.bloomberg.com) - The Bloomberg Market Data Feed (B-PIPE) provides consolidated, normalized market data in real time.

### Cybersecurity
- [Kaspersky Threat Data Feeds](https://support.kaspersky.com/datafeeds) - Kaspersky Threat Data Feeds deliver continuously updated, real‐time threat intelligence by aggregating data from diverse sources.
- [Bitdefender Threat Intelligence Feeds](https://www.bitdefender.com/en-us/oem/threat-intelligence-feeds-services) - A comprehensive suite of real-time, curated threat data streams that deliver actionable insights on malicious domains, IP addresses, URLs, file hashes, and vulnerabilities.
- [ANY.RUN Threat Intelligence Feeds](https://any.run/cybersecurity-blog/threat-intelligence-feeds/) – Near real-time feeds generated from interactive malware sandbox sessions, providing deep insights into malware behaviors and associated indicators of compromise (IoCs).
- [Deepinfo Data Feeds](https://docs.deepinfo.com/docs/getting-started) – Real-time updates on domain registrations, subdomain discoveries, and DNS changes accesible via REST-based web services.

### Transportation
- [AIS Data](https://spire.com/developers/) Maritime, Aviation and weather data available via Spire.
- [FlightAware Firehose](https://www.flightaware.com/commercial/firehose/) - Real-time data feed of global aircraft ADS-B positions and flight status.
- [Spire Data Services](https://documentation.spire.com) - Global maritime vessel tracking, combining Satellite automatic identification systems (AIS), Terrestrial AIS, and Dynamic AIS.

### Information
- [PurpleAir Air Quality Data](https://community.purpleair.com/t/new-api-dashboard/3981) - Developer API for accessing purple air sensor data.
- [NewsAPI](https://newsapi.org/docs/get-started) - NewsAPI tracks headlines in 7 categories across over 50 countries, and at over a hundred top publications and blogs, in near real time. Free developer version with 24 delays available.
- [X (Twitter)](https://developer.twitter.com/en/docs/tutorials/stream-tweets-in-real-time) - X provides a streaming interface for research or enterprise. 
- [Bing News Search API](https://www.microsoft.com/en-us/bing/apis/bing-news-search-api) - Bing News Search API returns fresh news results from various sources in near real time
- [Reuters News API](https://reutersagency.com/content-delivery-platforms/api-integrations/) - Low latency news feed from Reuters
- [webz.io](https://webz.io/solutions/media-monitoring) - webz.io provides API with real-time information from thousnads of news sites, blogs, and discussion forums.
- [Mediastack](https://mediastack.com) - JSON API delivering worldwide news, headlines and blog articles in real-time 


### Sports
- [Sports Livescores](https://www.thesportsdb.com/docs_pricing) - Developer API of TheSportsDB that gives you access to livescores
- [Sportradar Sports Data](https://sportradar.com/media-tech/data-content/sports-data-api/) - Global live data of 80 sports, 500 sport leagues and 750k events a year (free 30 day trial available)
