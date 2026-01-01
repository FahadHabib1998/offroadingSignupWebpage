# Email Signup Landing Page

A simple, beautiful landing page for collecting email signups to validate your idea.

## 🚀 Quick Setup

### Option 1: Using Formspree (Recommended - Easiest)

1. **Get a free Formspree account:**
   - Go to [formspree.io](https://formspree.io)
   - Sign up for free (50 submissions/month free)
   - Create a new form
   - Copy your form endpoint URL (looks like `https://formspree.io/f/YOUR_FORM_ID`)

2. **Update the form action:**
   - Open `index.html`
   - Find the line: `action="https://formspree.io/f/YOUR_FORM_ID"`
   - Replace `YOUR_FORM_ID` with your actual Formspree form ID

3. **Host it for free:**
   - **GitHub Pages:** Push to GitHub and enable Pages in settings
   - **Netlify:** Drag and drop the folder to [netlify.com/drop](https://app.netlify.com/drop)
   - **Vercel:** Install Vercel CLI and run `vercel` in this directory

### Option 2: Using Netlify Forms (If hosting on Netlify)

If you're hosting on Netlify, you can use their built-in form handling:

1. Change the form tag in `index.html` to:
   ```html
   <form id="signupForm" name="signup" netlify>
   ```

2. Update the JavaScript fetch URL to:
   ```javascript
   const response = await fetch('/', {
       method: 'POST',
       headers: { "Content-Type": "application/x-www-form-urlencoded" },
       body: new URLSearchParams(formData).toString()
   });
   ```

3. Deploy to Netlify - forms work automatically!

## 📧 Where to Get Emails

- **Formspree:** Check your Formspree dashboard
- **Netlify:** Check your Netlify dashboard → Forms
- Both services can also email you notifications when someone signs up

## 🎨 Customization

- Edit the title, subtitle, and colors in `index.html`
- The gradient colors are in the CSS (currently purple/blue)
- All styling is in the `<style>` tag at the top

## 💡 Free Hosting Options

1. **GitHub Pages** - Free, unlimited
2. **Netlify** - Free tier (100GB bandwidth/month)
3. **Vercel** - Free tier (unlimited)
4. **Cloudflare Pages** - Free tier

All of these are completely free and perfect for this use case!

