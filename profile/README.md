<div align="center">

# Infomance

**Data infrastructure for companies building in Brazil**

*Infraestrutura de dados para empresas que constroem no Brasil*

[![Website](https://img.shields.io/badge/Website-infomance.com.br-0066FF?style=flat-square)](https://infomance.com.br)
[![API Docs](https://img.shields.io/badge/API%20Docs-Swagger-00C853?style=flat-square)](https://api.infomance.com.br/docs)
[![PyPI](https://img.shields.io/pypi/v/infomance?style=flat-square&label=PyPI)](https://pypi.org/project/infomance/)
[![NPM](https://img.shields.io/npm/v/infomance?style=flat-square&label=NPM)](https://www.npmjs.com/package/infomance)

</div>

---

## What we do / O que fazemos

Infomance provides unified access to Brazilian municipal data through a single, developer-friendly API. We aggregate, normalize, and enrich data from 50+ official sources so you don't have to.

A Infomance fornece acesso unificado a dados municipais brasileiros através de uma única API. Agregamos, normalizamos e enriquecemos dados de mais de 50 fontes oficiais para que você não precise.

### Data Coverage / Cobertura de Dados

| Category | Sources | Coverage |
|----------|---------|----------|
| **Economic** | IBGE, BCB, RAIS | 5,570 municipalities |
| **Health** | CNES, DataSUS | 330k+ establishments |
| **Education** | INEP, IDEB | 180k+ schools |
| **Agriculture** | SICOR, MapBiomas, SEEG | All rural credit |
| **Trade** | COMEX Stat | Exports by municipality |
| **Infrastructure** | SNIS, Anatel | Sanitation & connectivity |
| **Security** | SSP, Atlas da Violência | Crime statistics |

---

## Quick Start / Início Rápido

### TypeScript / JavaScript

```bash
npm install infomance
```

```typescript
import { InfomanceClient } from 'infomance';

const client = new InfomanceClient({ apiKey: process.env.INFOMANCE_API_KEY });

const sp = await client.getMunicipality('3550308');
console.log(`${sp.name}: R$ ${sp.pib.toLocaleString()}`);
```

### Python

```bash
pip install infomance
```

```python
from infomance import InfomanceClient

client = InfomanceClient(api_key=os.environ["INFOMANCE_API_KEY"])

sp = client.get_municipality("3550308")
print(f"{sp['name']}: R$ {sp['pib']:,.2f}")
```

---

## Repositories / Repositórios

| | Repository | Package |
|---|------------|---------|
| 🟦 | [sdk-js](https://github.com/inf0m4nce/sdk-js) | [![npm](https://img.shields.io/npm/v/infomance?style=flat-square)](https://www.npmjs.com/package/infomance) |
| 🐍 | [sdk-python](https://github.com/inf0m4nce/sdk-python) | [![pypi](https://img.shields.io/pypi/v/infomance?style=flat-square)](https://pypi.org/project/infomance/) |

---

## Resources / Recursos

| | |
|---|---|
| 📚 **[Documentation](https://api.infomance.com.br/docs)** | API reference and guides |
| 💰 **[Pricing](https://infomance.com.br/pricing)** | Plans from R$99/month |
| 📧 **[Support](mailto:suporte@infomance.com.br)** | Response within 24h |

---

<div align="center">

**Built with precision in Brazil** 🇧🇷

[infomance.com.br](https://infomance.com.br)

</div>
