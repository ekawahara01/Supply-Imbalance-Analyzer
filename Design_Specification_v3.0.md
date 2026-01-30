# Design Specification: SEO Decision Intelligence Engine (v3.0)

## 1. Product Core: The Triple-Lens Framework
The tool is architected into three distinct modes of operation, allowing users to transition from "cost-saving" to "strategic dominance."

### 🔵 Pattern C: Eco-Check (Low-Cost SEO Utility)
**Objective:** Replace high-cost legacy tools with an API-based decision engine for core SEO viability.

#### Input Parameters (Input)
*   **Keyword(s):** Single or multiple target phrases.
*   **Country/Market:** Target geographic location (e.g., US, UK, JP).
*   **Language:** Targeted search language.
*   **Competitor Domains (Optional):** Specific domains to benchmark against.
*   **SERP Depth:** Selection of Top 10 or Top 20 results for precision tuning.

#### Output Parameters (Output)
*   **Demand & Competition Summary:** Search demand estimates and count of active competitors in the SERP.
*   **Supply Density Score:** A metric reflecting how "crowded" the search space is.
*   **Entry Verdict:** A simple "Enterable" or "Hard" classification to mirror legacy tool decision paths.
*   **Cost Savings Report:** A direct comparison showing the $7,614/yr potential savings over traditional tools.

---

### 🟡 Pattern A: Market-Scan (Market & Product Diagnosis)
**Objective:** Provide high-level "Go/No-Go" business decisions based on supply integrity.

#### Input Parameters (Input)
*   **Product Type:** Choice of SaaS, API, Report, or Raw Data format.
*   **Product Scope:** The depth of information or service provided.
*   **Target Market:** Specific industry and country scope.
*   **Persona:** The intended customer profile or problem solver.

#### Output Parameters (Output)
*   **Competitive Volume:** Number of active competitors categorized by entity type (Corporate vs. Individual).
*   **Supply Health Score:** A 0–100 score measuring diversity, freshness, and structural sustainability.
*   **Structural Maintenance Burden:** An estimate of the ongoing effort required for current incumbents to stay relevant.
*   **Verdict Panel:** A color-coded (🔴/🟡/🟢) status: Underserved, Balanced, or Saturated.

---

### 🔴 Pattern B: Strategy-Hunt (Gap Discovery)
**Objective:** Identify "Zombie Supply" and define the ideal product design to outmaneuver incumbents.

#### Input Parameters (Input)
*   **Persona (Fixed):** The target audience whose problem remains unsolved.
*   **Market (Fixed):** The specific competitive landscape.
*   **Exploration Variables:**
    *   **Delivery Type:** API, CSV, SaaS, or Notebook.
    *   **Data Freshness:** Real-time vs. Batch processing requirements.
    *   **User Type:** Engineering-heavy vs. Business-centric users.

#### Output Parameters (Output)
*   **Zombie Supply Identification:** Specific domains with high SEVGI scores (High maintenance/complexity vs. low search visibility).
*   **Underserved Topics:** Specific sub-niches where supply is failing structurally.
*   **Recommended Product Blueprint:** A strategic proposal for the "ideal format" (e.g., API-first or CSV + Notebook) where competition is zero or weak.
*   **Reasoning Engine:** Qualitative explanation of why current supply is failing and how your specific design wins.

## 2. Infrastructure & Technical Stack
The new infrastructure is designed for low latency, high security, and seamless commercial delivery.

| Layer | Technology | Strategic Reasoning |
| :--- | :--- | :--- |
| **Hosting** | Vercel | Edge-ready infrastructure for global speed and GitHub-integrated CI/CD. |
| **Framework** | Next.js | Enables Server-Side API Key Masking, ensuring your DataForSEO credentials are never exposed to the client. |
| **Auth/Database** | Supabase | Managed PostgreSQL and Auth for tracking user sessions and validating Gumroad licenses. |
| **Payment/Licensing** | Gumroad | Native support for license key generation and API-based verification for one-time purchases. |

## 3. Data Flow & Security Model
1.  **Authentication:** The user enters a Gumroad License Key on the landing page.
2.  **Verification:** The Next.js backend verifies the key via the Gumroad API and creates a secure session in Supabase.
3.  **Encapsulation:** All requests to DataForSEO are handled by Next.js API Routes.
    *   User-side inputs (keywords) are sent to the server.
    *   The server injects the hidden API credentials and fetches data.
4.  **Processing:** The SupplyAnalyzer logic runs on the server, calculating Health Scores and SEVGI metrics.
5.  **Rendering:** Only the finalized "Verdict" and "Diagnostic Data" are sent back to the browser for visualization.

## 4. UI/UX: The Professional Dashboard
The UI will focus on "Actionable Insight" over "Raw Data".

*   **Mode Selector:** A sidebar allowing instant switching between Eco-Check, Market-Scan, and Strategy-Hunt.
*   **Verdict Panel:** A prominent header showing the Supply Status (e.g., 🔴 Underserved) and Health Score.
*   **Visual Diagnostics:**
    *   **Health Gauge:** Circular progress bar for immediate comprehension.
    *   **SEVGI Bar Chart:** Identifying specific "Zombie" competitors ranking in the top 10.
*   **Cost Efficiency Block:** A persistent footer reinforcing the >90% cost reduction achieved by using the tool.

### 🛡️ Trust & Transparency Requirements
*   **Disclaimer:** The tool evaluates structural sustainability, not market size or revenue.
*   **Privacy:** Credentials are encrypted and handled exclusively via server-side environment variables.
