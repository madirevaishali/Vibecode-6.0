# 👑 Hyderabadi Paradise
## Next-Generation Smart Dine-In Restaurant Ecosystem & Real-Time Kitchen Display System (KDS)


## Team Name
* Himaanishri01



## 🌐 Hosted Application Links
* **🍽️ Customer Table Display:** [https://restaurant-b0i1cjkwk-himaanishri01-9809s-projects.vercel.app/table/1](https://restaurant-b0i1cjkwk-himaanishri01-9809s-projects.vercel.app/table/1) *(Change the table number in the URL like `/table/2`, `/table/5`, etc., to test individual dining tables!)*
* **👨‍🍳 Kitchen Screen Display (KDS):** [https://restaurant-b0i1cjkwk-himaanishri01-9809s-projects.vercel.app/kitchen](https://restaurant-b0i1cjkwk-himaanishri01-9809s-projects.vercel.app/kitchen) *(Watch live orders stream in, filter by station, and manage ticket preparation workflows.)*



## 🛠️ Tech Stack
* **Frontend Framework:** Next.js (App Router) leveraging React Hooks for high-performance state management and dynamic UI rendering.
* **Styling & UI Design:** Tailwind CSS engineered with dark-mode optimized utility classes for high legibility in low-light restaurant environments.
* **Backend & Real-Time Database:** Supabase PostgreSQL Database utilizing real-time channels and WebSocket communication for instantaneous cross-device event broadcasting.
* **Deployment Infrastructure:** Vercel Global Edge Network ensuring lightning-fast loading speeds, zero-downtime reliability, and high availability worldwide.



##  User Stories Completed
1. **Dynamic Guest Ordering Ecosystem (`/table/[id]`):**
   * As a diner, I can open a table-specific URL (e.g., `/table/1`) to view an interactive menu categorized by starters, biryani, curries, beverages, and desserts without mandatory logins.
   * As a diner, I can append custom text instructions or allergy warnings (e.g., *"Extra spicy, peanut allergy alert"*) directly to items.
   * As a diner, I can track my active order status in real time as it transitions from *Pending* to *Preparing* to *Ready*.
2. **Industrial Kitchen Display System & Control Hub (`/kitchen`):**
   * As a kitchen chef, I can view all incoming live orders instantly on a dedicated dashboard.
   * As a chef, I can automatically route and parse items into station categories (*Main Course, Beverages, Desserts, Appetizers*).
   * As a chef, I can update ticket statuses (`Pending`, `Preparing`, `Ready`, `Completed`) and watch completed items auto-archive via an automated 10-second workflow timer.



## 🤖 AI Usage
* **AI Collaboration:** Leveraged an AI collaborator for architecture planning, component structuring (Next.js App Router dynamic routing), real-time database schema synchronization via Supabase, and rapid debugging during development and styling with Tailwind CSS.



## 💡 Detailed Project Concept & Problem Statement

### The Operational Challenge in Modern Dining
Traditional restaurants routinely struggle with peak-hour rushes due to structural inefficiencies:
1. **The Paper Ticket Bottleneck:** Hand-written orders are prone to illegibility, misplacement, and physical damage in humid or hot kitchen environments, leading to wrong orders and food waste.
2. **The Waitstaff Middleman Delay:** Relying solely on waiters to relay customer requests, modifications, and order updates introduces communication delays and human error.
3. **Customer Blind Spots:** Diners have zero visibility into where their order stands in the preparation pipeline, creating frustration and causing them to constantly flag down busy staff for updates.

### The Hyderabadi Paradise Solution
Our platform digitizes the entire dine-in lifecycle into a unified, lightning-fast digital workflow:
* **For the Diner (`/table/[id]`):** Replaces physical menus with an interactive, categorized digital catalog. Guests can browse rich categories, customize meal preferences, place orders straight from their smartphones or table devices, and track preparation progress live.
* **For the Kitchen Line (`/kitchen`):** Replaces messy paper pads with an industrial-grade Kitchen Display System (KDS) that instantly ingests, categorizes, and routes incoming tickets to appropriate culinary stations with clear visual cues and status pipelines.


## ⚙️ Core System Features & Architecture

1. **📱 Dynamic Guest Ordering Ecosystem (`/table/[id]`):**
   * **URL-Param Table Session Binding:** The Next.js dynamic routing extracts the table identifier directly from the path to bind all cart actions and status trackers to that exact physical table.
   * **Immersive Categorization & Catalog:** Menu items are systematically organized into high-demand sections including Signature Biryanis, Starters & Appetizers, Rich Curries & Breads, Refreshing Beverages, and Desserts.
   * **Live Order Tracking Pipeline:** Customers view real-time state changes from *Pending* to *Preparing* to *Ready*.

2. **🍳 Industrial Kitchen Display System (`/kitchen`):**
   * **Intelligent Station Routing:** The KDS engine automatically assigns items to preparation categories.
   * **Color-Coded Status Pipelines:** High-contrast visual indicators for rapid recognition (`Pending`, `Preparing`, `Ready`, `Completed`).
   * **Auto-Archive Workflow:** Orders marked as *Ready* trigger an automated 10-second timer transitioning them into the *Completed* archive list.
   * **Real-Time Supabase WebSocket Sync:** Powered by database subscriptions and polling fallbacks ensuring zero dropped tickets.
