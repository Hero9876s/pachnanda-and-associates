# Troubleshooting Guide - Website Not Opening

## Common Issues and Solutions

### 1. **Dependencies Not Installed**

**Problem:** `node_modules` folder is missing or incomplete.

**Solution:**
```bash
# Delete node_modules and package-lock.json
rm -rf node_modules package-lock.json

# Reinstall dependencies
npm install
```

**For Windows PowerShell:**
```powershell
Remove-Item -Recurse -Force node_modules, package-lock.json
npm install
```

---

### 2. **Port Already in Use**

**Problem:** Port 3000 is already being used by another application.

**Solution:**
- **Option A:** Stop the other application using port 3000
- **Option B:** Use a different port:
  ```bash
  npm run dev -- -p 3001
  ```
  Then open: `http://localhost:3001`

---

### 3. **Node.js Version Issues**

**Problem:** Node.js version is too old or incompatible.

**Check your version:**
```bash
node --version
```

**Required:** Node.js 18 or higher

**Solution:** Download latest Node.js from [nodejs.org](https://nodejs.org/)

---

### 4. **Build Errors**

**Problem:** TypeScript or build errors preventing the server from starting.

**Solution:**
```bash
# Check for errors
npm run lint

# Try building first
npm run build
```

---

### 5. **Cache Issues**

**Problem:** Next.js cache is corrupted.

**Solution:**
```bash
# Delete .next folder
rm -rf .next

# For Windows PowerShell:
Remove-Item -Recurse -Force .next

# Then restart
npm run dev
```

---

### 6. **Missing Files**

**Problem:** Required files are missing.

**Check if these files exist:**
- `app/layout.tsx`
- `app/page.tsx`
- `app/globals.css`
- `package.json`
- `next.config.js`
- `tailwind.config.js`

---

## Step-by-Step Diagnostic

### Step 1: Verify Installation
```bash
node --version    # Should show v18 or higher
npm --version     # Should show version number
```

### Step 2: Check Dependencies
```bash
npm list --depth=0
```

### Step 3: Clean Install
```bash
# Remove everything
rm -rf node_modules .next package-lock.json

# Reinstall
npm install

# Start server
npm run dev
```

### Step 4: Check for Errors
Look at the terminal output for:
- Error messages (red text)
- Warnings (yellow text)
- Port number (should show `http://localhost:3000`)

---

## Quick Fix Commands

**Complete reset (Windows PowerShell):**
```powershell
cd "C:\Users\adi98\Downloads\major project"
Remove-Item -Recurse -Force node_modules, .next, package-lock.json -ErrorAction SilentlyContinue
npm install
npm run dev
```

**Complete reset (Command Prompt):**
```cmd
cd "C:\Users\adi98\Downloads\major project"
rmdir /s /q node_modules
rmdir /s /q .next
del package-lock.json
npm install
npm run dev
```

---

## Still Not Working?

1. **Check the terminal output** - Look for specific error messages
2. **Try a different browser** - Sometimes browser cache causes issues
3. **Check firewall** - Make sure port 3000 isn't blocked
4. **Restart your computer** - Sometimes helps with port issues

---

## Expected Output When Working

When `npm run dev` works correctly, you should see:
```
▲ Next.js 14.0.4
- Local:        http://localhost:3000
- Ready in 2.3s

✓ Ready in 2.3s
```

Then open `http://localhost:3000` in your browser.








