# Changelog

Tutte le modifiche rilevanti all'ontologia OpenCUP sono documentate in questo file.

Il formato è basato su [Keep a Changelog](https://keepachangelog.com/it/1.1.0/).

## [0.6] - 2025-07-23

### Prima release pubblica

Modello ontologico del dominio CUP sviluppato con Eddy (Graphol v3).

#### Classi principali

- `Progetto_investimento_pubblico` — il progetto associato al CUP
- `CUP` — il Codice Unico di Progetto (standard, master, cumulativo, collegato)
- `Intervento_di_investimento_pubblico` — l'intervento con la relativa natura progettuale
- `Atto` — atti amministrativi, di finanziamento, autorizzazione, chiusura, revoca
- `Soggetto_richiedente_cup` — soggetti titolari, concentratori, deleganti
- `Natura_progettuale` — lavori pubblici, beni, contributi, servizi, formazione, incentivi, ricerca
- `Area_di_intervento`, `Settore`, `Sotto_settore`, `Categoria`
- `Stato_di_cup`, `Stato_di_atto_di_finanziamento` — stati del ciclo di vita

#### Object Properties principali

- `ha_cup`, `ha_intervento`, `ha_natura_progettuale`
- `ha_soggetto_titolare`, `ha_soggetto_concentratore`
- `ha_area_intervento`, `ha_settore`, `ha_sotto_settore`, `ha_categoria`
- `ha_localizzazione_intervento`, `ha_stato_cup`

#### Data Properties principali

- `codice_cup`, `codice_locale_progetto`, `descrizione_progetto`
- `costo_progetto`, `importo_finanziamento`
- `data_generazione_cup`, `anno_decisione`

#### Ontologie OntoPiA referenziate

- L0, CLV, COV, CPV, TI, RO, SM
