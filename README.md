# EduGenius - AI-Powered Educational Content Generator

[![Vercel Deployment](https://img.shields.io/badge/Vercel-Deployed-black?logo=vercel)](https://edugenius-f21g13qbe-siyamthanda-dlakavus-projects.vercel.app/)
[![GitHub last commit](https://img.shields.io/github/last-commit/SiyamthandaD/edugenius)](https://github.com/SiyamthandaD/edugenius/commits/main)
[![License](https://img.shields.io/badge/License-MIT-blue)](LICENSE)

🚀 **Live Demo:** [https://edugenius-f21g13qbe-siyamthanda-dlakavus-projects.vercel.app/](https://edugenius-f21g13qbe-siyamthanda-dlakavus-projects.vercel.app/)

## 📚 Overview

EduGenius is an AI-powered platform that generates high-quality educational materials including lesson plans, study guides, worksheets, and assessments. Designed for educators and students to streamline content creation.

```mermaid
graph TD
    A[User Input] --> B(AI Processing)
    B --> C{Content Type}
    C --> D[Lesson Plans]
    C --> E[Study Guides]
    C --> F[Worksheets]
    C --> G[Assessments]
✨ Key Features
🎯 Content Generation
Feature	Description
📝 Lesson Plans	Complete with objectives, activities and assessments
📖 Study Guides	Topic summaries with key concepts
✍️ Worksheets	Practice problems with answer keys
🧠 Assessments	Quizzes and tests with varied question types
🛠️ Technical Features
Component	Technology
Frontend	Next.js, Tailwind CSS
AI Engine	OpenAI GPT-4
Deployment	Vercel
State Management	React Context
🚀 Getting Started
Prerequisites
Node.js (v18+)

npm or yarn

OpenAI API key

Installation
bash
# Clone repository
git clone https://github.com/SiyamthandaD/edugenius.git
cd edugenius

# Install dependencies
npm install

# Set up environment variables
cp .env.example .env.local
# Add your OpenAI API key in .env.local

# Run development server
npm run dev
📂 Project Structure
text
src/
├── app/            # Next.js app router
├── components/     # React components
├── context/        # Application context
├── lib/            # Utility functions
├── styles/         # Global styles
public/             # Static assets
🤖 AI Implementation Example
javascript
async function generateLessonPlan(topic, gradeLevel) {
  const prompt = `Generate a detailed lesson plan about ${topic} for ${gradeLevel} grade students.
  Include: objectives, materials, activities, and assessment. Format as Markdown.`;
  
  const response = await openai.chat.completions.create({
    model: "gpt-4",
    messages: [{ role: "user", content: prompt }]
  });
  
  return response.choices[0].message.content;
}
🌟 Roadmap
Basic content generation

Multiple content types

PDF export functionality

Template customization

User accounts system

📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

<div align="center"> <p>Built with ❤️ by Siyamthanda Dlakavu</p> <p> <a
