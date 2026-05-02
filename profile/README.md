<div align="center">

# Infomance

**European municipal data. One API.**

[![Website](https://img.shields.io/badge/Website-infomance.io-0066FF?style=flat-square)](https://infomance.io)
[![API Docs](https://img.shields.io/badge/API%20Docs-docs.infomance.io-00C853?style=flat-square)](https://docs.infomance.io)
[![PyPI](https://img.shields.io/pypi/v/infomance?style=flat-square&label=PyPI)](https://pypi.org/project/infomance/)
[![NPM](https://img.shields.io/npm/v/infomance?style=flat-square&label=NPM)](https://www.npmjs.com/package/infomance)

</div>

---

## What we do

Infomance normalizes municipal data from 30+ official EU sources into a single REST API. One schema, 34 countries, 98,000 municipalities. So you don't have to integrate SDMX, WFS, DESTATIS, INSEE, and INE separately.

### Data Coverage

| Category | Sources | Coverage |
|----------|---------|----------|
| **Demographic** | GISCO, INSEE, DESTATIS, INE | 98,000 LAUs, 34 countries |
| **Economic** | Eurostat, CBS, INE PT | GDP, income, employment |
| **Territorial** | Kadaster, Catastro, AT | Parcels, zoning (roadmap) |
| **Safety** | Politie NL, BKA DE | Crime by region (roadmap) |
| **Boundaries** | GISCO LAU/NUTS | Full geometry coverage |

---

## Quick Start

### TypeScript / JavaScript

```bash
npm install infomance
```

```typescript
import { InfomanceClient } from 'infomance';

const client = new InfomanceClient({ apiKey: process.env.INFOMANCE_API_KEY });

const berlin = await client.getEULAUById('DE_11000000');
console.log(`${berlin.name}: ${berlin.population.toLocaleString()}`);
// Berlin: 3,755,251
```

### Python

```bash
pip install infomance
```

```python
from infomance import InfomanceClient

client = InfomanceClient(api_key=os.environ["INFOMANCE_API_KEY"])

berlin = client.get_eu_lau("DE_11000000")
print(f"{berlin['name']}: {berlin['population']:,}")
# Berlin: 3,755,251
```

### REST

```bash
curl https://api.infomance.io/api/v1/eu/lau/DE_11000000 \
  -H "X-API-Key: YOUR_API_KEY"
```

---

## Repositories

| Repository | Package |
|------------|---------|
| [sdk-js](https://github.com/inf0m4nce/sdk-js) | [![npm](https://img.shields.io/npm/v/infomance?style=flat-square)](https://www.npmjs.com/package/infomance) |
| [sdk-python](https://github.com/inf0m4nce/sdk-python) | [![pypi](https://img.shields.io/pypi/v/infomance?style=flat-square)](https://pypi.org/project/infomance/) |

---

## Resources

| | |
|---|---|
| 📚 **[Documentation](https://docs.infomance.io)** | API reference and guides |
| 🗺️ **[Coverage](https://infomance.io/en/features/europe)** | 34 countries, 98k municipalities |
| 💰 **[Pricing](https://infomance.io/en/pricing)** | Free tier · Plans from €49/month |
| 📧 **[Contact](mailto:contact@infomance.io)** | Response within 24h |

<div align="center">

**Built for Europe.**

</div>
