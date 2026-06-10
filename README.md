# CollegeIQ - College Discovery & Predictor Platform

CollegeIQ is a high-performance, feature-rich web application designed to help students discover, compare, and predict their chances of admission into top colleges. Built with a modern tech stack, it features responsive design, instant client-side filtering, detailed college profiles, multi-college comparison matrices, and an intelligent cutoff predictor tool.

## 🚀 Live Demo & Preview
* **Local Development URL:** `http://localhost:3000`

---

## 🎯 Key Features Built

### 1. 🏠 Homepage (`/`)
* **Hero Section:** Engaging headline with targeted Call-to-Actions (CTAs) routing users to key features.
* **Animated Stats Bar:** Dynamic counters showcasing database depth (total colleges, active students, successful predictions).
* **Feature Cards:** Visual entry points for the Search Engine, Comparison Engine, and Predictor Tool.
* **Top Colleges Leaderboard:** A clean, high-level preview table highlighting premium institutions.
* **Bottom CTA Banner:** Direct funnel routing students straight to the Predictor tool.

### 2. 🔍 Advanced College Listing & Search (`/colleges`)
* **Instant Filter Search:  ** Search bar featuring real-time query filtering and a one-click clear button.
* **Sidebar Filter Panel:  ** Multi-dimensional filtering across:
  * Institution Type (Public, Private)
  * Location (State-wise)
  * Fee Range (Interactive range slider)
  * Minimum Rating thresholds
  * Accepted Entrance Exams

* **State Management UI:** Active filter count badges with a "Reset All" utility.
* **Sorting Engine:** Dynamic re-ordering by Rating, NIRF Rank, Placement Packages, and Fee structures (Low to High / High to Low).
* **Mobile-First UX:** Fully responsive slide-in filter drawer for smaller viewports.
* **Optimized Loading:** Skeleton loader cards to mitigate perceived latency during state transitions.
* **Sticky CompareBar:** A persistent footer layout to aggregate selections for the comparison engine.
* **Empty State Handling:** Friendly user prompt with a quick "Clear Filters" action when zero results match.

### 3. 🏫 Deep-Dive College Detail Page (`/college/[id]`)
* **Visual Hero Header:** Dynamic cover image with a sleek gradient overlay, integrated NIRF ranking badges, and college type indicators.
* **Quick Stats Ribbon:** At-a-glance visibility into ratings, annual fees, average packages, and absolute placement percentages.
* **5-Tab Deep Architecture:**
  * **Overview:** Institutional highlights grid, accreditation badges, and facility tags.
  * **Courses & Fees:** Structured data tables breaking down degrees, fees, and eligibility criteria.
  * **Placements:** Graphical/metric cards mapping historical placement data and top corporate recruiters.
  * **Cutoffs:** Historical entry cutoffs color-coded by student category for maximum legibility.
  * **Reviews:** Aggregated authentic student feedback separated into scannable Pros and Cons layout cards.

### 4. ⚖️ Multi-College Comparison Engine (`/compare`)
* **Smart Dropdowns:  ** 3-way asynchronous selection dropdowns that automatically exclude already-selected colleges to prevent redundancy.
* **13-Row Comparison Matrix:  ** Exhaustive data mapping across structural, academic, financial, and placement metrics.
* **Algorithmic Highlighting:** Automatically computes and applies a green checkmark highlight to the "Best Value" winner across numeric rows (Lowest Fees, Highest Packages, Best Ratings, Top NIRF Rankings, and Highest Placement %).
* **Seamless Context Passing:** Automatically hydrates selected colleges directly from the listing page's `CompareBar`.

### 5. 🎯 Admission Predictor Tool (`/predictor`)
* **Intuitive Data Input:** Button-grid system for exam selection, numeric input fields for rank/score tracking, and category selection nodes.
* **One-Click Demos:** 4 quick-fill sample presets allowing users to instantly test system capabilities.
* **UX Feedback:** Animated processing state simulation during calculation.
* **Probability Engine UI:** Color-coded categorization mapping results into High, Medium, and Low admission chances.
* **Granular Results Display:** Output cards display target cutoffs, estimated fees, average packages, and institutional ratings alongside a supportive Prediction Guide Legend.

---

## 🛠️ Tech Stack & Architecture

* **Framework:** React / Next.js (Pages or App Router)
* **Styling:** Tailwind CSS (Fully responsive, layout grids, Custom animations)
* **Icons:** Lucide React / React Icons
* **State Management:** React Context API / Custom Hooks (for Compare Basket and Filters)

---

## ⚙️ Local Development Setup

Follow these steps to spin up the project locally on your machine:

### Prerequisites
Ensure you have **Node.js (v18.0.0 or higher)** and **npm** installed.

### Installation Steps

1. **Extract the Source Code:**
   ```bash
   unzip college-discovery-platform.zip
   ```

2. **Navigate to the Directory:**
   ```bash
   cd college-discovery
   ```

3. **Install Dependencies:**
   ```bash
   npm install
   ```

4. **Launch the Development Server:**
   ```bash
   npm run dev
   ```

5. **Open the Application:**
   Open your browser and navigate to `http://localhost:3000` to see the live app.

---

## 📂 Project Structure Preview
```text
college-discovery/
├── components/          # Reusable UI (FilterPanel, CompareBar, Skeleton, Navbar)
├── pages/ or app/       # Core Routing (/, /colleges, /college/[id], /compare, /predictor)
├── public/              # Static assets (Images, Icons)
├── styles/              # Global styles & Tailwind configuration
├── package.json         # Project metadata and dependencies
└── README.md            # Documentation
```

---

## 📄 License
This project is available under the [MIT License](LICENSE).

