# Sistema di Gestione Magazzino e Ordini

Sistema completo di gestione magazzino e ordini sviluppato in Python per piccole e medie imprese.

## Caratteristiche

- **Gestione Ordini**: Registrazione, monitoraggio ed evasione con aggiornamento automatico giacenze
- **Inventario Intelligente**: Alert automatici per prodotti sotto soglia di riordino
- **Import/Export**: Supporto CSV e JSON per integrazione con altri sistemi
- **Report Automatici**: Generazione report giornalieri esportabili
- **Sistema di Logging**: Tracciabilità completa di tutte le operazioni
- **CLI Intuitiva**: Interfaccia a riga di comando user-friendly

## Requisiti

- Python 3.7+
- Librerie standard Python (nessuna dipendenza esterna)

## Installazione
```bash
git clone https://github.com/nbaronio/warehouse-management-system.git
cd warehouse-management-system
python src/main.py
```

## Utilizzo

Il sistema inizializza automaticamente con:
- 4 clienti di esempio
- 7 prodotti in magazzino
- Sistema di logging attivo

### Menu Principale
```
1. Registrazione nuovi ordini (manuale o CSV)
2. Visualizza o evadi ordini
3. Consultazione magazzino
4. Generazione report
5. Import/Export JSON
0. Esci
```

### Esempio Import Ordini da CSV

Formato file CSV:
```csv
ORD001,ROSSI,2024-06-01,"{'P001': 10, 'P002': 5}"
```

## Architettura

Sistema costruito con 6 classi principali:
- `Prodotto`: Gestione articoli e giacenze
- `Cliente`: Anagrafica con storico ordini
- `Ordine`: Gestione ordine con stati (NUOVO/EVASO/PARZIALE/IN ATTESA)
- `Magazzino`: Inventario completo
- `GestoreOrdini`: Coordinamento ordini/clienti
- `Report`: Generazione report

## Licenza

MIT License - Vedi file LICENSE

## Autore

Baronio - Progetto sviluppato per l'esame di Programmazione con Python
