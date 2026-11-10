# Kazakhstan Import Export Data MCP

**Kazakhstan Customs Data: Importers, Suppliers & HS Codes.** Kazakhstan import export data for your AI assistant. Search Kazakhstan customs shipment records, find importers and foreign suppliers, and break down trade by HS code, partner country and counterparty company, through the Model Context Protocol.

An AI-native alternative to Kazakhstan trade data from Panjiva, ImportGenius, Volza, Seair, TradeInt and ExportGenius: ask in plain language instead of exporting spreadsheets.

The MCP connection is provided by [The Company Atlas](https://thecompanyatlas.com). This repository does not run a separate server.

## Connect

```
https://thecompanyatlas.com/mcp/trade/kazakhstan
```

Add this URL as a custom MCP connector in Claude, ChatGPT, Cursor, or any MCP-compatible client. Sign in with Google when prompted.

- Transport: Streamable HTTP
- Auth: Google OAuth (sign in once, stays authorized)
- Free accounts get 50 credits per calendar month
- Defaults to Kazakhstan: the server tells your AI to filter on `KZ` unless you ask about another country

## Kazakhstan data coverage

- **Years:** 2024–2026
- **Records:** Import declarations: Kazakh importer, foreign supplier, origin country, HS code, goods description, value, quantity, port and date.
- **Country code:** `KZ` (use `buyerCountry: "KZ"` for imports into Kazakhstan)
- **Common products:** cars (HS 8703), vehicle parts (HS 8708), steel (HS 7208), agricultural machinery (HS 8432)

> Party names are stored as declared, often in Russian (Cyrillic). Search in Cyrillic as well as Latin script.

## Notable traders in the data

Companies that appear most often in recent Kazakhstan records (by number of declaration lines, not value):

**Importers**

- SaryarkaAvtoProm
- Coca-Cola Almaty Bottlers
- Kazzinc
- Agromashholding KZ
- Caspian Steel

## Example prompts

- *"Who are the top importers of vehicle parts (HS 8708) into Kazakhstan?"*
- *"What does Kazzinc import, and from which countries?"*
- *"List Kazakh importers of agricultural machinery (HS 8432) in 2025"*
- *"Which Chinese suppliers ship to SaryarkaAvtoProm?"*
- *"Show recent import shipments for Coca-Cola Almaty Bottlers"*

## Tools

### Trade search

| Tool | Description |
|---|---|
| `Trade_search_trades` | Paginated customs shipment search: filter by HS code, buyer, seller, country, port, value and date range |
| `Trade_company_trade_volume_by_year` | Rank importers or exporters by declared value and line counts per year, with HS code and country filters |

### Trade analytics

| Tool | Description |
|---|---|
| `Trade_hs_code_breakdown` | For one company, import and export value by HS chapter, heading or subheading |
| `Trade_year_country_breakdown` | For one company, trade value by year and counterparty country |
| `Trade_partner_breakdown` | For one company, trade value by year and matched counterparty company |

### Company registry

| Tool | Description |
|---|---|
| `Company_search` | Search the global company registry by name or id, with optional country filter |
| `Company_get_by_id` | Full company profile by id |

## Keywords

Kazakhstan import data, Kazakhstan export data, Kazakhstan customs data, Kazakhstan shipment data, importers in Kazakhstan, Kazakhstan buyers and suppliers, HS code search, таможенные данные Казахстана, импорт Казахстана, импортеры, ТН ВЭД
