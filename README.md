SkillSync-A 
AI-Powered Interview Preparation & Resume Builder Platform
SkillSync-A is a full-stack AI-powered platform that helps job seekers prepare smarter for interviews. Upload your resume and job description  the AI analyzes the gap between your profile and the role, generates targeted interview questions, and helps you build an ATS-friendly resume.

 What It Does
 Resume + JD Gap Analysis
Upload your resume and paste the job description — the AI identifies exactly where your profile falls short and what skills/keywords are missing for that specific role.
 Targeted Interview Question Generation
Based on your resume and JD, the platform generates 3 types of interview questions:
Relevant Questions — Role-specific conceptual questions (e.g. What is Generative AI? What are common applications?)
Technical Questions — Deep-dive technical questions (e.g. Explain Transformer architecture, self-attention and multi-head attention)
Behavioural Questions — Situational questions based on your experience (e.g. Tell me about a time you used AI to solve a real-world problem)
 ATS-Friendly Resume Builder
Build or improve your resume to be optimized for Applicant Tracking Systems (ATS) — targeted to the specific job description you're applying for.
 Dedicated Interview Preparation
Get a structured, role-specific preparation plan based on your gap analysis — so you know exactly what to study before the interview.

 Tech Stack
Layer
Technology
Frontend
React.js, SCSS
Backend
Node.js, Express.js
AI Integration
OpenAI API
PDF Generation
Resume PDF export
Version Control
Git & GitHub


 Project Structure
SkillSync-A/
├── Frontend/           # React.js application
│   ├── src/
│   │   ├── components/ # UI components
│   │   ├── pages/      # App pages
│   │   └── styles/     # SCSS stylesheets
└── Backend/            # Node.js + Express server
    ├── src/
    │   └── services/   # AI & PDF generation services
    └── server.js


 QA Exploration & Testing Notes
As part of my QA learning journey, I explored this project from a quality assurance perspective:
 Test Scenarios Explored
Resume Upload Validation — Tested behavior with empty file, wrong file format, and oversized files
JD Input Edge Cases — Tested with very short JD, no keywords, and extremely long job descriptions
Gap Analysis Accuracy — Verified that identified skill gaps correctly matched missing keywords between resume and JD
Question Generation Consistency — Checked if Relevant, Technical, and Behavioural questions were always generated across multiple runs
ATS Resume Output — Validated that generated resume included JD-specific keywords and proper formatting
API Error Handling — Identified missing user feedback when OpenAI API response is delayed or fails
PDF Export Testing — Verified resume PDF formatting across different content lengths
 Setup & Installation
Prerequisites
Node.js v18+
npm or yarn
OpenAI API Key
Backend Setup
cd Backend
npm install
# Create .env file and add your API key
npm start
Frontend Setup
cd Frontend
npm install
npm run dev
 Environment Variables
Create a .env file inside the Backend folder:
OPENAI_API_KEY=your_api_key_here
PORT=3000




