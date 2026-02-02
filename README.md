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

## ⚠️ Use Case: Automated Crisis Management

To demonstrate the agent's decision-making capabilities, a "Stress Test" scenario was simulated involving a physical vault breach and a simultaneous market crash (-10% Gold Spot).

### Agent Response: Emergency Report
In response to the physical tampering of the **Gold Solidus (NUMI-99823-XYZ)** in Zurich, the Agent executed the following protocol:

1. **Protocol Execution:** Triggered the `removeFromWhitelist` function on the Smart Contract to freeze all secondary market transfers (Liquidity Lock).
2. **Asset Downgrade:** Issued an immediate "Red Level" alert, reclassifying the asset from *Investment Grade* to *Under Review*.
3. **Recovery Action:** Initiated an insurance claim under the MiCA framework and scheduled an urgent re-appraisal session within 48 hours.

> **Why this matters:** This automation prevents information asymmetry and protects retail investors from trading tokens that lack physical backing, ensuring full transparency and regulatory compliance.


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

# Caso d'Uso: Gestione Automatizzata delle Crisi
Per dimostrare le capacità decisionali dell'agente, è stato simulato uno scenario di "Stress Test" che prevede una violazione fisica del caveau e un contemporaneo crollo del mercato (-10% Oro Spot).

Risposta dell'Agente: Report di Emergenza
In risposta alla manomissione fisica del Solido d'Oro (NUMI-99823-XYZ) a Zurigo, l'Agente ha eseguito il seguente protocollo:

Esecuzione del Protocollo: Attivazione della funzione removeFromWhitelist sullo Smart Contract per congelare tutti i trasferimenti sul mercato secondario (Blocco della Liquidità).

Declassamento dell'Asset: Emissione di un'allerta immediata di "Livello Rosso", riclassificando l'asset da Investment Grade a Under Review (Sotto Revisione).

Azione di Ripristino: Apertura di una richiesta di risarcimento assicurativo sotto il framework MiCA e pianificazione di una sessione di perizia urgente entro 48 ore.

> **Perché è importante:** Questa automazione previene l'asimmetria informativa e protegge gli investitori retail dallo scambio di token privi di garanzia fisica, assicurando piena trasparenza e conformità normativa.
