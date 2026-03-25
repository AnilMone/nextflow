# NextFlow - Complete Setup Guide

## Quick Start (Local Development)

### 1. Clone this repository
```bash
git clone https://github.com/AnilMone/nextflow.git
cd nextflow
```

### 2. Install dependencies
```bash
npm install
# or
yarn install
```

### 3. Create .env.local file
```bash
NEXT_PUBLIC_GEMINI_API_KEY=your_gemini_api_key
NEXT_PUBLIC_API_URL=http://localhost:3000/api
```

### 4. Run development server
```bash
npm run dev
```

Open http://localhost:3000

## Deployment to Vercel

1. Push code to GitHub
2. Go to vercel.com and connect your GitHub account
3. Import this repository
4. Add environment variables in Vercel Settings
5. Deploy

## Project Structure

```
nextflow/
├── app/              # Next.js app directory
├── components/       # React components
├── hooks/            # Custom React hooks  
├─┠─ store/            # Zustand store
├── utils/            # Utility functions
├── public/           # Static files
├── package.json      # Dependencies
├── tailwind.config.js # Tailwind config
├── tsconfig.json     # TypeScript config
└── .env.local        # Environment variables
```

## Features

- ✅ React Flow for visual workflow canvas
- ✅ TypeScript for type safety
- ✅ Tailwind CSS + ShadCN for styling
- ✅ Zustand for state management
- ✅ 6 Node Types (Text, Image Upload, Video Upload, LLM, Crop, Extract Frame)
- ✅ Gemini API integration
- ✅ Vercel deployment ready

## API Endpoints

- `POST /api/gemini` - Run LLM prompts
- `POST /api/upload` - File uploads
- `POST /api/workflows` - Save workflows
- `GET /api/workflows` - Get workflows

## Tech Stack

- **Frontend**: Next.js 14, React 18, TypeScript
- **State Management**: Zustand
- **UI**: Tailwind CSS, ShadCN UI, Lucide Icons
- **Workflow**: React Flow (@xyflow)
- **API**: Gemini API, Trigger.dev
- **Deployment**: Vercel

## Contributing

Feel free to submit issues and enhancement requests!

## License

MIT
