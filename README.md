# Mermaid Diagram Sketcher 🎨

An interactive web application for creating beautiful flowcharts and diagrams using Mermaid syntax with AI assistance.

**Created by:** Satyam Kumar  
**Contact:** satyamkmr37@gmail.com  
**Live Demo:** [View Application](https://lovable.dev/projects/e751f4c0-8ecf-4b68-92d9-99805a66e66e)

## 🚀 What This Project Does

This application helps users create professional diagrams and flowcharts using:
- **Mermaid Syntax**: Industry-standard diagramming language
- **AI-Powered Generation**: Describe your diagram in plain English, get Mermaid code
- **Live Preview**: See your diagrams render in real-time as you type
- **Export Functionality**: Save your diagrams as SVG files
- **Dark/Light Mode**: Toggle between themes for comfortable viewing

## 🛠️ Technical Implementation

### Architecture Overview
- **Frontend Framework**: React 18 with TypeScript for type safety
- **Build Tool**: Vite for fast development and optimized builds
- **Styling**: Tailwind CSS with custom design tokens
- **UI Components**: Shadcn/ui component library
- **Diagram Rendering**: Mermaid.js library for diagram visualization
- **State Management**: React hooks (useState, useEffect)
- **File Export**: FileSaver.js for SVG export functionality

### Key Features I Built

#### 1. **Dual-Panel Interface**
```typescript
// Split layout with editor and preview
<div className="grid grid-cols-1 md:grid-cols-2 gap-6">
  <Editor /> {/* Left panel for code editing */}
  <Preview /> {/* Right panel for live preview */}
</div>
```

#### 2. **Real-time Diagram Rendering**
- Integrated Mermaid.js with React lifecycle
- Custom error handling for invalid syntax
- Loading states for better user experience
- Theme synchronization between app and diagrams

#### 3. **AI Prompt Integration**
- Tab-based interface switching between manual code and AI prompts
- Structured prompt handling for diagram generation
- User-friendly error messaging

#### 4. **Export System**
- SVG extraction from rendered diagrams
- Dynamic filename generation based on diagram content
- Toast notifications for user feedback

### Development Challenges Solved

1. **Mermaid Integration**: Had to carefully manage Mermaid initialization and re-rendering when themes change
2. **Theme Consistency**: Ensured diagrams match the application's dark/light mode
3. **Error Handling**: Implemented graceful error handling for invalid Mermaid syntax
4. **Responsive Design**: Created a layout that works on both desktop and mobile devices

## 🏗️ Project Structure

```
src/
├── components/
│   ├── ui/           # Reusable UI components (buttons, dialogs, etc.)
│   ├── Header.tsx    # Top navigation with export and theme toggle
│   ├── Editor.tsx    # Code editor with tab interface
│   ├── Preview.tsx   # Mermaid diagram renderer
│   └── AIPrompt.tsx  # AI prompt handling component
├── pages/
│   ├── Index.tsx     # Main application page
│   └── NotFound.tsx  # 404 error page
├── hooks/            # Custom React hooks
├── lib/              # Utility functions
└── utils/            # API and helper functions
```

## 💻 Technologies Used

- **React 18**: Modern React with hooks and functional components
- **TypeScript**: Static typing for better code quality and developer experience
- **Vite**: Fast build tool and development server
- **Tailwind CSS**: Utility-first CSS framework for rapid styling
- **Mermaid.js**: Diagram and flowchart library
- **Shadcn/ui**: Modern, accessible component library
- **Lucide React**: Beautiful icon library
- **React Query**: Data fetching and caching (for future API integration)

## 🔧 Setup and Installation

```bash
# Clone the repository
git clone <repository-url>

# Navigate to project directory
cd mermaid-diagram-sketcher

# Install dependencies
npm install

# Start development server
npm run dev

# Build for production
npm run build
```

## 🎯 Future Enhancements

- [ ] User authentication and diagram saving
- [ ] Collaboration features for team diagram editing
- [ ] More diagram types (Gantt charts, sequence diagrams, etc.)
- [ ] Template library for common diagram patterns
- [ ] Export to multiple formats (PNG, PDF, etc.)

## 🎨 Design Principles

- **User-Centric**: Clean, intuitive interface prioritizing ease of use
- **Responsive**: Works seamlessly across all device sizes
- **Accessible**: Proper contrast ratios and keyboard navigation
- **Performance**: Optimized rendering and minimal bundle size

## 📈 What I Learned

This project helped me understand:
- **Complex State Management**: Managing multiple interconnected states (code, preview, themes)
- **Third-party Library Integration**: Working with Mermaid.js and handling its lifecycle
- **Modern React Patterns**: Hooks, context, and component composition
- **Build Tools**: Vite configuration and optimization
- **User Experience**: Creating intuitive interfaces for technical tools

---

**Note**: This project demonstrates my ability to build modern, interactive web applications using current industry standards and best practices. The clean architecture and thoughtful user experience design showcase my understanding of both technical implementation and user-centered design principles.