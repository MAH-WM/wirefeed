# MarketWire LLM

Automatisk processering af danske børsmeddelelser med AI-baseret udvinding af forventningstal.

## 📡 RSS Feed

**Feed URL:** https://[dit-username].github.io/marketwire-rss/processed_feed.xml

## 📈 Hvad er MarketWire LLM?

MarketWire LLM overvåger danske børsmeddelelser fra GlobeNewswire og bruger kunstig intelligens til at udtrække selskabernes forventningstal til omsætning, indtjening og overskudsgrader.

### Format
```
SELSKAB: VENTER I REGNSKABSÅR EN/ET MÅLETYPE PÅ TAL ENHED VALUTA
```

### Eksempel
```
NOVO NORDISK: VENTER I 2025 EN OMSÆTNING PÅ 850-900 MIA DKK
GABRIEL HOLDING: VENTER I 2024/25 ET EBIT PÅ 25-35 MIO DKK
```

## 🔄 Opdateringsfrekvens

- **Tjekkes:** Hver 5. minut for nye meddelelser
- **Kilde:** GlobeNewswire Danmark
- **AI Model:** GPT-4 via Azure OpenAI
- **Output:** "N.B" hvis ingen forventninger findes

## 📱 Sådan bruger du feedet

1. **Kopier RSS URL** fra toppen
2. **Tilføj til din RSS læser** (Feedly, Inoreader, Apple News, etc.)
3. **Modtag automatiske opdateringer** når nye forventningstal bliver fundet

## ⚙️ Tekniske detaljer

- Multiple forventninger fra samme artikel bliver splittet til separate RSS items
- Hver forventning får sit eget unike GUID
- Title indeholder forventningen, description indeholder original artikel titel
- Link peger på original GlobeNewswire artikel

---

*Sidste opdatering: Automatisk via GitHub Actions*
