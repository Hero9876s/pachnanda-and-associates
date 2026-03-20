# How to Start the Website Server

## The Error You're Seeing

**"ERR_CONNECTION_REFUSED"** means the development server is NOT running.

## Solution: Start the Server

### Method 1: Using Command Prompt/PowerShell

1. **Open Command Prompt or PowerShell**

2. **Navigate to your project folder:**
   ```bash
   cd "C:\Users\adi98\Downloads\major project"
   ```

3. **Start the server:**
   ```bash
   npm run dev
   ```

4. **Wait for this message:**
   ```
   ▲ Next.js 14.0.4
   - Local:        http://localhost:3000
   - Ready in 2.3s
   ```

5. **THEN open your browser** and go to: `http://localhost:3000`

### Method 2: Using the Batch File

1. **Double-click:** `start-website.bat` in your project folder
2. Wait for the server to start
3. Open browser to: `http://localhost:3000`

## Important Notes

- **The server MUST be running** before you can open the website
- **Keep the terminal window open** while using the website
- **Don't close the terminal** - that will stop the server
- **The website only works while the server is running**

## If It Still Doesn't Work

1. Make sure you're in the correct folder
2. Check if Node.js is installed: `node --version`
3. Install dependencies: `npm install`
4. Try clearing cache: `rmdir /s /q .next` then `npm run dev`

## Quick Command (Copy & Paste)

```bash
cd "C:\Users\adi98\Downloads\major project" && npm run dev
```






