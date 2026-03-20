# How to Open and Run the Website

## Step-by-Step Instructions

### 1. Install Dependencies (First Time Only)

Open your terminal/command prompt in the project folder and run:

```bash
npm install
```

This will install all required packages (Next.js, React, Tailwind CSS, etc.)

**Note:** Make sure you have Node.js installed on your computer. If not, download it from [nodejs.org](https://nodejs.org/)

---

### 2. Start the Development Server

After dependencies are installed, run:

```bash
npm run dev
```

You should see output like:
```
▲ Next.js 14.0.4
- Local:        http://localhost:3000
- Ready in 2.3s
```

---

### 3. Open in Browser

1. **Open your web browser** (Chrome, Firefox, Edge, etc.)

2. **Navigate to:**
   ```
   http://localhost:3000
   ```

3. The website should now be visible!

---

## Quick Commands Reference

| Command | What it does |
|---------|-------------|
| `npm install` | Install all dependencies (run once) |
| `npm run dev` | Start development server |
| `npm run build` | Build for production |
| `npm start` | Run production build |
| `npm run lint` | Check for code errors |

---

## Troubleshooting

### If `npm install` fails:
- Make sure Node.js is installed (check with `node --version`)
- Try deleting `node_modules` folder and `package-lock.json`, then run `npm install` again

### If port 3000 is already in use:
- Next.js will automatically use port 3000, 3001, 3002, etc.
- Check the terminal output for the actual port number

### If the website doesn't load:
- Make sure the development server is running (check terminal)
- Try refreshing the browser (Ctrl+R or Cmd+R)
- Check for any error messages in the terminal

---

## What You'll See

Once running, you can navigate to:
- **Home:** http://localhost:3000
- **About Us:** http://localhost:3000/about
- **Services:** http://localhost:3000/services
- **Contact:** http://localhost:3000/contact
- And all other pages!

---

## Stop the Server

To stop the development server:
- Press `Ctrl + C` (Windows/Linux) or `Cmd + C` (Mac) in the terminal

---

## Need Help?

If you encounter any issues, check:
1. Node.js is installed (`node --version`)
2. You're in the correct project folder
3. Dependencies are installed (`npm install` completed successfully)








