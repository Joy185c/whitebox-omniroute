# WhiteBox OmniRoute Deployment

OmniRoute gateway deployment for WhiteBox AI.

## Setup

1. Deploy to Render using the `render.yaml`
2. Set these environment variables in Render dashboard:
   - `API_KEY_SECRET` — your chosen master key (keep secret, goes in WhiteBox OMNIROUTE_MASTER_KEY)
   - `OPENAI_API_KEY` — your OpenAI key
   - `ANTHROPIC_API_KEY` — your Anthropic key
   - `GEMINI_API_KEY` — your Google Gemini key
   - `GROQ_API_KEY` — your Groq key

3. Copy the Render service URL and `API_KEY_SECRET` to WhiteBox Vercel env:
   ```
   OMNIROUTE_URL=https://whitebox-omniroute.onrender.com
   OMNIROUTE_MASTER_KEY=<your API_KEY_SECRET>
   ```
