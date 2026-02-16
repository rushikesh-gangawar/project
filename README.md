# ResumeFlow: AI-Powered Resume Builder

This is a Next.js application that helps users build resumes, generate cover letters, and find job recommendations using AI.

## Getting Started

Follow these instructions to get a copy of the project up and running on your local machine for development and testing purposes.

### Prerequisites

- Node.js (v18 or later)
- npm or yarn

### Installation

1. Clone the repository to your local machine:
   ```bash
   git clone <your-repository-url>
   ```

2. Navigate to the project directory:
   ```bash
   cd <project-directory>
   ```

3. Install the dependencies:
   ```bash
   npm install
   ```

## Environment Variables

This project uses Genkit with Google's Gemini models for its AI features. To use them, you need to provide an API key.

1.  Create a file named `.env.local` in the root of your project.
2.  Add your Gemini API key to this file:
    ```
    GEMINI_API_KEY=your_gemini_api_key_here
    ```
    You can get a free API key from [Google AI Studio](https://aistudio.google.com/app/apikey).

## Running the Development Server

To start the development server, run:

```bash
npm run dev
```

Open [http://localhost:9002](http://localhost:9002) with your browser to see the result.

## Deployment on Vercel

You can easily deploy this application to Vercel.

1.  **Import Project:** Go to your Vercel dashboard and import the project from your Git repository.
2.  **Configure Environment Variables:** In the project settings on Vercel, add the `GEMINI_API_KEY` as an environment variable with the same value you used in your `.env.local` file.
3.  **Deploy:** Vercel will automatically detect that this is a Next.js project and deploy it. The configuration in `vercel.json` ensures that the Genkit AI flows are correctly deployed as serverless functions.
