# Sheria Index: Africa Bitcoin & Digital Asset Regulatory Frameworks

A structured, open-source dataset assessing the regulatory environment for Bitcoin and digital assets across Africa. Moving beyond standard corporate compliance trackers, the **Sheria Index** specifically evaluates how state-level legal frameworks impact the financial sovereignty, self-custody rights, and privacy of individuals and civil society organisations (CSOs).

---

## Index Overview

The Sheria Index bridges the gap between complex statutory instruments and operational reality on the ground. By mapping indicators like self-custody laws, peer-to-peer (P2P) trading restrictions, and identity-mapping mandates, the index provides researchers, human rights defenders, and developers with a clear risk assessment metric for local operating environments.

### Civil Society Risk Level Definitions

*   **High Risk:** Explicit prohibitions, active state weaponisation of financial infrastructure, or severe surveillance mandates (e.g., draft border key disclosures or real-time identity mapping of all transactions).
*   **Medium Risk:** Legal or newly regulated environments carrying active surveillance flags (e.g., law enforcement freezing P2P accounts without formal charges, or strict VASP frameworks with heavy monitoring).
*   **Low-Medium Risk:** Emerging or transitional frameworks where individual P2P/non-custodial acquisition remains lower-risk, or where regulations target formal intermediaries rather than end-users.
*   **Low Risk:** Established, clear, and stable regulatory environments with robust rule of law and no documented history of financial repression targeting civic space through digital asset mechanisms.

---

## Dataset Schema

The core repository database is maintained as a lightweight CSV file located at `data/sheria_index.csv`. It contains the following structural metrics:

| Column Header | Data Type | Description |
| :--- | :--- | :--- |
| `incident_id` | Alphanumeric | Unique record identifier (e.g., `SI-001`). |
| `country` | String | Target African nation. |
| `civil_society_risk_level` | String | Evaluated qualitative score (`High`, `Medium`, `Low-Medium`, `Low`). |
| `civil_society_notes` | String | Granular analysis of civic space, surveillance, and enforcement impacts. |
| `self_custody_status` | String | Legal and practical status of holding private keys. |
| `p2p_status` | String | Direct peer-to-peer trading status and active local channels. |
| `legal_status` | String | Overall legal classification of digital assets within the jurisdiction. |
| `kyc_aml_required` | String | Mandatory customer due diligence and data retention obligations. |
| `regulatory_classification` | String | Legal treatment of digital assets (e.g., securities, financial products). |
| `vasp_licensing` | String | Licensing or registration requirements for service providers. |
| `tax_treatment` | String | Capital gains, income, or transaction tax structures applied to digital assets. |
| `key_legislation` | String | Primary gazetted acts, bills, or central bank directives. |
| `enforcement_notes` | String | Documented state actions, court precedents, or operational bottlenecks. |
| `region` | String | Geographic African sub-region. |
| `last_updated` | Date | Year and month of the latest verified record revision (`YYYY-MM`). |
| `sources` | String | Semicolon-separated URLs pointing to primary legislative texts or verified reports. |

---

## Contributing

We welcome updates, corrections, and new country data from local legal scholars, researchers, and human rights advocates across the continent. 

To contribute:
1. **Fork** the repository.
2. Edit or append data rows directly inside `data/sheria_index.csv`. Ensure text fields containing internal commas are properly wrapped in double quotes (`"..."`).
3. Submit a **Pull Request** with clear references to official gazetted text, central bank notices, or landmark judicial precedents.

---

## License

This directory is open-source. The mapping data and documentation are available under the terms of the central [HakiFedha LICENSE](https://github.com/HakiFedha/.github/blob/main/profile/LICENSE).
