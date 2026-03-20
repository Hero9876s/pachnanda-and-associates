# Website Not Opening - Troubleshooting Guide

## Quick Fixes

### 1. **Clear Cache and Restart**

**Windows PowerShell:**
```powershell
cd "C:\Users\adi98\Downloads\major project"
Remove-Item -Recurse -Force .next -ErrorAction SilentlyContinue
npm run dev
```

**Command Prompt:**
```cmd
cd "C:\Users\adi98\Downloads\major project"
rmdir /s /q .next
npm run dev
```

### 2. **Check if Port 3000 is Already in Use**

If port 3000 is busy, Next.js will use port 3001, 3002, etc.
- Check the terminal output for the actual port number
- Or use a specific port: `npm run dev -- -p 3001`

### 3. **Reinstall Dependencies**

```powershell
cd "C:\Users\adi98\Downloads\major project"
Remove-Item -Recurse -Force node_modules, package-lock.json -ErrorAction SilentlyContinue
npm install
npm run dev
```

### 4. **Check Node.js Version**

```bash
node --version
```
Should be v18 or higher. If not, download from [nodejs.org](https://nodejs.org/)

### 5. **Check for Error Messages**

Look at the terminal output for:
- Red error messages
- Yellow warnings
- Port number (should show `http://localhost:3000`)

## Step-by-Step Diagnostic

### Step 1: Verify You're in the Right Folder
```powershell
cd "C:\Users\adi98\Downloads\major project"
pwd
```

### Step 2: Check if Dependencies are Installed
```powershell
Test-Path node_modules
```
Should return `True`

### Step 3: Try Building First
```powershell
npm run build
```
This will show any build errors

### Step 4: Start Development Server
```powershell
npm run dev
```

### Step 5: Check Terminal Output
You should see:
```
▲ Next.js 14.0.4
- Local:        http://localhost:3000
- Ready in 2.3s
```

## Common Issues

### Issue: "Port 3000 is already in use"
**Solution:** 
- Stop other applications using port 3000
- Or use different port: `npm run dev -- -p 3001`

### Issue: "Cannot find module"
**Solution:**
```powershell
npm install
```

### Issue: "Build failed"
**Solution:**
- Check terminal for specific error
- Clear .next folder: `Remove-Item -Recurse -Force .next`
- Try again: `npm run dev`

### Issue: Browser shows "This site can't be reached"
**Solution:**
- Make sure server is running (check terminal)
- Try `http://127.0.0.1:3000` instead of `localhost:3000`
- Check firewall settings

## Still Not Working?

1. **Share the exact error message** from the terminal
2. **Check if Node.js is installed:** `node --version`
3. **Check if npm is installed:** `npm --version`
4. **Try a different browser**
5. **Restart your computer** (sometimes helps with port issues)

