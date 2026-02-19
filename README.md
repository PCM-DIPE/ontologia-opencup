# Ontologia OpenCUP

**Ontologia OWL del dominio del Codice Unico di Progetto (CUP) per gli investimenti pubblici italiani.**

[![License: CC BY 4.0](https://img.shields.io/badge/License-CC%20BY%204.0-lightgrey.svg)](https://creativecommons.org/licenses/by/4.0/)
[![OWL](https://img.shields.io/badge/OWL-2-blue.svg)](https://www.w3.org/TR/owl2-overview/)

| Proprietà | Valore |
|---|---|
| **Namespace IRI** | `https://w3id.org/italia/onto/OpenCUP/` |
| **Prefisso** | `ocup` |
| **Versione corrente** | 0.6 |
| **Licenza** | [CC BY 4.0](https://creativecommons.org/licenses/by/4.0/) |
| **Autore** | [DIPE – Presidenza del Consiglio dei Ministri](https://www.programmazioneeconomica.gov.it) |

---

## Descrizione

L'ontologia OpenCUP modella il dominio del **Codice Unico di Progetto (CUP)**, il codice alfanumerico di 15 caratteri che identifica in modo univoco ogni progetto di investimento pubblico in Italia.

L'ontologia formalizza:

- **Soggetti e Organizzazioni** – soggetti titolari, concentratori, deleganti e i relativi ruoli nella gestione del CUP
- **CUP** – le diverse tipologie (standard, master, cumulativo, collegato) e i relativi stati del ciclo di vita
- **Progetto di investimento pubblico** – i dati generali, geografici e finanziari del progetto
- **Interventi** – le diverse nature progettuali (lavori pubblici, acquisto di beni, contributi, servizi, incentivi, ricerca, ecc.)
- **Atti** – atti amministrativi, di finanziamento, autorizzazione, chiusura, revoca, delega
- **Classificazioni** – natura, settore, sotto-settore, categoria, area di intervento

L'ontologia è sviluppata come parte del framework nazionale di interoperabilità semantica ed è allineata con la rete di ontologie **OntoPiA** (`https://w3id.org/italia/onto/`).

## Statistiche (v0.6)

| Elemento | Quantità |
|---|---|
| Classi (OpenCUP) | 74 |
| Classi (riferimenti esterni) | 8 |
| Object Properties | 64 |
| Data Properties | 36 |
| Named Individuals | 8 |
| Triple RDF totali | 865 |

## Struttura del repository

```
ontologia-opencup/
├── latest/                     # Versione corrente
│   ├── OpenCUP.owl             # OWL (RDF/XML)
│   ├── OpenCUP.rdf             # RDF/XML
│   ├── OpenCUP.ttl             # Turtle
│   ├── OpenCUP.jsonld          # JSON-LD
│   ├── OpenCUP.nt              # N-Triples
│   └── OpenCUP.graphol         # Sorgente Graphol (Eddy)
├── 0.6/                        # Versione 0.6
│   ├── (stesse serializzazioni)
│   └── OpenCUP_v0_6.graphol    # Sorgente Graphol originale
├── w3id/                       # File per registrazione w3id.org
│   ├── .htaccess
│   └── README.md
├── docs/                       # Documentazione HTML
│   └── index.html
├── CHANGELOG.md
├── LICENSE
└── README.md                   # Questo file
```

## Ontologie esterne referenziate

L'ontologia OpenCUP fa riferimento (import) alle seguenti ontologie della rete OntoPiA:

| Prefisso | Ontologia | Namespace |
|---|---|---|
| `L0` | Top-level Ontology | `https://w3id.org/italia/onto/l0/` |
| `CLV` | Core Location Vocabulary | `https://w3id.org/italia/onto/CLV/` |
| `COV` | Core Organization Vocabulary | `https://w3id.org/italia/onto/COV/` |
| `CPV` | Core Person Vocabulary | `https://w3id.org/italia/onto/CPV/` |
| `TI` | Time Ontology | `https://w3id.org/italia/onto/TI/` |
| `RO` | Role Ontology | `https://w3id.org/italia/onto/RO/` |
| `SM` | Social Media / Online Contact | `https://w3id.org/italia/onto/SM/` |

## URI permanenti (w3id.org)

Le URI dell'ontologia sono registrate tramite il servizio [w3id.org](https://w3id.org/):

```
# Ontologia (con content negotiation)
https://w3id.org/italia/onto/OpenCUP/

# Singola classe o proprietà
https://w3id.org/italia/onto/OpenCUP/Progetto_investimento_pubblico

# Versione specifica
https://w3id.org/italia/onto/OpenCUP/0.6/
```

Content negotiation supportata:

```bash
# Turtle
curl -L -H "Accept: text/turtle" https://w3id.org/italia/onto/OpenCUP/

# RDF/XML
curl -L -H "Accept: application/rdf+xml" https://w3id.org/italia/onto/OpenCUP/

# JSON-LD
curl -L -H "Accept: application/ld+json" https://w3id.org/italia/onto/OpenCUP/

# HTML (documentazione, default browser)
curl -L https://w3id.org/italia/onto/OpenCUP/
```

## Risorse correlate

- **Portale OpenCUP**: [https://opencup.gov.it](https://opencup.gov.it)
- **API OpenCUP**: [https://www.opencup.gov.it/portale/web/opencup/le-api-di-opencup](https://www.opencup.gov.it/portale/web/opencup/le-api-di-opencup)
- **Scheda CUP** (URL breve): `https://opencup.gov.it/portale/progetto/-/cup/{CODICE_CUP}`
- **DIPE**: [https://www.programmazioneeconomica.gov.it](https://www.programmazioneeconomica.gov.it)
- **OntoPiA**: [https://github.com/italia/daf-ontologie-vocabolari-controllati](https://github.com/italia/daf-ontologie-vocabolari-controllati)
- **Schema.gov.it**: [https://schema.gov.it](https://schema.gov.it)

## Strumenti utilizzati

- **[Eddy](https://www.obdasystems.com/eddy)** – editor visuale per ontologie basato su Graphol
- **[rdflib](https://rdflib.readthedocs.io/)** – libreria Python per la serializzazione RDF

## Licenza

Quest'opera è distribuita con Licenza [Creative Commons Attribuzione 4.0 Internazionale](https://creativecommons.org/licenses/by/4.0/).

## Contatti

**Dipartimento per la programmazione e il coordinamento della politica economica (DIPE)**
Presidenza del Consiglio dei Ministri

- Web: [https://www.programmazioneeconomica.gov.it](https://www.programmazioneeconomica.gov.it)
- GitHub: [@PCM-DIPE](https://github.com/PCM-DIPE)
