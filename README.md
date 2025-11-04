# SentinelAI - AI-Powered Security Dashboard

![SentinelAI](https://picsum.photos/seed/readme/1200/300?data-ai-hint=cyber%20security)

> Advanced, web-based platform designed to enhance network security operations by leveraging the power of generative artificial intelligence.

## About The Project

In the current digital landscape, the volume and complexity of cyber threats are increasing exponentially. Security Operations Centers (SOCs) are on the front line, but analysts are often overwhelmed by a deluge of alerts, leading to "alert fatigue" and the risk of missing critical threats.

**SentinelAI** is a next-generation Intrusion Detection System (IDS) dashboard designed to address this fundamental challenge. It provides a centralized, intuitive interface for monitoring network activity, but its true power lies in its integration of cutting-edge generative AI. By translating raw, cryptic security data into clear, human-readable language, SentinelAI provides context-rich insights and actionable intelligence. This empowers analysts, from junior to senior, to understand and respond to threats with greater speed and confidence.

---

## Key Features

- **Real-Time Monitoring:** A live dashboard showing key security metrics, network traffic, and a feed of the latest threat events.
- **Dynamic Statistics:** Dashboard cards update in real-time to simulate a live data feed.
- **AI-Powered Threat Analysis:** Select any threat to receive an AI-generated explanation, confidence score, and suggested actions.
- **AI Mitigation Strategies:** Request and receive clear, actionable mitigation steps for any identified threat.
- **IP Address Analysis:** An integrated tool to analyze any public IP address for its reputation, geolocation, ISP, and known malicious activity.
- **Website Safety Checker:** A tool to analyze any website URL for a safety score and a summary of potential risks like phishing or malware.
- **Live Network View:** A real-time table of active system connections, including process names, protocols, and addresses.
- **Reporting:** Generate and view security reports for specific date ranges.
- **Customizable Settings:** A dedicated page for users to update their profile and notification preferences.
- **Responsive Design:** A modern, clean interface that works seamlessly on both desktop and mobile devices.
- **Light & Dark Mode:** Switch between themes for your viewing comfort.

---

## Built With

This project is built on a modern, robust, and scalable technology stack.

- **[Next.js](https://nextjs.org/)** - React Framework for full-stack web applications.
- **[React.js](https://reactjs.org/)** - A JavaScript library for building user interfaces.
- **[Genkit (for Firebase)](https://firebase.google.com/docs/genkit)** - An open-source framework to build, deploy, and monitor production-grade AI-powered apps.
- **[Google Gemini](https://ai.google.dev/)** - The generative AI model powering the intelligent features.
- **[Tailwind CSS](https://tailwindcss.com/)** - A utility-first CSS framework for rapid UI development.
- **[ShadCN UI](https://ui.shadcn.com/)** - A collection of re-usable UI components.
- **[TypeScript](https://www.typescriptlang.org/)** - A typed superset of JavaScript that compiles to plain JavaScript.

---

## Getting Started

To get a local copy up and running, follow these simple steps.

### Prerequisites

- Node.js (v18 or later)
- npm or yarn

### Installation & Setup

1.  **Clone the repository:**
    ```sh
    git clone https://github.com/your_username/sentinel-ai.git
    cd sentinel-ai
    ```

2.  **Install NPM packages:**
    ```sh
    npm install
    ```

3.  **Set up environment variables:**
    Create a `.env` file in the root of your project and add your Google AI Studio API key.
    ```env
    GEMINI_API_KEY=YOUR_API_KEY
    ```

4.  **Run the development server:**
    ```sh
    npm run dev
    ```

5.  Open [http://localhost:9002](http://localhost:9002) with your browser to see the result.

---

## Project Structure

The project follows the standard Next.js App Router structure.

-   `src/app/`: Contains all the application's routes and pages.
    -   `src/app/dashboard/`: Contains all pages that are part of the main, authenticated dashboard layout.
    -   `src/app/page.tsx`: The main landing page.
    -   `src/app/layout.tsx`: The root layout for the entire application.
    -   `src/app/actions.ts`: Contains all Next.js Server Actions used to communicate with the backend AI flows.
-   `src/components/`: Home to all shared React components.
    -   `src/components/dashboard/`: Components specific to the dashboard (e.g., charts, tables, sidebar).
    -   `src/components/ui/`: Components from the ShadCN UI library.
-   `src/ai/`: Contains all Genkit-related code.
    -   `src/ai/flows/`: All the individual AI flows for features like IP analysis, threat explanation, etc.
    -   `src/ai/genkit.ts`: The main Genkit configuration file.
-   `src/lib/`: Contains utility functions, static data, and type definitions.
-   `public/`: For static assets like images.
-   `PROJECT_REPORT.md`: The detailed project report document.

---

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.
# SentinelAI
