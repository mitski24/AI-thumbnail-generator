# AI-thumbnail-generator
Features
AI-Powered Generation: Uses Google Gemini 2.5 Flash with image generation to create professional thumbnails
Reference Image Support: Upload a reference image to influence the generated thumbnails
Multiple Variations: Generate 3 thumbnails per request with different styles
Modern UI: Clean, intuitive interface built with React 19, TypeScript, and Tailwind CSS 4
Secure: API keys stored locally in your browser, never sent to external servers
Real-time Generation: See thumbnails appear as they're generated
Easy Download: Download or remove generated thumbnails with a single click
Smart Prompts: Optimized prompts designed specifically for YouTube thumbnails with 16:9 aspect ratio
Drag & Drop: Upload images via drag-and-drop or file picker
Quick Start
Prerequisites
Node.js v20.19+ or v22.12+ (required by Vite 7)
Check your version: node --version
If using nvm: nvm use (will use .nvmrc file)
Download Node.js: https://nodejs.org
Google Gemini API key (Get one here)
Installation
Clone the repository:
git clone https://github.com/yourusername/yt-thumbnail-generator.git
cd yt-thumbnail-generator
Install dependencies:
npm install
Start the development server:
npm run dev
Open your browser and navigate to http://localhost:5173
Usage
Add Your API Key: In the top-right corner, enter your Gemini API key and click "Save"
Upload Image: Click the upload area or drag-and-drop to select a reference image (optional)
Add Description: Enter a detailed description of what you want in your thumbnail
Generate: Click the "Generate Thumbnail" button (generates 3 variations)
Download: Hover over any generated thumbnail and click the download icon
Remove: Click the X icon to remove unwanted thumbnails
How It Works
The application uses Google's Gemini 2.5 Flash image generation model to create thumbnails optimized for YouTube. Each generation includes:

High contrast and vibrant colors for better visibility
16:9 aspect ratio perfect for YouTube
Reference image integration - your uploaded image influences the generated thumbnails
Multiple style variations - generates 3 unique thumbnails per request
Optimized prompts that emphasize clickability and engagement
Real-time streaming - see thumbnails as they're generated
API Usage & Costs
This application uses Google's Gemini 2.5 Flash image generation model. Pricing:

Gemini offers a free tier with generous limits for developers
For production use, check current pricing at Google AI Studio
Generating 3 thumbnails typically falls within the free tier limits. Check current pricing

Technology Stack
React 19: Modern UI framework with latest features
TypeScript: Type-safe development
Vite 7: Lightning-fast build tool and dev server
Tailwind CSS 4: Utility-first styling with latest features
Google Gemini API: AI-powered image generation (Gemini 2.5 Flash)
AI SDK by Vercel: Type-safe AI integration
Tabler Icons: Beautiful icon library
Motion (Framer Motion): Smooth animations
React Dropzone: Drag-and-drop file uploads
Development
Build for Production
npm run build
Preview Production Build
npm run preview
Lint
npm run lint
Project Structure
yt-thumbnail-generator/
├── src/
│   ├── components/
│   │   ├── upload.tsx        # Main upload interface with file dropzone
│   │   ├── hero.tsx          # Landing page hero section
│   │   └── Home.tsx          # Home page component
│   ├── lib/
│   │   ├── gemini.ts         # Google Gemini API integration
│   │   └── utils.ts          # Utility functions (cn, etc.)
│   ├── App.tsx               # Main application component
│   ├── main.tsx              # Application entry point
│   ├── App.css
│   └── index.css
├── public/
├── eslint.config.ts          # ESLint configuration
├── tsconfig.json             # TypeScript configuration
├── tailwind.config.js        # Tailwind CSS configuration
├── vite.config.ts            # Vite configuration
├── package.json
└── README.md
Tips for Best Results
Upload a Reference Image: The AI works best when you provide a reference image to build upon

Upload a photo, screenshot, or existing thumbnail to use as a base
Be Specific: Describe colors, mood, style, and key elements

Good: "Epic gaming moment with neon blue and red colors, excited facial expression, bold text saying VICTORY"
Bad: "Gaming thumbnail"
Mention Text: If you want text, specify it clearly

Example: "Include large bold text saying 'TOP 10 TIPS'"
Describe Style: Mention lighting, mood, and aesthetic

Example: "Cinematic dramatic lighting, dark background with spotlight"
Keep It Simple: YouTube thumbnails work best when not overcrowded

Focus on one main subject or message
Iterate: Generate multiple times with different prompts to get the perfect thumbnail

Security & Privacy
Your Gemini API key is stored only in your browser's localStorage
No data is sent to any server except Google's Gemini API
The application runs entirely client-side
You maintain full control of your API key and usage
Images are processed securely through Google's AI infrastructure
Contributing
Contributions are welcome! Please feel free to submit a Pull Request. For major changes, please open an issue first to discuss what you would like to change.

Fork the repository
Create your feature branch (git checkout -b feature/AmazingFeature)
Commit your changes (git commit -m 'Add some AmazingFeature')
Push to the branch (git push origin feature/AmazingFeature)
Open a Pull Request
License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgments
Built with Google Gemini 2.5 Flash
AI SDK by Vercel
Icons by Tabler Icons
Animations by Motion (Framer Motion)
Styled with Tailwind CSS
Troubleshooting
"crypto.hash is not a function" Error
This error occurs when using Node.js version below 20.19. Please upgrade to Node.js v20.19+ or v22.12+:

# Using nvm (recommended)
nvm install 20.19.0
nvm use

# Or download from nodejs.org
# https://nodejs.org
API Key Not Working
Ensure your Gemini API key is correct
Check that you have API access enabled in Google AI Studio
Verify the key has permissions for Gemini API
Images Not Generating
Check browser console for errors
Verify your API key is saved (look at top-right corner)
Ensure your Gemini API has image generation enabled
Check that you haven't exceeded your API quota
