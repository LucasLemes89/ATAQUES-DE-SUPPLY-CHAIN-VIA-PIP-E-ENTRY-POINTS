# ATAQUES-DE-SUPPLY-CHAIN-VIA-PIP-E-ENTRY-POINTS
Palestra ministrada no Evento Python Brasil - 2026

## 📚 Referências

Casos, números e recursos usados na palestra. O cenário de supply chain muda
rápido — confira datas e versões perto da sua apresentação.

### Incidentes e análises técnicas (2026)

- **PyPI — Incident report: LiteLLM/Telnyx supply-chain attacks** (abr/2026): vetor (token exposto via dependência de CI), janelas de exposição, downloads e orientações. <https://blog.pypi.org/posts/2026-04-02-incident-report-litellm-telnyx-supply-chain-attack/>
- **Mente Binária — "Três camadas, uma botnet: análise técnica de infostealer encontrado no pacote LiteLLM"**: dissecação do payload (camadas de ofuscação, botnet, roubo de credenciais). <https://www.mentebinaria.com.br/artigos/an%C3%A1lise-de-malware/tr%C3%AAs-camadas-uma-botnet-an%C3%A1lise-t%C3%A9cnica-de-infostealer-encontrado-no-pacote-litellm-r120/>
- **CISO Advisor — "LiteLLM comprometido em ataque de cadeia de suprimentos"** (25/03/2026): cobertura do incidente em pt-BR. <https://www.cisoadvisor.com.br/119524-2/>
- **FutureSearch — LiteLLM 1.82.8 Supply Chain Attack on PyPI** (mar/2026): ~119 mil downloads na janela de exposição. <https://futuresearch.ai/blog/litellm-pypi-supply-chain-attack/>
- **TabNews — Ataque à cadeia de suprimentos compromete pacote "telnyx" no PyPI**: persistência no Windows, ~742 mil downloads no mês. <https://www.tabnews.com.br/NewsletterOficial/ataque-a-cadeia-de-suprimentos-compromete-pacote-telnyx-no-pypi>

### Worm Shai-Hulud (npm + PyPI, 2026)

- **GitLab — Shai-Hulud copycat campaign targets Python developers**: typosquat + persistência via `.pth` / `sitecustomize`. <https://about.gitlab.com/blog/shai-hulud-copycat-campaign-targets-python-developers/>
- **JFrog — "Shai-Hulud: Here We Go Again"**: 170+ pacotes atingidos em npm/PyPI. <https://research.jfrog.com/post/shai-hulud-here-we-go-again/>
- **Unit 42 (Palo Alto) — "Shai-Hulud" Worm Compromises npm Ecosystem**: análise da campanha e propagação. <https://unit42.paloaltonetworks.com/npm-supply-chain-attack/>

### Panorama e números do PyPI

- **PyPI — 2025 in review**: 2.000+ denúncias de malware (66% resolvidas em ≤4h), Trusted Publishing >20% dos uploads, attestations 17%. <https://blog.pypi.org/posts/2025-12-31-pypi-2025-in-review/>

### Typosquatting

- **Check Point — PyPI Inundated by Malicious Typosquatting Campaign**. <https://blog.checkpoint.com/securing-the-cloud/pypi-inundated-by-malicious-typosquatting-campaign/>
- **Snyk — Security risks with Python package naming: typosquatting and beyond**. <https://snyk.io/articles/security-risks-with-python-package-naming-convention-typosquatting-and/>

### Dependency Confusion

- **Alex Birsan — "Dependency Confusion: How I Hacked Into Apple, Microsoft and Dozens of Other Companies"** (2021): a pesquisa original; 35+ empresas, US$ 130k+ em bounties. <https://medium.com/@alex.birsan/dependency-confusion-4a5d60fec610>

### Bibliotecas brasileiras (contexto do recorte Brasil)

- **brutils** — validação de CPF/CNPJ/CEP/Pix. <https://pypi.org/project/brutils/> · <https://github.com/brazilian-utils/python>
- **validate-docbr**. <https://pypi.org/project/validate-docbr/>
- **pycep-correios**. <https://pypi.org/project/pycep-correios/>

### Defesas e ferramentas

- **pip 26.1 — dependency cooldown (`--uploaded-prior-to`) e suporte a `pylock.toml`**. <https://sichard.ca/blog/2026/04/whats-new-in-pip-26.1/> · <https://www.infoq.com/news/2026/05/pip-261-dependency-cooldowns/>
- **pip — Secure installs** (`--require-hashes`, `--only-binary`). <https://pip.pypa.io/en/stable/topics/secure-installs/>
- **uv — proteção contra supply chain** (`exclude-newer`, `malware-check`, hashes, `--no-build`). <https://pydevtools.com/handbook/how-to/how-to-protect-against-python-supply-chain-attacks-with-uv/>
- **PEP 751 — `pylock.toml`** (formato padrão de lock). <https://peps.python.org/pep-0751/> · <https://pydevtools.com/handbook/explanation/what-is-pep-751/>
- **pip-audit** — auditoria contra OSV / PyPI Advisory. <https://pypi.org/project/pip-audit/>

---

> ⚠️ Todo o código deste repositório é **educacional** e roda **isolado e
> offline**. Os "segredos" exfiltrados nas demos são **iscas fictícias**; não
> publique nenhum destes pacotes no PyPI real nem reutilize o código fora do lab.
