# EduGenius - AI-Powered Educational Content Generator
EduGenius is an innovative AI-powered platform designed to transform educational content creation. By leveraging advanced AI technology, we empower educators and students to generate high-quality, customized learning materials quickly and efficiently. Say goodbye to hours of manual content creation and hello to intelligent, instant educational resources.

🚀 **Live Demo:** https://edugenius-f21g13qbe-siyamthanda-dlakavus-projects.vercel.app/

## 📚 Overview
EduGenius is an AI-powered platform that generates high-quality educational materials including lesson plans, study guides, worksheets, and assessments. Designed for educators and students to streamline content creation.

## ✨ Key Features
### 🎯 Comprehensive Content Generation

### Feature	Description
* 📝 Lesson Plans	Complete with objectives, activities and assessments:
  - Complete educational blueprints with clear objectives, engaging activities, and comprehensive assessments.
* 📖 Study Guides	Topic summaries with key concepts:
  - Detailed topic summaries highlighting key concepts, definitions, and important information.
* ✍️ Worksheets	Practice problems with answer keys:
  - Practice problems and exercises with automatically generated answer keys.
* 🧠 Assessments	Quizzes and tests with varied question types:
  - Customizable :quizzes and tests featuring multiple question types and difficulty levels.
* 🎨 Custom Templates:
  - Adaptable formats for different subjects and educational levels.

### 🛠️ Technical Excellence
* Frontend Framework:	Next.js 14+ with App Router.
* Styling & UI:	Tailwind CSS for responsive design.
* AI Engine:	OpenAI GPT-4 for intelligent content generation.
* Deployment:	Vercel for seamless hosting.
* State Management:	React Context API.
* Development:	TypeScript for type safety.

## 🚀 Getting Started
### Prerequisites
* Ensure you have the following installed and configured:
  - Node.js (version 18.0 or higher)
  - npm or yarn package manager.
  - OpenAI API key (Get one here)

## Installation & Setup
* Clone repository
  ```bash
  - git clone https://github.com/SiyamthandaD/edugenius.git
  - cd edugenius

* Install dependencies
  ```bash
  npm install
  # or
  yarn install

* Set up environment variables
  ```bash
  cp .env.example .env.local
  
* Edit .env.local and add your configuration
  ```bash
  OPENAI_API_KEY=your_openai_api_key_here
  NEXT_PUBLIC_APP_URL=http://localhost:3000

* Run development server
  ```bash
  npm run dev
  # or
  yarn dev

Open your browser
Navigate to *http://localhost:3000* to access EduGenius

* Building for Production
  ```bash
  # Create production build
  npm run build
  # Start production server
  npm start

## 🤖 AI Implementation
### Advanced Content Generation
* EduGenius leverages GPT-4 with specialized educational prompts to create high-quality content:
  ```javascript
   async function generateEducationalContent(contentType, topic, gradeLevel, specifications) {
    const prompt = `
      As an expert educational content creator, generate ${contentType} about "${topic}" 
      for ${gradeLevel} grade students.
      
      Requirements:
      - Educational level: ${gradeLevel}
      - Content type: ${contentType}
      - Key focus areas: ${specifications.focus}
      - Learning objectives: ${specifications.objectives}
      - Format: Structured educational content
      
      Please provide comprehensive, accurate, and engaging content suitable for the specified grade level.
    `;
  
  const response = await openai.chat.completions.create({
    model: "gpt-4",
    messages: [{ role: "user", content: prompt }],
    temperature: 0.7,
    max_tokens: 2000
  });
  
  return response.choices[0].message.content;
  }

* Content Types Supported
   - Lesson Plans: Objectives, materials, procedures, assessments.
   - Study Guides: Summaries, key concepts, review questions.
   - Worksheets: Exercises, problems, activities with solutions.
   - Assessments: Multiple choice, short answer, essay questions.

## 🏗️ Project Structure
* EduGenius - TeachiQ
  ```bash
    edugenius/
  ├── app/                  # Next.js app directory
  │   ├── generate/         # Content generation pages
  │   ├── templates/        # Educational templates
  │   ├── layout.tsx        # Root layout
  │   └── page.tsx          # Home page
  ├── components/           # React components
  │   ├── ui/               # Reusable UI components
  │   ├── forms/            # Input forms and controls
  │   ├── content/          # Content display components
  │   └── layout/           # Layout components
  ├── contexts/             # React contexts
  │   └── AppContext.tsx    # Global state management
  ├── lib/                  # Utility libraries
  │   ├── openai.ts         # OpenAI API integration
  │   ├── prompts.ts        # AI prompt templates
  │   └── utils.ts          # Helper functions
  ├── styles/               # Global styles
  ├── public/               # Static assets
  └── types/                # TypeScript type definitions

## 📊 Usage Guide
* Content Generation
  - Select content type (Lesson Plan, Study Guide, etc.)
  - Specify topic and educational level.
  - Add specific requirements or focus areas.
  - Generate and review AI-created content.
* Customization
  - Edit generated content directly.
  - Adjust difficulty levels.
  - Modify templates to suit specific needs.
  - Add personal teaching style.
* Export & Distribution
  - Copy content to clipboard.
  - Save as Markdown files.
  - Print directly from browser.
  - Share with students or colleagues.
 
## 🛠️ Development
* Available Scripts
  ```bash
  # Development
  npm run dev
  # Production build
  npm run build
  # Start production server
  npm start
  # Linting
  npm run lint
  # Type checking
  npm run type-check

* Environment Variables
  - [Variable]: OPENAI_API_KEY - [Description]: Your OpenAI API key - [Required]: Yes.
  - [Variable]: NEXT_PUBLIC_APP_URL - [Description]: Application base URL - [Required]: No.

### 🌟 Roadmap
## 🎯 Completed Features
  - ✅ Basic content generation for multiple formats.
  - ✅ PDF export functionality.
  - ✅ User-friendly interface with Tailwind CSS.
  - ✅ OpenAI GPT-4 integration.
  - ✅ Responsive design for all devices.

## 🚧 In Development
  - 🔄 Template customization system.
  - 🔄 User accounts and content saving.
  - 🔄 Collaborative editing features.

## 📅 Planned Features
  - 🗓️ Advanced content customization options.
  - 🗓️ Integration with learning management systems.
  - 🗓️ Multi-language support.
  - 🗓️ Student progress tracking.
  - 🗓️ Mobile application.

## 🤝 Contributing
We welcome contributions from the community! Whether you're fixing bugs, adding new features, or improving documentation, your help is appreciated.
## Contribution Workflow
* Fork the repository.
* Create a feature branch
   ```bash
   git checkout -b feature/amazing-feature
* Commit your changes
   ```bash
   git commit -m 'Add some amazing feature'
* Push to the branch
   ```bash
   git push origin feature/amazing-feature
* Open a Pull Request

* Areas for Contribution
  - New educational templates.
  - AI prompt improvements.
  - UI/UX enhancements.
  - Documentation updates.
  - Testing and bug fixes.

## 📄 License
This project is licensed under the MIT License - see the LICENSE file for details.

## 🙏 Acknowledgments
* Technologies & Services
  - OpenAI - For providing the powerful GPT-4 AI model.
  - Next.js - For the robust React framework.
  - Vercel - For seamless deployment and hosting.
  - Tailwind CSS - For beautiful, responsive styling.
* Inspiration
  - Dedicated educators seeking efficient content creation tools.
  - The evolving landscape of AI in education.
  - Open-source educational technology initiatives
  
<div align="center">
🎓 Transform Education with AI
EduGenius is committed to empowering educators and enhancing learning experiences through artificial intelligence.

⭐ Support Our Mission
If you find EduGenius valuable, please consider giving it a star on GitHub!

Built with ❤️ by Siyamthanda Dlakavu

Empowering educators, inspiring students - one AI-generated lesson at a time.

</div>
