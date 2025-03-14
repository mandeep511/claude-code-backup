# OpenAGI

**Note: This repository has been archived. All code is now available in `archive.zip`.**

AI-powered coding assistant with direct filesystem access. No login required, just your API key.

<div align="center">
  <img src="./logo.svg" alt="OpenAGI Logo" width="400" />
</div>

## What is this thing?

OpenAGI is a standalone coding assistant built from the TypeScript code extracted from the official Claude Code package by Anthropic. I've forked and removed the authentication requirements. Now you can use all the features with just an Anthropic API key - no login process needed.

## Installation & Setup

### Option 1: Global Installation (The Easy Way)

```bash
npm install -g open-agi
```

Then run it from any directory:

```bash
openagi
```

### Option 2: Local Development (The Hacker Way)

1. Clone the repository
2. Set up your environment variables:
   ```bash
   # Copy the example file
   cp .env.example .env
   
   # Edit the .env file with your API key
   ANTHROPIC_API_KEY=sk-ant-your-api-key-here
   ```
3. Build the project:
   ```bash
   npm run build:no-types
   ```
4. Run the CLI:
   ```bash
   npm run cli
   # OR if using yarn
   yarn cli
   ```

## Usage

```bash
# Start OpenAGI in the current directory
openagi

# Start with a specific directory
openagi --dir=/path/to/project

# Run in print-only mode (non-interactive)
openagi -p "Generate a React component for a user profile"

# Enable debug mode
openagi -d
```

## Environment Variables

Create a `.env` file with your API key:

```
ANTHROPIC_API_KEY=your_api_key_here
```


## License

MIT (feel free to do whatever, I'm not your boss)