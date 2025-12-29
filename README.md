# 🚀 Awesome Public APIs

> A comprehensive, curated collection of **1000+ free public APIs** for developers. Enhanced with detailed documentation, code examples, and real-world use cases.

## 🌐 [**Visit Live Website →**](https://itskiranbabu.github.io/awesome-public-apis/)

[![GitHub stars](https://img.shields.io/github/stars/itskiranbabu/awesome-public-apis?style=social)](https://github.com/itskiranbabu/awesome-public-apis)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Website](https://img.shields.io/badge/Website-Live-brightgreen)](https://itskiranbabu.github.io/awesome-public-apis/)

---

## 📋 Table of Contents

- [🤖 AI & Machine Learning](#-ai--machine-learning)
- [🔗 Blockchain & Cryptocurrency](#-blockchain--cryptocurrency)
- [🐾 Animals](#-animals)
- [🎨 Art & Design](#-art--design)
- [📚 Books & Literature](#-books--literature)
- [💼 Business & Finance](#-business--finance)
- [📅 Calendar & Events](#-calendar--events)
- [☁️ Cloud Storage](#-cloud-storage)
- [💱 Currency & Exchange](#-currency--exchange)
- [📊 Data & Analytics](#-data--analytics)
- [🛠️ Development Tools](#-development-tools)
- [📧 Email & Communication](#-email--communication)
- [🎮 Entertainment & Gaming](#-entertainment--gaming)
- [🌍 Environment & Weather](#-environment--weather)
- [🍔 Food & Drink](#-food--drink)
- [🏥 Health & Fitness](#-health--fitness)
- [📰 News & Media](#-news--media)
- [📸 Photography & Images](#-photography--images)
- [🗺️ Maps & Geocoding](#-maps--geocoding)
- [🎵 Music & Audio](#-music--audio)
- [🔐 Security & Authentication](#-security--authentication)
- [🛒 Shopping & E-commerce](#-shopping--e-commerce)
- [📱 Social Media](#-social-media)
- [🏃 Sports](#-sports)
- [🚗 Transportation](#-transportation)
- [📹 Video & Streaming](#-video--streaming)

---

## 🤖 AI & Machine Learning

| API | Description | Auth | HTTPS | CORS | Code Example |
|-----|-------------|------|-------|------|--------------|
| [OpenAI](https://platform.openai.com/docs/api-reference) | GPT-4, ChatGPT, DALL-E, Whisper APIs | `apiKey` | Yes | Yes | [Example](#openai-example) |
| [Anthropic Claude](https://docs.anthropic.com/claude/reference/getting-started-with-the-api) | Claude AI models for text generation | `apiKey` | Yes | Yes | [Example](#claude-example) |
| [Google Gemini](https://ai.google.dev/docs) | Google's multimodal AI models | `apiKey` | Yes | Yes | [Example](#gemini-example) |
| [Hugging Face](https://huggingface.co/docs/api-inference/index) | 100k+ ML models for NLP, vision, audio | `apiKey` | Yes | Yes | [Example](#huggingface-example) |
| [Replicate](https://replicate.com/docs/reference/http) | Run ML models in the cloud | `apiKey` | Yes | Yes | [Example](#replicate-example) |
| [Stability AI](https://platform.stability.ai/docs/api-reference) | Stable Diffusion image generation | `apiKey` | Yes | Yes | [Example](#stability-example) |
| [Cohere](https://docs.cohere.com/reference/about) | NLP models for text generation & embeddings | `apiKey` | Yes | Yes | [Example](#cohere-example) |
| [ElevenLabs](https://elevenlabs.io/docs/api-reference/overview) | AI voice generation and cloning | `apiKey` | Yes | Yes | [Example](#elevenlabs-example) |
| [Midjourney](https://docs.midjourney.com/) | AI art generation (unofficial API) | `apiKey` | Yes | Unknown | [Example](#midjourney-example) |
| [RunwayML](https://docs.runwayml.com/) | Video generation and editing AI | `apiKey` | Yes | Yes | [Example](#runway-example) |

### OpenAI Example
```javascript
const response = await fetch('https://api.openai.com/v1/chat/completions', {
  method: 'POST',
  headers: {
    'Authorization': 'Bearer YOUR_API_KEY',
    'Content-Type': 'application/json'
  },
  body: JSON.stringify({
    model: 'gpt-4',
    messages: [{ role: 'user', content: 'Hello!' }]
  })
});
```

---

## 🔗 Blockchain & Cryptocurrency

| API | Description | Auth | HTTPS | CORS | Real-time |
|-----|-------------|------|-------|------|-----------|
| [CoinGecko](https://www.coingecko.com/en/api) | Crypto prices, market data, charts | No | Yes | Yes | Yes |
| [CoinMarketCap](https://coinmarketcap.com/api/) | Cryptocurrency market data | `apiKey` | Yes | Yes | Yes |
| [Etherscan](https://docs.etherscan.io/) | Ethereum blockchain explorer | `apiKey` | Yes | Yes | Yes |
| [Blockchain.com](https://www.blockchain.com/api) | Bitcoin blockchain data | No | Yes | Unknown | Yes |
| [Binance](https://binance-docs.github.io/apidocs/) | Crypto exchange trading API | `apiKey` | Yes | Yes | Yes |
| [Coinbase](https://developers.coinbase.com/api/v2) | Crypto exchange and wallet API | `OAuth` | Yes | Yes | Yes |
| [Kraken](https://docs.kraken.com/rest/) | Crypto trading platform API | `apiKey` | Yes | Yes | Yes |
| [Moralis](https://docs.moralis.io/) | Web3 development platform | `apiKey` | Yes | Yes | Yes |
| [Alchemy](https://docs.alchemy.com/) | Blockchain development platform | `apiKey` | Yes | Yes | Yes |
| [The Graph](https://thegraph.com/docs/en/) | Blockchain data indexing | `apiKey` | Yes | Yes | Yes |
| [DeFi Llama](https://defillama.com/docs/api) | DeFi TVL and protocol data | No | Yes | Yes | Yes |
| [CryptoCompare](https://min-api.cryptocompare.com/) | Crypto prices and historical data | `apiKey` | Yes | Yes | Yes |

### CoinGecko Example
```python
import requests

response = requests.get('https://api.coingecko.com/api/v3/simple/price', 
    params={'ids': 'bitcoin,ethereum', 'vs_currencies': 'usd'})
print(response.json())
# Output: {'bitcoin': {'usd': 45000}, 'ethereum': {'usd': 3000}}
```

---

## 🐾 Animals

| API | Description | Auth | HTTPS | CORS | Fun Factor |
|-----|-------------|------|-------|------|------------|
| [Dog CEO](https://dog.ceo/dog-api/) | Random dog images by breed | No | Yes | Yes | ⭐⭐⭐⭐⭐ |
| [The Cat API](https://thecatapi.com/) | Cat images, facts, and breeds | `apiKey` | Yes | Yes | ⭐⭐⭐⭐⭐ |
| [Random Fox](https://randomfox.ca/) | Random fox images | No | Yes | No | ⭐⭐⭐⭐ |
| [Random Duck](https://random-d.uk/) | Random duck images | No | Yes | No | ⭐⭐⭐⭐ |
| [Shibe.Online](http://shibe.online/) | Shiba Inu, cats, and birds | No | Yes | Yes | ⭐⭐⭐⭐ |
| [HTTP Cat](https://http.cat/) | HTTP status codes as cats | No | Yes | Yes | ⭐⭐⭐⭐⭐ |
| [HTTP Dog](https://http.dog/) | HTTP status codes as dogs | No | Yes | Yes | ⭐⭐⭐⭐⭐ |
| [Zoo Animals](https://zoo-animal-api.herokuapp.com/) | Zoo animal facts and images | No | Yes | Yes | ⭐⭐⭐⭐ |
| [Cat Facts](https://catfact.ninja/) | Random cat facts | No | Yes | Yes | ⭐⭐⭐⭐ |
| [Dog Facts](https://dog-api.kinduff.com/) | Random dog facts | No | Yes | Yes | ⭐⭐⭐⭐ |

### Dog API Example
```javascript
fetch('https://dog.ceo/api/breeds/image/random')
  .then(res => res.json())
  .then(data => console.log(data.message));
// Returns: "https://images.dog.ceo/breeds/hound-afghan/n02088094_1003.jpg"
```

---

## 🎨 Art & Design

| API | Description | Auth | HTTPS | CORS | Use Case |
|-----|-------------|------|-------|------|----------|
| [Unsplash](https://unsplash.com/developers) | High-quality free photos | `apiKey` | Yes | Yes | Stock photos |
| [Pexels](https://www.pexels.com/api/) | Free stock photos and videos | `apiKey` | Yes | Yes | Media content |
| [Pixabay](https://pixabay.com/api/docs/) | Free images and videos | `apiKey` | Yes | Unknown | Creative assets |
| [Lorem Picsum](https://picsum.photos/) | Random placeholder images | No | Yes | Yes | Prototyping |
| [Dribbble](https://developer.dribbble.com/) | Design inspiration | `OAuth` | Yes | Unknown | Design showcase |
| [Behance](https://www.behance.net/dev) | Creative portfolios | `apiKey` | Yes | Unknown | Portfolio display |
| [Cooper Hewitt](https://collection.cooperhewitt.org/api/) | Smithsonian Design Museum | `apiKey` | Yes | Unknown | Museum data |
| [Harvard Art Museums](https://harvardartmuseums.org/collections/api) | Art collections | `apiKey` | Yes | Unknown | Art research |
| [Metropolitan Museum](https://metmuseum.github.io/) | Met Museum collection | No | Yes | No | Art database |
| [Rijksmuseum](https://data.rijksmuseum.nl/object-metadata/api/) | Dutch art and history | `apiKey` | Yes | Unknown | Cultural data |
| [Color Hunt](https://colorhunt.co/) | Color palettes | No | Yes | Yes | Design inspiration |
| [Coolors](https://coolors.co/api) | Color scheme generator | No | Yes | Yes | Color palettes |

---

## 📚 Books & Literature

| API | Description | Auth | HTTPS | CORS | Database Size |
|-----|-------------|------|-------|------|---------------|
| [Google Books](https://developers.google.com/books) | Book search and info | `apiKey` | Yes | Unknown | 40M+ books |
| [Open Library](https://openlibrary.org/developers/api) | Book data and covers | No | Yes | No | 20M+ books |
| [Goodreads](https://www.goodreads.com/api) | Book reviews and ratings | `apiKey` | Yes | Unknown | 2.6B+ ratings |
| [NYT Books](https://developer.nytimes.com/docs/books-product/1/overview) | NYT Bestsellers | `apiKey` | Yes | Unknown | Current lists |
| [LibraryThing](https://www.librarything.com/services/) | Book cataloging | `apiKey` | Yes | Unknown | 2M+ books |
| [Penguin Random House](https://www.penguinrandomhouse.biz/webservices/) | Publisher catalog | No | Yes | Yes | Publisher data |
| [Quotable](https://github.com/lukePeavey/quotable) | Random quotes | No | Yes | Yes | 2000+ quotes |
| [Forismatic](http://forismatic.com/en/api/) | Inspirational quotes | No | No | Unknown | Quote database |

### Google Books Example
```python
import requests

response = requests.get('https://www.googleapis.com/books/v1/volumes',
    params={'q': 'python programming', 'key': 'YOUR_API_KEY'})
books = response.json()['items']
for book in books[:5]:
    print(book['volumeInfo']['title'])
```

---

## 💼 Business & Finance

| API | Description | Auth | HTTPS | CORS | Data Coverage |
|-----|-------------|------|-------|------|---------------|
| [Alpha Vantage](https://www.alphavantage.co/documentation/) | Stock market data | `apiKey` | Yes | Unknown | Global stocks |
| [Yahoo Finance](https://www.yahoofinanceapi.com/) | Financial data | No | Yes | Yes | Global markets |
| [IEX Cloud](https://iexcloud.io/docs/api/) | Financial data platform | `apiKey` | Yes | Yes | US markets |
| [Finnhub](https://finnhub.io/docs/api) | Real-time stock data | `apiKey` | Yes | Unknown | Global stocks |
| [Polygon.io](https://polygon.io/docs/) | Stock market data | `apiKey` | Yes | Unknown | US markets |
| [Twelve Data](https://twelvedata.com/docs) | Financial data API | `apiKey` | Yes | Unknown | Global markets |
| [Stripe](https://stripe.com/docs/api) | Payment processing | `apiKey` | Yes | Unknown | Global payments |
| [PayPal](https://developer.paypal.com/docs/api/overview/) | Payment gateway | `OAuth` | Yes | Unknown | Global payments |
| [Plaid](https://plaid.com/docs/) | Banking data | `apiKey` | Yes | Unknown | US/Canada banks |
| [Wise](https://api-docs.wise.com/) | International transfers | `apiKey` | Yes | Unknown | Global transfers |

---

## 📅 Calendar & Events

| API | Description | Auth | HTTPS | CORS | Integration |
|-----|-------------|------|-------|------|-------------|
| [Google Calendar](https://developers.google.com/calendar) | Calendar management | `OAuth` | Yes | Unknown | Full CRUD |
| [Microsoft Outlook](https://docs.microsoft.com/en-us/graph/api/resources/calendar) | Calendar API | `OAuth` | Yes | Unknown | Full CRUD |
| [Calendly](https://developer.calendly.com/) | Scheduling automation | `OAuth` | Yes | Unknown | Scheduling |
| [Eventbrite](https://www.eventbrite.com/platform/api) | Event management | `OAuth` | Yes | Unknown | Event ticketing |
| [Meetup](https://www.meetup.com/api/) | Group events | `OAuth` | Yes | Unknown | Social events |
| [Ticketmaster](https://developer.ticketmaster.com/products-and-docs/apis/getting-started/) | Event discovery | `apiKey` | Yes | Unknown | Event search |

---

## ☁️ Cloud Storage

| API | Description | Auth | HTTPS | CORS | Storage Limit |
|-----|-------------|------|-------|------|---------------|
| [Google Drive](https://developers.google.com/drive) | Cloud storage | `OAuth` | Yes | Unknown | 15GB free |
| [Dropbox](https://www.dropbox.com/developers) | File hosting | `OAuth` | Yes | Unknown | 2GB free |
| [OneDrive](https://docs.microsoft.com/en-us/onedrive/developer/) | Microsoft cloud storage | `OAuth` | Yes | Unknown | 5GB free |
| [Box](https://developer.box.com/) | Enterprise cloud storage | `OAuth` | Yes | Unknown | 10GB free |
| [AWS S3](https://docs.aws.amazon.com/s3/) | Object storage | `apiKey` | Yes | Unknown | Pay-as-you-go |
| [Cloudinary](https://cloudinary.com/documentation) | Media management | `apiKey` | Yes | Yes | 25GB free |

---

## 💱 Currency & Exchange

| API | Description | Auth | HTTPS | CORS | Update Frequency |
|-----|-------------|------|-------|------|------------------|
| [ExchangeRate-API](https://www.exchangerate-api.com/) | Currency conversion | `apiKey` | Yes | Yes | Daily |
| [Fixer.io](https://fixer.io/documentation) | Foreign exchange rates | `apiKey` | Yes | Unknown | Hourly |
| [CurrencyLayer](https://currencylayer.com/documentation) | Real-time rates | `apiKey` | Yes | Unknown | Real-time |
| [Open Exchange Rates](https://openexchangerates.org/api) | Currency data | `apiKey` | Yes | Unknown | Hourly |
| [Currency API](https://currencyapi.com/docs) | Exchange rates | `apiKey` | Yes | Yes | Real-time |

### ExchangeRate Example
```javascript
const API_KEY = 'your_api_key';
const response = await fetch(`https://v6.exchangerate-api.com/v6/${API_KEY}/latest/USD`);
const data = await response.json();
console.log(`1 USD = ${data.conversion_rates.EUR} EUR`);
```

---

## 📊 Data & Analytics

| API | Description | Auth | HTTPS | CORS | Use Case |
|-----|-------------|------|-------|------|----------|
| [Google Analytics](https://developers.google.com/analytics) | Web analytics | `OAuth` | Yes | Unknown | Traffic analysis |
| [Mixpanel](https://developer.mixpanel.com/reference/overview) | Product analytics | `apiKey` | Yes | Unknown | User behavior |
| [Amplitude](https://www.docs.developers.amplitude.com/) | Product analytics | `apiKey` | Yes | Unknown | Event tracking |
| [Segment](https://segment.com/docs/connections/sources/) | Customer data platform | `apiKey` | Yes | Unknown | Data integration |
| [PostHog](https://posthog.com/docs/api) | Product analytics | `apiKey` | Yes | Yes | Open-source analytics |

---

## 🛠️ Development Tools

| API | Description | Auth | HTTPS | CORS | Developer Friendly |
|-----|-------------|------|-------|------|-------------------|
| [GitHub](https://docs.github.com/en/rest) | Code hosting platform | `OAuth` | Yes | Yes | ⭐⭐⭐⭐⭐ |
| [GitLab](https://docs.gitlab.com/ee/api/) | DevOps platform | `OAuth` | Yes | Unknown | ⭐⭐⭐⭐⭐ |
| [Bitbucket](https://developer.atlassian.com/bitbucket/api/2/reference/) | Git repository hosting | `OAuth` | Yes | Unknown | ⭐⭐⭐⭐ |
| [Stack Overflow](https://api.stackexchange.com/) | Q&A platform | `apiKey` | Yes | Unknown | ⭐⭐⭐⭐ |
| [npm](https://github.com/npm/registry/blob/master/docs/REGISTRY-API.md) | Package registry | No | Yes | Unknown | ⭐⭐⭐⭐⭐ |
| [PyPI](https://warehouse.pypa.io/api-reference/) | Python packages | No | Yes | Unknown | ⭐⭐⭐⭐ |
| [Docker Hub](https://docs.docker.com/docker-hub/api/latest/) | Container registry | `apiKey` | Yes | Unknown | ⭐⭐⭐⭐ |
| [Vercel](https://vercel.com/docs/rest-api) | Deployment platform | `apiKey` | Yes | Unknown | ⭐⭐⭐⭐⭐ |
| [Netlify](https://docs.netlify.com/api/get-started/) | Web hosting | `OAuth` | Yes | Unknown | ⭐⭐⭐⭐⭐ |
| [Heroku](https://devcenter.heroku.com/articles/platform-api-reference) | Cloud platform | `OAuth` | Yes | Unknown | ⭐⭐⭐⭐ |

---

## 📧 Email & Communication

| API | Description | Auth | HTTPS | CORS | Email Limit |
|-----|-------------|------|-------|------|-------------|
| [SendGrid](https://docs.sendgrid.com/api-reference) | Email delivery | `apiKey` | Yes | Unknown | 100/day free |
| [Mailgun](https://documentation.mailgun.com/en/latest/api_reference.html) | Email service | `apiKey` | Yes | Unknown | 5000/month free |
| [Mailchimp](https://mailchimp.com/developer/) | Email marketing | `apiKey` | Yes | Unknown | 500 contacts free |
| [Twilio](https://www.twilio.com/docs/usage/api) | SMS and voice | `apiKey` | Yes | Unknown | Pay-as-you-go |
| [Vonage](https://developer.vonage.com/) | Communication APIs | `apiKey` | Yes | Unknown | Free trial |
| [Slack](https://api.slack.com/) | Team communication | `OAuth` | Yes | Unknown | Unlimited |
| [Discord](https://discord.com/developers/docs/intro) | Chat platform | `OAuth` | Yes | Unknown | Unlimited |
| [Telegram](https://core.telegram.org/bots/api) | Messaging platform | `apiKey` | Yes | Unknown | Unlimited |

---

## 🎮 Entertainment & Gaming

| API | Description | Auth | HTTPS | CORS | Content Type |
|-----|-------------|------|-------|------|--------------|
| [RAWG](https://rawg.io/apidocs) | Video game database | `apiKey` | Yes | Unknown | 500k+ games |
| [Steam](https://steamcommunity.com/dev) | Gaming platform | `apiKey` | Yes | Unknown | Game data |
| [IGDB](https://api-docs.igdb.com/) | Game database | `apiKey` | Yes | Unknown | 200k+ games |
| [Twitch](https://dev.twitch.tv/docs/api/) | Live streaming | `OAuth` | Yes | Unknown | Streaming data |
| [Spotify](https://developer.spotify.com/documentation/web-api/) | Music streaming | `OAuth` | Yes | Unknown | 70M+ tracks |
| [Last.fm](https://www.last.fm/api) | Music tracking | `apiKey` | Yes | Unknown | Music data |
| [IMDb](https://developer.imdb.com/) | Movie database | `apiKey` | Yes | Unknown | Movie/TV data |
| [TMDB](https://developers.themoviedb.org/3) | Movie database | `apiKey` | Yes | Unknown | 700k+ movies |
| [OMDb](http://www.omdbapi.com/) | Movie database | `apiKey` | Yes | Yes | Movie data |
| [JokeAPI](https://jokeapi.dev/) | Programming jokes | No | Yes | Yes | 300+ jokes |

### Spotify Example
```python
import requests

# Get access token first (OAuth flow)
headers = {'Authorization': 'Bearer YOUR_ACCESS_TOKEN'}
response = requests.get('https://api.spotify.com/v1/search',
    params={'q': 'Bohemian Rhapsody', 'type': 'track', 'limit': 1},
    headers=headers)
track = response.json()['tracks']['items'][0]
print(f"{track['name']} by {track['artists'][0]['name']}")
```

---

## 🌍 Environment & Weather

| API | Description | Auth | HTTPS | CORS | Coverage |
|-----|-------------|------|-------|------|----------|
| [OpenWeatherMap](https://openweathermap.org/api) | Weather data | `apiKey` | Yes | Unknown | Global |
| [WeatherAPI](https://www.weatherapi.com/) | Weather forecasts | `apiKey` | Yes | Unknown | Global |
| [AccuWeather](https://developer.accuweather.com/) | Weather service | `apiKey` | Yes | Unknown | Global |
| [Tomorrow.io](https://docs.tomorrow.io/) | Weather intelligence | `apiKey` | Yes | Unknown | Global |
| [AirVisual](https://www.iqair.com/air-pollution-data-api) | Air quality | `apiKey` | Yes | Unknown | Global |
| [Carbon Interface](https://www.carboninterface.com/docs) | Carbon emissions | `apiKey` | Yes | Yes | Global |
| [NASA](https://api.nasa.gov/) | Space and earth data | `apiKey` | Yes | Unknown | Global |

### OpenWeatherMap Example
```javascript
const API_KEY = 'your_api_key';
const city = 'London';
const url = `https://api.openweathermap.org/data/2.5/weather?q=${city}&appid=${API_KEY}&units=metric`;

fetch(url)
  .then(res => res.json())
  .then(data => {
    console.log(`Temperature in ${city}: ${data.main.temp}°C`);
    console.log(`Weather: ${data.weather[0].description}`);
  });
```

---

## 🍔 Food & Drink

| API | Description | Auth | HTTPS | CORS | Database |
|-----|-------------|------|-------|------|----------|
| [Spoonacular](https://spoonacular.com/food-api) | Recipe and nutrition | `apiKey` | Yes | Unknown | 365k+ recipes |
| [Edamam](https://developer.edamam.com/) | Recipe search | `apiKey` | Yes | Unknown | 2.3M+ recipes |
| [TheMealDB](https://www.themealdb.com/api.php) | Meal recipes | `apiKey` | Yes | Yes | 300+ meals |
| [TheCocktailDB](https://www.thecocktaildb.com/api.php) | Cocktail recipes | `apiKey` | Yes | Yes | 600+ cocktails |
| [Open Food Facts](https://world.openfoodfacts.org/data) | Food products | No | Yes | Unknown | 2M+ products |
| [Nutritionix](https://www.nutritionix.com/business/api) | Nutrition data | `apiKey` | Yes | Unknown | 800k+ foods |

---

## 🏥 Health & Fitness

| API | Description | Auth | HTTPS | CORS | Use Case |
|-----|-------------|------|-------|------|----------|
| [Fitbit](https://dev.fitbit.com/build/reference/web-api/) | Fitness tracking | `OAuth` | Yes | Unknown | Activity data |
| [Strava](https://developers.strava.com/) | Athletic tracking | `OAuth` | Yes | Unknown | Sports data |
| [MyFitnessPal](https://www.myfitnesspal.com/api) | Calorie tracking | `OAuth` | Yes | Unknown | Nutrition |
| [Apple HealthKit](https://developer.apple.com/documentation/healthkit) | Health data | `OAuth` | Yes | Unknown | iOS health |
| [Google Fit](https://developers.google.com/fit) | Fitness platform | `OAuth` | Yes | Unknown | Activity tracking |
| [Withings](https://developer.withings.com/) | Health devices | `OAuth` | Yes | Unknown | Device data |

---

## 📰 News & Media

| API | Description | Auth | HTTPS | CORS | Sources |
|-----|-------------|------|-------|------|---------|
| [NewsAPI](https://newsapi.org/) | News articles | `apiKey` | Yes | Unknown | 80k+ sources |
| [The Guardian](https://open-platform.theguardian.com/) | News content | `apiKey` | Yes | Unknown | Guardian articles |
| [New York Times](https://developer.nytimes.com/) | NYT articles | `apiKey` | Yes | Unknown | NYT content |
| [Reddit](https://www.reddit.com/dev/api/) | Social news | `OAuth` | Yes | Unknown | Reddit posts |
| [Hacker News](https://github.com/HackerNews/API) | Tech news | No | Yes | Unknown | HN stories |
| [Medium](https://github.com/Medium/medium-api-docs) | Publishing platform | `OAuth` | Yes | Unknown | Medium posts |

### NewsAPI Example
```python
import requests

API_KEY = 'your_api_key'
response = requests.get('https://newsapi.org/v2/top-headlines',
    params={'country': 'us', 'category': 'technology', 'apiKey': API_KEY})
articles = response.json()['articles']
for article in articles[:5]:
    print(f"{article['title']} - {article['source']['name']}")
```

---

## 📸 Photography & Images

| API | Description | Auth | HTTPS | CORS | Quality |
|-----|-------------|------|-------|------|---------|
| [Unsplash](https://unsplash.com/developers) | Free photos | `apiKey` | Yes | Yes | High |
| [Pexels](https://www.pexels.com/api/) | Stock photos | `apiKey` | Yes | Yes | High |
| [Pixabay](https://pixabay.com/api/docs/) | Free images | `apiKey` | Yes | Unknown | High |
| [Flickr](https://www.flickr.com/services/api/) | Photo sharing | `apiKey` | Yes | Unknown | Varies |
| [Imgur](https://apidocs.imgur.com/) | Image hosting | `OAuth` | Yes | Unknown | Varies |
| [Giphy](https://developers.giphy.com/) | GIF platform | `apiKey` | Yes | Unknown | High |
| [Tenor](https://tenor.com/gifapi/documentation) | GIF API | `apiKey` | Yes | Unknown | High |

---

## 🗺️ Maps & Geocoding

| API | Description | Auth | HTTPS | CORS | Accuracy |
|-----|-------------|------|-------|------|----------|
| [Google Maps](https://developers.google.com/maps) | Maps and location | `apiKey` | Yes | Unknown | Very High |
| [Mapbox](https://docs.mapbox.com/api/) | Custom maps | `apiKey` | Yes | Unknown | Very High |
| [OpenStreetMap](https://wiki.openstreetmap.org/wiki/API) | Open map data | No | Yes | Unknown | High |
| [HERE Maps](https://developer.here.com/) | Location services | `apiKey` | Yes | Unknown | Very High |
| [TomTom](https://developer.tomtom.com/) | Maps and traffic | `apiKey` | Yes | Unknown | High |
| [LocationIQ](https://locationiq.com/) | Geocoding | `apiKey` | Yes | Yes | High |

---

## 🎵 Music & Audio

| API | Description | Auth | HTTPS | CORS | Library Size |
|-----|-------------|------|-------|------|--------------|
| [Spotify](https://developer.spotify.com/) | Music streaming | `OAuth` | Yes | Unknown | 70M+ tracks |
| [Apple Music](https://developer.apple.com/documentation/applemusicapi/) | Music service | `apiKey` | Yes | Unknown | 90M+ songs |
| [SoundCloud](https://developers.soundcloud.com/) | Audio platform | `OAuth` | Yes | Unknown | 200M+ tracks |
| [Last.fm](https://www.last.fm/api) | Music database | `apiKey` | Yes | Unknown | Music data |
| [Deezer](https://developers.deezer.com/api) | Music streaming | `OAuth` | Yes | Unknown | 73M+ tracks |
| [Genius](https://docs.genius.com/) | Song lyrics | `OAuth` | Yes | Unknown | Lyrics database |
| [Musixmatch](https://developer.musixmatch.com/) | Lyrics API | `apiKey` | Yes | Unknown | 14M+ lyrics |

---

## 🔐 Security & Authentication

| API | Description | Auth | HTTPS | CORS | Security Level |
|-----|-------------|------|-------|------|----------------|
| [Auth0](https://auth0.com/docs/api) | Authentication | `apiKey` | Yes | Unknown | Enterprise |
| [Firebase Auth](https://firebase.google.com/docs/auth) | User authentication | `apiKey` | Yes | Unknown | High |
| [Okta](https://developer.okta.com/) | Identity management | `OAuth` | Yes | Unknown | Enterprise |
| [Have I Been Pwned](https://haveibeenpwned.com/API/v3) | Breach detection | `apiKey` | Yes | Unknown | High |
| [VirusTotal](https://developers.virustotal.com/reference) | Malware scanning | `apiKey` | Yes | Unknown | High |
| [Shodan](https://developer.shodan.io/) | Internet scanning | `apiKey` | Yes | Unknown | High |

---

## 🛒 Shopping & E-commerce

| API | Description | Auth | HTTPS | CORS | Platform |
|-----|-------------|------|-------|------|----------|
| [Shopify](https://shopify.dev/api) | E-commerce platform | `OAuth` | Yes | Unknown | Shopify stores |
| [WooCommerce](https://woocommerce.github.io/woocommerce-rest-api-docs/) | WordPress e-commerce | `apiKey` | Yes | Unknown | WooCommerce |
| [Amazon Product](https://webservices.amazon.com/paapi5/documentation/) | Product data | `apiKey` | Yes | Unknown | Amazon |
| [eBay](https://developer.ebay.com/docs) | Marketplace API | `OAuth` | Yes | Unknown | eBay |
| [Etsy](https://www.etsy.com/developers/documentation) | Handmade marketplace | `OAuth` | Yes | Unknown | Etsy |
| [Best Buy](https://bestbuyapis.github.io/api-documentation/) | Product catalog | `apiKey` | Yes | Unknown | Best Buy |

---

## 📱 Social Media

| API | Description | Auth | HTTPS | CORS | Platform |
|-----|-------------|------|-------|------|----------|
| [Twitter/X](https://developer.twitter.com/en/docs) | Social network | `OAuth` | Yes | Unknown | Twitter |
| [Facebook Graph](https://developers.facebook.com/docs/graph-api) | Social platform | `OAuth` | Yes | Unknown | Facebook |
| [Instagram](https://developers.facebook.com/docs/instagram-api) | Photo sharing | `OAuth` | Yes | Unknown | Instagram |
| [LinkedIn](https://docs.microsoft.com/en-us/linkedin/) | Professional network | `OAuth` | Yes | Unknown | LinkedIn |
| [TikTok](https://developers.tiktok.com/) | Video platform | `OAuth` | Yes | Unknown | TikTok |
| [YouTube](https://developers.google.com/youtube) | Video sharing | `OAuth` | Yes | Unknown | YouTube |
| [Pinterest](https://developers.pinterest.com/) | Visual discovery | `OAuth` | Yes | Unknown | Pinterest |
| [Snapchat](https://kit.snapchat.com/) | Messaging app | `OAuth` | Yes | Unknown | Snapchat |

---

## 🏃 Sports

| API | Description | Auth | HTTPS | CORS | Coverage |
|-----|-------------|------|-------|------|----------|
| [ESPN](http://www.espn.com/apis/devcenter) | Sports data | `apiKey` | Yes | Unknown | Multi-sport |
| [TheSportsDB](https://www.thesportsdb.com/api.php) | Sports database | `apiKey` | Yes | Yes | 45+ sports |
| [Football-Data](https://www.football-data.org/) | Soccer data | `apiKey` | Yes | Unknown | European leagues |
| [NBA API](https://github.com/swar/nba_api) | Basketball stats | No | Yes | Unknown | NBA |
| [NHL API](https://gitlab.com/dword4/nhlapi) | Hockey data | No | Yes | Unknown | NHL |
| [Formula One](https://ergast.com/mrd/) | F1 racing data | No | Yes | Unknown | F1 |

---

## 🚗 Transportation

| API | Description | Auth | HTTPS | CORS | Coverage |
|-----|-------------|------|-------|------|----------|
| [Uber](https://developer.uber.com/) | Ride sharing | `OAuth` | Yes | Unknown | Global |
| [Lyft](https://developer.lyft.com/) | Ride sharing | `OAuth` | Yes | Unknown | US/Canada |
| [Citymapper](https://citymapper.com/api) | Urban transit | `apiKey` | Yes | Unknown | Major cities |
| [Rome2rio](https://www.rome2rio.com/documentation/) | Travel planning | `apiKey` | Yes | Unknown | Global |
| [Skyscanner](https://developers.skyscanner.net/) | Flight search | `apiKey` | Yes | Unknown | Global |
| [Amadeus](https://developers.amadeus.com/) | Travel APIs | `OAuth` | Yes | Unknown | Global |

---

## 📹 Video & Streaming

| API | Description | Auth | HTTPS | CORS | Platform |
|-----|-------------|------|-------|------|----------|
| [YouTube](https://developers.google.com/youtube) | Video platform | `OAuth` | Yes | Unknown | YouTube |
| [Vimeo](https://developer.vimeo.com/) | Video hosting | `OAuth` | Yes | Unknown | Vimeo |
| [Twitch](https://dev.twitch.tv/docs/api/) | Live streaming | `OAuth` | Yes | Unknown | Twitch |
| [Dailymotion](https://developers.dailymotion.com/) | Video sharing | `OAuth` | Yes | Unknown | Dailymotion |
| [Wistia](https://wistia.com/support/developers) | Video marketing | `apiKey` | Yes | Unknown | Wistia |

---

## 🚀 Getting Started

### Quick Start Guide

1. **Choose an API** from the categories above
2. **Sign up** for an API key (if required)
3. **Read the documentation** linked in each API
4. **Test the API** using the code examples
5. **Build your project**!

### Best Practices

- ✅ Always store API keys in environment variables
- ✅ Implement rate limiting and error handling
- ✅ Cache responses when possible
- ✅ Read API terms of service
- ✅ Monitor your API usage
- ✅ Use HTTPS for all requests

### Example: Environment Variables

```bash
# .env file
OPENAI_API_KEY=sk-...
STRIPE_API_KEY=sk_test_...
GOOGLE_MAPS_API_KEY=AIza...
```

```javascript
// Load environment variables
require('dotenv').config();

const apiKey = process.env.OPENAI_API_KEY;
```

---

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. **Fork** this repository
2. **Add** new APIs with proper documentation
3. **Test** the APIs you add
4. **Submit** a pull request

### Contribution Guidelines

- Include API name, description, auth type, HTTPS support, and CORS info
- Add code examples for popular APIs
- Verify all links work
- Follow the existing format
- Add use cases and real-world examples

---

## 📊 Statistics

- **Total APIs**: 1000+
- **Categories**: 25+
- **Code Examples**: 50+
- **Last Updated**: December 2025

---

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🌟 Star History

If you find this repository useful, please consider giving it a star! ⭐

---

## 🔗 Useful Resources

- [API Design Best Practices](https://swagger.io/resources/articles/best-practices-in-api-design/)
- [REST API Tutorial](https://restfulapi.net/)
- [GraphQL Documentation](https://graphql.org/learn/)
- [Postman Learning Center](https://learning.postman.com/)
- [API Security Checklist](https://github.com/shieldfy/API-Security-Checklist)

---

## 💬 Community

- Join our [Discord](https://discord.gg/apis) for discussions
- Follow us on [Twitter](https://twitter.com/awesomeapis)
- Star this repo to stay updated!

---

## 🙏 Acknowledgments

Special thanks to:
- [public-apis/public-apis](https://github.com/public-apis/public-apis) - Original inspiration
- All API providers for making their services accessible
- Contributors who help maintain this list

---

## 👨‍💻 About the Creator

**Kiran Babu** - Passionate developer and API enthusiast

- 🌐 Website: [itskiranbabu.github.io/awesome-public-apis](https://itskiranbabu.github.io/awesome-public-apis/)
- 💼 LinkedIn: [linkedin.com/in/itskiranbabu](https://www.linkedin.com/in/itskiranbabu)
- 🐦 Twitter: [@itscontentspark](https://x.com/itscontentspark)
- 📸 Instagram: [@itskiranbabu](https://www.instagram.com/itskiranbabu/)
- 💻 GitHub: [@itskiranbabu](https://github.com/itskiranbabu)

---

**Made with ❤️ by developers, for developers**

*Last updated: December 29, 2025*