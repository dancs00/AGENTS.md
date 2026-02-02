# AGENTS.md

# 🤖 AI Agent Architecture: RWA Portfolio Analyst

This project implements an autonomous AI Agent designed to bridge the gap between On-chain data (Smart Contracts) and Off-chain financial analysis (RWA Valuation).

## Agent Specifications
- **Role:** RWA Portfolio & Compliance Agent
- **Objective:** Monitor asset health, ensure MiCA transparency, and detect pricing anomalies.
- **Data Sources:** `asset-metadata.json`, Real-time Gold Spot APIs, MiCA Regulatory Framework.

## Logic Workflow
The agent operates through a **Reasoning & Acting (ReAct)** loop:
1. **Observation:** Monitors the `assetDocumentationURI` for changes in grading or storage location.
2. **Analysis:** Calculates the "Premium over Melt" by comparing the token price with the physical gold value (4.4g per Solidus).
3. **Action:** Triggers "Investor Alerts" or schedules mandatory quarterly audits at the Zurich vault.



## Real-world Impact
By automating the monitoring of physical underlying assets, we reduce operational costs for the issuer and increase trust for institutional investors.

# Versione italiana

Questo progetto implementa un Agente AI autonomo progettato per colmare il divario tra i dati On-chain (Smart Contracts) e l'analisi finanziaria Off-chain (Valutazione degli Asset Reali - RWA).

Specifiche dell'Agente
Ruolo: Agente di Portafoglio RWA e Compliance.

Obiettivo: Monitorare lo stato di salute degli asset, garantire la trasparenza richiesta dal MiCA e rilevare anomalie di prezzo.

Fonti Dati: asset-metadata.json, API in tempo reale del prezzo dell'oro (Gold Spot), Quadro Regolamentare MiCA.

Workflow Logico
L'agente opera attraverso un ciclo di Ragionamento e Azione (ReAct):

Osservazione: Monitora l' assetDocumentationURI per rilevare cambiamenti nel grado di conservazione (grading) o nella posizione di stoccaggio.

Analisi: Calcola il "Premium over Melt" (premio rispetto al valore del metallo) confrontando il prezzo del token con il valore dell'oro fisico (4,4g per Solido).

Azione: Attiva "Alert per gli Investitori" o pianifica gli audit trimestrali obbligatori presso il caveau di Zurigo.

Impatto nel Mondo Reale
Automatizzando il monitoraggio degli asset fisici sottostanti, riduciamo i costi operativi per l'emittente e aumentiamo la fiducia degli investitori istituzionali.
