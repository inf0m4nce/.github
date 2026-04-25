<div align="center">

<img src="https://infomance.com.br/logo.svg" alt="Infomance" width="200" />

# Infomance

**Data infrastructure for companies building in Brazil**

*Infraestrutura de dados para empresas que constroem no Brasil*

[![Website](https://img.shields.io/badge/Website-infomance.com.br-0066FF?style=flat-square)](https://infomance.com.br)
[![API Docs](https://img.shields.io/badge/API%20Docs-docs-00C853?style=flat-square)](https://api.infomance.com.br/docs)
[![Status](https://img.shields.io/badge/Status-Operational-00C853?style=flat-square)](https://status.infomance.com.br)

</div>

---

## What we do / O que fazemos

Infomance provides unified access to Brazilian municipal data through a single, developer-friendly API. We aggregate, normalize, and enrich data from 50+ official sources so you don't have to.

A Infomance fornece acesso unificado a dados municipais brasileiros através de uma única API amigável para desenvolvedores. Agregamos, normalizamos e enriquecemos dados de mais de 50 fontes oficiais para que você não precise.

### Data Coverage / Cobertura de Dados

| Category | Sources | Coverage |
|----------|---------|----------|
| **Economic** | IBGE, BCB, RAIS | 5,570 municipalities |
| **Health** | CNES, DataSUS | 330k+ establishments |
| **Education** | INEP, IDEB | 180k+ schools |
| **Agriculture** | SICOR, MapBiomas, SEEG | All rural credit data |
| **Trade** | COMEX Stat | Export data by municipality |
| **Infrastructure** | SNIS, Anatel | Sanitation & connectivity |
| **Security** | SSP, Atlas da Violência | Crime statistics |

---

## SDKs

Install our official SDKs to get started in minutes:

### TypeScript / JavaScript

```bash
npm install infomance
```

```typescript
import { InfomanceClient } from 'infomance';

const client = new InfomanceClient({ apiKey: 'your-api-key' });
const saopaulo = await client.getMunicipality('3550308');
```

### Python

```bash
pip install infomance
```

```python
from infomance import InfomanceClient

client = InfomanceClient("your-api-key")
sao_paulo = client.get_municipality("3550308")
```

---

## Resources / Recursos

- **[Documentation](https://api.infomance.com.br/docs)** — API reference and guides
- **[Pricing](https://infomance.com.br/pricing)** — Plans starting at R$99/month
- **[Status](https://status.infomance.com.br)** — Real-time system status
- **[Support](mailto:suporte@infomance.com.br)** — We respond within 24h

---

<div align="center">

**Built with precision in Brazil 🇧🇷**

*Construído com precisão no Brasil*

[Website](https://infomance.com.br) · [Twitter](https://twitter.com/infomaboreia) · [LinkedIn](https://linkedin.com/company/infomance)

</div>
