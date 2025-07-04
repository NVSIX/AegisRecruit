# AegisRecruit: The AI-Powered Talent Acquisition System

**AegisRecruit is an intelligent, all-in-one recruitment platform that leverages generative AI to streamline hiring, from deep resume analysis to data-driven cultural fit assessment.**

Built for the modern HR professional, this app transforms the tedious, manual process of screening and evaluating candidates into a fast, insightful, and objective workflow.

---

## 🚀 The Problem

In today's competitive job market, recruiters face immense pressure. They are often inundated with hundreds of resumes for a single position, leading to:

-   **Time-Consuming Manual Work**: Hours are spent reading through resumes, often leading to evaluator fatigue and missed opportunities.
-   **Subjective Bias**: It's challenging to remain completely objective, and unconscious bias can influence decision-making.
-   **Inauthentic Resumes**: The rise of AI-generated content makes it difficult to assess the authenticity of a candidate's experience and accomplishments.
-   **Poor Cultural Fit**: A technically skilled candidate may not thrive if they don't align with the company's culture, leading to higher turnover.

AegisRecruit was built to tackle these challenges head-on.

## ✨ The Solution

AegisRecruit acts as an AI co-pilot for recruiters. By integrating Google's Gemini models through Firebase Genkit, we provide a suite of tools that automate, analyze, and enrich the entire hiring process.

-   **Deep AI Analysis**: Goes beyond keywords to provide objective scores on **Suitability**, **Authenticity**, and **Cultural Fit**.
-   **Centralized Pipeline Management**: A visual Kanban-style board to track every candidate through every stage of the hiring process.
-   **Data-Driven Insights**: An analytics dashboard visualizes hiring trends, source effectiveness, and position performance, helping you make smarter decisions.
-   **Intelligent Automation**: Features like automatic interview scheduling and AI-assisted job requirement generation reduce repetitive manual tasks.

---

## 🛠️ How We Built It (Tech Stack)

This project was developed rapidly using a modern, robust, and scalable tech stack.

-   **Framework**: **Next.js 15** (App Router)
-   **Language**: **TypeScript**
-   **Generative AI**: **Firebase Genkit** with **Google's Gemini 1.5 Flash** model.
-   **UI Components**: **ShadCN UI**
-   **Styling**: **Tailwind CSS**
-   **State Management**: **React Context API** for clean, centralized state logic.
-   **Charts & Visualization**: **Recharts**
-   **Development Environment**: Prototyped and built entirely within **Firebase Studio**.

---

## 🌟 Key Features

### 1. **Analytics Dashboard**
A comprehensive overview of your recruitment efforts with real-time charts for:
-   **Hiring Trends**: Track applications, hires, and rejections over time.
-   **Source of Hire**: See which channels are bringing in the most candidates.
-   **Position Performance**: Identify which roles are attracting the most applicants.

### 2. **Visual Hiring Pipeline**
Manage all your job openings from a central hub. Each position has its own Kanban-style pipeline, allowing you to:
-   Visually track candidates from "New Applicant" to "Hired".
-   Drag-and-drop candidates between stages.
-   Get a quick overview of every candidate in the pipeline.

### 3. **The "Brutally Honest" AI Candidate Profile**
This is the core of AegisRecruit. For each candidate, the AI generates a detailed profile, including:
-   **Suitability Analysis**: A radar chart breaking down the candidate's match based on Skills, Experience, Education, and Alignment with the job description.
-   **Authenticity Report**: A "Human-Likeness" score to detect potential AI generation or exaggeration, along with key red flags to investigate.
-   **Cultural Fit Assessment**: The AI analyzes the candidate's resume against your organization's unique values (which you can define in settings) to provide a cultural fit score and analysis.
-   **Objective Narrative**: A clear, unbiased summary of the candidate's strengths, potential weaknesses, and the benefits they could bring to the company.

### 4. **Proactive Background Analysis**
To ensure a smooth user experience and avoid API rate-limiting, the app intelligently pre-fetches and analyzes candidate profiles in the background as soon as they hit the "Screening" stage.

### 5. **Historical Hiring Suggestions**
The AI learns from your decisions! When evaluating a new candidate, it compares their profile to the historical data of previously hired and rejected candidates for that role, providing a predictive hiring suggestion.

### 6. **Smart Interview Scheduling**
When a candidate is moved to the "Interview" stage, the system automatically finds the next available interview slot, ensuring a professional buffer of at least 6 working days.

### 7. **Customizable for Any Organization**
-   **Company Details**: Add your company's mission, vision, and values in the settings to tailor the AI's cultural fit analysis.
-   **Hilti Mode**: A special theme for our hackathon partner, Hilti, demonstrating the app's adaptability. When a user logs in with a `@hilti.com` email, the app's theme and default company details automatically switch.

---

## 🏃‍♀️ How to Run the Project

This project was built to run seamlessly within the Firebase Studio environment.

1.  **Install Dependencies**:
    ```bash
    npm install
    ```

2.  **Set Up Environment Variables**:
    Create a `.env` file in the root of the project and add your Google AI API key:
    ```
    GOOGLE_API_KEY=YOUR_API_KEY_HERE
    ```

3.  **Run the Development Server**:
    ```bash
    npm run dev
    ```
    The application will be available at `http://localhost:9002`.

## 💡 What's Next for AegisRecruit

-   **Deeper Calendar Integration**: Connect with Google Calendar or Outlook to schedule interviews directly.
-   **AI-Powered Interview Questions**: Generate tailored interview questions based on the candidate's resume and the job requirements.
-   **Full User Authentication & Roles**: Implement a complete authentication system with distinct roles for Recruiters, Hiring Managers, and Administrators.
-   **Automated Candidate Sourcing**: Integrate with platforms like LinkedIn to automatically source and import potential candidates.
