# 🇮🇹 Italy Tax Calculator 2025 (Partita IVA)

A lightweight, single-file HTML/JS calculator designed to estimate net income, taxes, and social security contributions (INPS) for freelancers and sole traders in Italy under the 2025 tax regulations.

![License](https://img.shields.io/badge/license-MIT-blue.svg)
![Year](https://img.shields.io/badge/regulations-2025-green.svg)
![Dependencies](https://img.shields.io/badge/dependencies-none-lightgrey.svg)

## 📋 Overview

The Italian tax system for freelancers (*Partita IVA*) is complex, with varying rules based on business type, revenue, and residency status. This tool simplifies the calculation by handling the logic for both the Flat Tax regime (*Forfettario*) and the Standard regime (*Ordinario*), including specific deductions for new residents and families.

## ✨ Features

### 1. Tax Regimes
*   **Regime Forfettario (Flat Tax):** 
    *   Calculates the 15% standard substitute tax.
    *   **Start-up Support:** Toggle for the reduced **5%** tax rate for new businesses (first 5 years).
    *   **Revenue Limits:** Alerts when approaching or exceeding the €85,000 threshold.
*   **Regime Ordinario (IRPEF):** 
    *   Full progressive IRPEF calculation (23% - 43% brackets).
    *   Regional and Municipal surtax estimation.
    *   Real expense deduction logic.

### 2. Social Security (INPS)
*   **Freelancers:** Calculations for *Gestione Separata* (~26.07%).
*   **Artisans & Traders:** Calculations for *Gestione Artigiani e Commercianti*.
    *   Handles Fixed Minimum Contributions + Variable rates.
    *   **Reduction Toggle:** Option to apply the **35% contribution reduction** available to Forfettario traders.

### 3. Special Exemptions & Allowances
*   **Lavoratori Impatriati ("Brain Drain"):** 
    *   Specific logic for the 2025 "New Resident" tax break (50% taxable base exemption).
    *   Automatically enforces incompatibility with Regime Forfettario.
*   **Family & Dependents:**
    *   **Children:** Estimates the *Assegno Unico* cash benefit (added to net income).
    *   **Spouse:** Calculates dependent spouse tax deductions (Ordinario only).

### 4. User Interface
*   **Zero Dependencies:** Runs entirely in the browser. No Node.js, React, or servers required.
*   **Multi-language:** Instant switching between **English**, **Italian**, and **German**.
*   **Dark Mode:** System-aware automatic theme plus a manual toggle.
*   **Responsive:** Fully optimized for mobile and desktop views.

## 🚀 Quick Start

There is no installation required. This is a standalone client-side application.

1.  **Download** the repository or just the `index.html` file.
2.  **Open** `index.html` in any modern web browser (Chrome, Firefox, Safari, Edge).

Alternatively, you can host it immediately via **GitHub Pages**:
1.  Go to your repository Settings.
2.  Select "Pages".
3.  Choose the `main` branch as the source.

## 🧮 Logic & Regulations (2025)

This calculator is updated based on the standard projections for the 2025 fiscal year:
*   **Forfettario Limit:** €85,000.
*   **Impatriati Relief:** Calculated at the new 50% exemption rate (capped at €600k revenue).
*   **INPS Rates:** Based on current projected rates for Gestione Separata and Artigiani.
*   **Coefficiente di Redditività:** Automatically adjusts based on activity type (Freelance vs. E-commerce/Artisan).

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
