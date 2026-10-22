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
 - [FilingFirehose](https://filingfirehose.com) - Real-time parsed SEC EDGAR filings via REST. Body-text-classified 8-Ks (catches buried cyber and officer-departure events), activist-tagged Schedule 13D/G, ATM-offering detection in S-3 / 424B5. Free public tier covers last 72h, no API key.
 - [Binance](https://developers.binance.com/docs/binance-spot-api-docs/web-socket-streams) - WebSocket API that delivers real-time cryptocurrency trading data and order book updates
 - [OANDA](https://github.com/oanda/py-api-streaming) - HTTP based FOREX rates stream through the OANDA API.
 - [CoinCap](https://docs.coincap.io) - Provides real-time pricing and market activity for over 1,000 cryptocurrencies
 - [Polygon.io](https://polygon.io/docs/stocks/getting-started) - Provides real‑time stock market and cryptocurrency data from all US exchanges via REST and WebSocket endpoints.
 - [FinancialData.Net](https://financialdata.net/documentation) - Stock market data, financial statements, insider and institutional trading data, sustainability data, earnings releases, and much more.
 - [CoinPaprika](https://api.coinpaprika.com) - Cryptocurrency market data API with real-time prices, OHLCV, and tickers for 12,000+ coins. Free tier, no API key required.
 - [DexPaprika](https://api.dexpaprika.com) - DEX data API with pool data, token prices, OHLCV, trade history, and SSE streaming across 36 chains. Free tier, no signup to start, data delayed up to 15s.
 - [Pyth Network](https://docs.pyth.network/) - Delivers financial market data across every asset class through one API.
 - [Sharpe](https://www.sharpe.ai/docs/free-api) - Real-time crypto market data API covering funding, derivatives, arbitrage, narratives, listings, and news.
 - [Agent Gateway](https://agent-gateway-kappa.vercel.app/prices) - Free REST API for real-time prices of 500+ crypto tokens via Hyperliquid. No API key required. Poll `GET /prices` for live market data.
 - [OpenChainBench](https://openchainbench.com) - Open benchmarks of crypto infrastructure (RPC providers, bridges, oracles, L1 finality, prediction-market data, Hyperliquid builders) refreshed every minute via a JSON feed, with daily Parquet snapshots on [Hugging Face](https://huggingface.co/datasets/OpenChainBench/benchmarks) (CC-BY-4.0) archived on Zenodo. [[DOI]](https://doi.org/10.5281/zenodo.20800311)
 - [0xArchive](https://www.0xarchive.io/) - Real-time Hyperliquid and Lighter market data via REST and WebSocket, with historical data also available. Permanent no-card free tier.
 - [Eulerpool](https://eulerpool.com/developers/streaming) - Streaming stock quotes (trades, NBBO, 1-second bars, L2) over WebSocket `wss://stream.eulerpool.com/v1/subscribe` and SSE, plus a REST API for fundamentals, ETFs, macro, crypto and FX. Free keys receive delayed 1-second aggregates; paid keys get live ticks.
 - [Adanos](https://adanos.org/) - Near-real-time stock and crypto sentiment from Reddit, X, financial news, and Polymarket via REST, with a free API tier.

### Transportation
 - [ADSBiq](https://adsbiq.com/api/other/websocket?utm_source=awesome-realtime-datasets&utm_medium=directory&utm_campaign=developer_ecosystem&utm_content=websocket) - Community-powered real-time aircraft positions over WebSocket. Sends an initial snapshot followed by sequence-numbered deltas, with optional geographic subscriptions; free access requires no API key.
 - [Open Rail Data](https://wiki.openraildata.com/index.php/Rail_Data_FAQ) - A collection of APIs that provide data relating to the UK rail network, including reference data, train timetables, and live service updates. The live data is streamed using the STOMP protocol.
 - [GBFS New York](http://gbfs.citibikenyc.com/gbfs/gbfs.json) - GBFS is the standard for bike share data with many locations around the world. Find more information [here](https://github.com/MobilityData/gbfs/blob/master/gbfs.md)
 - [Open Sky Flight](https://openskynetwork.github.io/opensky-api/rest.html) - Data from Open Sky Api via HTTP endpoint. Supports real-time, but not streaming. Need to continually poll.
 - [Open Glider Network](http://wiki.glidernet.org/) - The OGN provides real-time traffic for gliders and other light aircraft. You can use an OGN client like [python-ogn-client](https://github.com/glidernet/python-ogn-client) to connect to OGN servers, parse the APRS messages and push them to a broker like Kafka for streaming processing. 
 - [MTA GTFS Feed](https://new.mta.info/developers) - Transit data in [GTFS format](https://developers.google.com/transit/gtfs-realtime/) for transit systems like NYC subway and Caltrain.
 - [NY 511 live camera data](https://511ny.org/cctv) - This live camera data requires some scraping to use. From this list of cameras you can then source the individual camera id and then request the timestamped image or most recent image by building the url like - `https://511ny.org/map/Cctv/<image-id-goes-here>`
 - [Transport for London (TfL)](https://tfl.gov.uk/info-for-open-data-users/our-open-data) - live data about the tube, buses, and more
 - [Norwegian Coastal Administration](https://www.kystverket.no/en/navigation-and-monitoring/ais/access-to-ais-data/) - AIS data from vessels within the Norwegian economic zone and the protection zones off Svalbard and Jan Mayen. (https://www.kystverket.no/en/sea-transport-and-ports/ais/access-to-ais-data/) 
 - [German Traffic Data](https://mobilithek.info/offers?categories=%5B%22https%3A%2F%2Fw3id.org%2Fmdp%2Fschema%2Fdata_categories%23REALTIME_TRAFFIC_DATA%22%5D) - German real-time traffic information
 - [Swiss Traffic & Public Transport Data](https://opentransportdata.swiss/en/group/api-group) - Various real-time transport data from Switzerland such road traffic, status of EV charging stations, shared mobility services and live arrivals/departures of public transport
 - [Transport for NSW API](https://api.nsw.gov.au/ProductCatalogue?apiCategoryId=2) - Real‑time public transport data (buses, trains, ferries) available for New South Wales, Australia
 - [Ireland National Transport Authority](https://developer.nationaltransport.ie/api-details#api=gtfsr&operation=gtfsr-v2) -  Real-time update stream for services provided by Dublin Bus, Bus Éireann, and Go-Ahead Ireland.
 - [LiveTrafficCam](https://bzsasson.github.io/traffic-camera-sources/api.html) - Live US state DOT traffic camera data as JSON: cameras by state or mountain pass with verified live status from rolling HTTP checks, plus measured per-state camera uptime. No auth.

### Information
- [Wikimedia SSE](https://wikitech.wikimedia.org/wiki/Event_Platform/EventStreams) Event Stream of recent changes to the wikimedia foundation pages.
- [Seismic Data](https://www.seismicportal.eu/realtime.html) Seismic Portal provides a websocket interface to real-time seismic events.
- [Open Weather API](https://openweathermap.org/api) - Current weather data available free at rate of 1 request per ~90 seconds (only first 1000 API calls per day are free).
- [Clima Cell](https://docs.tomorrow.io/reference/realtime-weather) - Real-time weather data in a free or paid API.
- [NOAA Buoy Data](https://www.ndbc.noaa.gov/data/realtime2/) - Real-time buoy data from NOAA
- [NOAA Weather Data](https://www.weather.gov/documentation/services-web-api) - Live Weather Data API from NOAA
- [ENSO Historical Dataset](https://github.com/dayu2333-jinyul/enso-historical-data) - Monthly ENSO data (1950-2026), 126 records with ONI/SOI/subsurface anomalies, CSV+JSON, CC0.
- [ENSO Tracker Dashboard](https://elninoguide.com/dashboard) - Real-time El Niño/La Niña monitoring. ONI, SOI, trade winds, and subsurface temps from NOAA/BOM/ECMWF, updated daily.
- [Redfin Realestate](https://github.com/ryansherby/RedfinScraper) - pull up to date data from redfin unofficial API.
- [EPA Airnow data](https://docs.airnowapi.org/) - Air quality data hosted by the EPA.
- [UK Flood Data](https://environment.data.gov.uk/flood-monitoring/doc/reference) - UK government real-time API for flood data.
- [ZipCheckup](https://zipcheckup.com/api) - Free REST API for ZIP-level environmental safety data across the US: water quality, air quality, PFAS contamination, radon, lead, flood risk, and 11 more verticals. Covers 42,000+ ZIP codes. No API key required. CC BY 4.0.
- [US Energy Grid Data](https://www.gridstatus.io/datasets) - Real-time grid information for the US energy grid
- [DC Hub Grid Prices](https://dchub.cloud/api-docs) - Free, no-key REST endpoint (`https://api.dchub.cloud/api/v1/lmp/prices`) returning live 5-minute real-time LMPs for CAISO, ERCOT, MISO, NYISO, PJM and SPP, with per-hub detail at `/api/v1/iso-lmp/snapshot`. Part of DC Hub, the live data layer for data-center site selection; the same data is available to AI agents over MCP at https://dchub.cloud/mcp.
- [USGS Earthquake Real-time Feed](https://earthquake.usgs.gov/fdsnws/event/1/) - Live seismological data feed to know about earthquakes as they happen
- [News API](https://newsapi.org) - Aggregator that pulls headlines and articles from dozens of news outlets worldwide in near real time via API. It offers a free tier (with rate limits)
- [New York Times Newswire API](https://developer.nytimes.com/docs/timeswire-product/1/overview) - The Times Newswire API provides an up-to-the-minute stream of articles published on NYTimes.com.
- [GDELT 2.0 Event Database](https://blog.gdeltproject.org/gdelt-2-0-our-global-world-in-realtime/) - Collection of all events happening everywhere in the world, with emotional valence estimation, realtime translations.
- [CrustAPI](https://crustapi.com) - Live Google News, web search and Maps results as structured JSON, fetched on every request. Free tier of 3,000 credits per month, no credit card.
- [LottoLens PH PCSO Draw Results](https://lottolensph.com/api/draws/latest) - Free, no-key JSON feed of independently compiled Philippine PCSO draw results, refreshed after scheduled draws are source-verified. Poll over HTTP; records include draw date, draw time, and source URL.

### Health
- [Longevity World Cup](https://longevityworldcup.com/api/data/athletes) - Live public biological-age competition dataset with athlete profiles, biomarker records, proof links, placements, and crowd-age fields. Free JSON over HTTP; no API key required.
- [Urgences Québec](https://sante.handled.tools/api) - Live stretcher occupancy and waiting-room counts for every emergency room in Quebec, refreshed from the ministry feed every 15 minutes. JSON over HTTP with no API key needed, and there's an hourly history endpoint per hospital back to August 2026.
- [AlertX Outbreak Signal Clusters](https://alertx.enclai.net/developers) - Clusters of outbreak-shaped public health signals worldwide, rebuilt hourly, with syndrome and disease triage, confidence scores, and whether an official health authority later confirmed the event. Free JSON over HTTP, no API key required; aggregated to WHO region.

### IoT
- [ThingSpeak IoT Public Channels](https://thingspeak.com/channels/public) - Crowdsourced IoT channels of users publishing various IoT sensor data in real-time. Accessible via REST API or MQTT API.
- [Sensor.Community](https://sensor.community/en/) - 15,000+ air quality sensors worldwide, REST API.

### Cybersecurity
- [Certstream](https://certstream.calidog.io) - Certstream provides a publicly accessible real‐time feed of certificate transparency logs, delivering live updates on SSL/TLS certificate issuance as it occurs.
- [Free CertStream API](https://certstream.dev/free-certstream-api.html) - Free hosted WebSocket stream of newly issued TLS certificates and their domain names from Certificate Transparency logs, at `wss://api.certstream.dev/`. No API key required.
- [URLhaus](https://urlhaus.abuse.ch/api/) - Community-driven repository for real-time malicious URL data, offering actionable threat intelligence to block phishing and malware.
- [CISA Automated Indicator Sharing (AIS)](https://www.cisa.gov/topics/cyber-threats-and-advisories/information-sharing/automated-indicator-sharing-ais) - US government-led service that enables public and private organizations to exchange machine-readable threat indicators in real time.
- [Open Threat Exchange (OTX)](https://otx.alienvault.com/api) - Community-driven threat intelligence platform that streams real-time data on malicious IPs, domains, and URL through the OTX DirectConnect API.
- [Shodan Streaming API](https://developer.shodan.io/api/stream) - Real-time feed of devices/banners discovered on the internet. Free tier available.
- [GreyNoise Community API](https://docs.greynoise.io/reference/community-api) - Free IP intelligence lookups for identifying mass scanners and background noise on the internet.

### Development & Testing
- [Lenses Datagen](https://github.com/lensesio/datagen) - Open-source (Apache 2.0) synthetic streaming data generator by Lenses.io. Publishes to Kafka, Pulsar, or any target system. Ships with rich built-in datasets including sea vessel position reports (AIS), NYC taxi trips, telecom Italia network data, IoT device temperature readings, and more.
- [Mockingbird by Tinybird](https://github.com/tinybirdco/mockingbird) - Open-source mock streaming data generator. Pairs well with EventSim which is already listed.
- [SSE.dev](https://sse.dev/test) - Public SSE test endpoint with configurable intervals. Useful for streaming pipeline testing.
  - `https://sse.dev/test?interval=5000`

### AI/ML
- [AI Detector Arena](https://aidetectarena.com) - Live leaderboard and benchmark dataset for evaluating AI-generated image detectors. Real-time rankings updated as new detectors are evaluated against 2,038 images across 17 AI generators. Data accessible via HTTP API. [[DOI]](https://doi.org/10.5281/zenodo.18620634)

### Sports
- [World Cup 2026 Tour](https://ay-worldcup2026.zeabur.app/developers) - Free HTTP API for current 2026 World Cup match-day fixtures, next-match polling, RSS, and calendar feeds. No API key required.
- [Live Tennis API](https://livetennisapi.com/) - Live match state for ATP, WTA, Challenger and ITF over REST: sets, games, points, who is serving and tiebreak flag, plus fixtures and results. Free tier requires a key but no card (30 requests/minute, 100/day); the WebSocket push feed is a paid tier. Open studies dataset (CC BY 4.0) at https://livetennisapi.com/open-tennis-data

### Other
- [US National Parks Live Status (Park Atlas)](https://theparkatlas.com/) - Live alerts, entrance fees, reservation requirements, webcams, and conditions for all 474 US National Park System units, aggregated nightly from official federal APIs. Bulk CSV snapshots: [park-atlas-data](https://github.com/kirkwood-justin/park-atlas-data). No key required.
- [GitHub Events](https://github.com/fastai/ghapi) - Use the GitHub API to consume public events happening on GitHub.
- [EventSim](https://github.com/viirya/eventsim) - Tool to simulate event data
- [Formula 1 Stats & Telemetry](https://github.com/theOehrly/Fast-F1) - Python package that provides an easy-to-use API into live and historical F1 data.
- [International Space Station Live Data](https://iss-mimic.github.io/Mimic/) - More about the project on GitHub https://github.com/ISS-Mimic/Mimic
- [Live Satellite Positions](https://www.n2yo.com/api/) - N2YO.COM allows tracking of satellites through REST API with the NORAD catalog number assigned by the United States Space Command.
- [Hacker News](https://github.com/HackerNews/API) - Near real-time news feed from Hacker News for tech and startup-related topics.
- [Bluesky](https://docs.bsky.app/docs/advanced-guides/firehose) - Firehose is an authenticated stream of events on the protocol that underlies Bluesky, enabling efficient syncing of user updates via a WebSocket connection.
- [SpaceX API](https://github.com/r-spacex/SpaceX-API) - Open-source REST API for SpaceX launches, rockets, capsules, landing pads.
- [OpenF1](https://openf1.org/) - Free and open-source API for real-time and historical Formula 1 data, including telemetry, lap timings, race control messages,  weather, pit stops, team radio, and standings

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
- [Xquik](https://github.com/Xquik-dev/x-twitter-scraper) - REST and MCP access for X/Twitter search, profiles, followers, monitors, webhooks, and bulk extraction workflows.
- [Bing News Search API](https://www.microsoft.com/en-us/bing/apis/bing-news-search-api) - Bing News Search API returns fresh news results from various sources in near real time
- [Reuters News API](https://reutersagency.com/content-delivery-platforms/api-integrations/) - Low latency news feed from Reuters
- [webz.io](https://webz.io/solutions/media-monitoring) - webz.io provides API with real-time information from thousands of news sites, blogs, and discussion forums.
- [Mediastack](https://mediastack.com) - JSON API delivering worldwide news, headlines and blog articles in real-time 


### Sports
- [Sports Livescores](https://www.thesportsdb.com/docs_pricing) - Developer API of TheSportsDB that gives you access to livescores
- [Sportradar Sports Data](https://sportradar.com/media-tech/data-content/sports-data-api/) - Global live data of 80 sports, 500 sport leagues and 750k events a year (free 30 day trial available)
- [HostDeFi](https://hostdefi.com) — free token-safety scanner grading tokens A+–F from on-chain checks (mint/freeze authority, liquidity, holder concentration) across Solana + 7 EVM chains. Keyless REST API, hosted MCP, x402 endpoints.
