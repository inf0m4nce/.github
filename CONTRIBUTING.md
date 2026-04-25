# Contributing to Infomance / Contribuindo para a Infomance

Thank you for your interest in contributing! / Obrigado pelo seu interesse em contribuir!

## How to Contribute / Como Contribuir

### Reporting Bugs / Reportando Bugs

1. Check if the issue already exists
2. Create a new issue with:
   - Clear title
   - Steps to reproduce
   - Expected vs actual behavior
   - SDK version and environment

### Suggesting Features / Sugerindo Funcionalidades

Open an issue with the `enhancement` label describing:
- The problem you're trying to solve
- Your proposed solution
- Any alternatives you've considered

### Pull Requests

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Make your changes
4. Add tests for new functionality
5. Ensure all tests pass
6. Commit with clear messages
7. Push and open a PR

## Development Setup / Configuração de Desenvolvimento

### TypeScript SDK

```bash
git clone https://github.com/inf0m4nce/sdk-js.git
cd sdk-js
npm install
npm test
```

### Python SDK

```bash
git clone https://github.com/inf0m4nce/sdk-python.git
cd sdk-python
pip install -e ".[dev]"
pytest
```

## Code Style / Estilo de Código

- **TypeScript**: ESLint + Prettier (configured in repo)
- **Python**: Ruff (configured in pyproject.toml)

## Questions? / Dúvidas?

- Open a [Discussion](https://github.com/orgs/inf0m4nce/discussions)
- Email: suporte@infomance.com.br
