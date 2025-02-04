# Next.js with Shadcn UI Template

This is a modern web application template built with:
- Next.js 15.1.4
- TypeScript
- TailwindCSS
- Shadcn UI Components

## Project Structure

```
next-mas/
├── src/
│   ├── app/              # Next.js app router
│   │   ├── api/         # API routes
│   │   │   └── upload/  # File upload endpoint
│   │   └── upload/      # Image display page
│   ├── components/       # React components including Shadcn UI
│   │   ├── ui/          # Shadcn UI components
│   │   └── upload-zone/ # Custom drag & drop upload component
│   └── lib/             # Utility functions and shared code
├── public/              # Static assets
│   └── uploads/         # Uploaded files storage
└── package.json         # Project dependencies and scripts
```

## Features
- Modern React development with Next.js
- Type-safe development with TypeScript
- Utility-first CSS with TailwindCSS
- Pre-built UI components from Shadcn UI
- Dark mode support
- Responsive design
- Image upload functionality:
  - Drag & drop support
  - File selection dialog
  - Server-side storage
  - Loading states
  - Error handling
  - Image preview
- Design Analysis:
  - Integration with external analysis API
  - Real-time design feedback
  - Detailed analysis results display
  - Error handling and status updates

## Pages
- `/` - Main page with image upload functionality
- `/upload` - Displays uploaded image and design analysis with back navigation
- `/api/upload` - API endpoint for handling file uploads

## External Services
- Design Analysis API:
  - Endpoint: http://127.0.0.1:8000/analyze-design
  - POST request with image file
  - Returns design analysis in JSON format
  - Error handling with status and message fields

## File Storage
- Uploaded files are stored in `/public/uploads`
- Files are served statically from `/uploads/[filename]`
- Unique filenames with timestamp prefixes
- Automatic directory creation

## Development
- Run `bun run dev` to start the development server
- Access the site at http://localhost:3000
