# 🌊 Serene Bay — Vercel & GitHub Static Studio

This version uses your actual GitHub account credentials to let you log into your `/admin` panel securely on your live website. No database passwords required.

---

## 📁 Step 1: Organize and Upload Your Repository
1. Create a brand-new repository on GitHub named `serene-bay`.
2. Make sure your local folder structure looks exactly like this:
   * `index.html`
   * `admin/index.html`
   * `admin/config.yml`
3. Drag both files and the `admin` folder directly into your GitHub web page drop-zone and click the green **Commit changes** button.

---

## 🚀 Step 2: Deploy to Vercel
1. Log into your account at [https://vercel.com](https://vercel.com).
2. Click **Add New...** -> **Project**.
3. Locate your `serene-bay` repository and click **Import**, followed by **Deploy**. Vercel will give you a live address link.

---

## 🔐 Step 3: Link Your GitHub Authentication (Final Step)
Because you want to prevent strangers from accessing your website editor, you need to quickly tell GitHub that *you* are the owner allowed to edit files.
1. In a new browser window, go to your GitHub Settings page: **Settings** -> **Developer Settings** (at the very bottom left) -> **OAuth Apps** -> **New OAuth App**.
2. Fill out the form fields exactly like this:
   * **Application Name:** `Serene Bay Studio`
   * **Homepage URL:** Paste your live Vercel website link (e.g., `https://serene-bay.vercel.app`)
   * **Authorization callback URL:** Paste this exact universal handler link: `https://decap-cms-oauth-vercel.vercel.app/callback`
3. Click **Register Application**.
4. Click the button that says **Generate a new client secret**.
5. Copy your **Client ID** string and your new **Client Secret** string.

---

## ✍️ Step 4: Write and Edit Content Live!
1. Go to your live Vercel website address and add `/admin/` to the end of the URL.
2. Click the **"Login with GitHub"** button. 
3. Type in your GitHub username/password when the prompt box pops up. 
4. Your beautiful WYSIWYG editor dashboard will open instantly. Whenever you create a post and hit save, your code will safely create real text files inside a new `/journal/` folder inside your GitHub profile, and your live Vercel site will refresh automatically with the updates!
