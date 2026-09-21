# FLH AI Mobile Studio (Zero-Ban Progressive Web App)

A mobile-first, dark-glassmorphic Progressive Web App (PWA) designed to control and interact with your private AI compute clusters (Kaggle Dual-T4 GPU, Kaggle CPU, Colab GPU, Colab CPU) directly from your smartphone browser (Safari on iOS or Chrome on Android).

---

## 🚀 3 Ways to Use It on Your Mobile Phone

### Option 1: 1-Click Deploy to Vercel (Recommended)
1. Fork or push `kg-server/mobile_web` to your GitHub.
2. Go to [vercel.com/new](https://vercel.com/new) and import the repository (or drag-and-drop the `mobile_web` directory).
3. Click **Deploy**. Vercel will give you a permanent HTTPS URL like `https://flh-studio.vercel.app`.
4. Open the link on your mobile phone and tap **Share -> Add to Home Screen** (iOS) or **Add to Home Screen** (Android) to use it as a native full-screen app!

### Option 2: Deploy to Cloudflare Pages
1. In Cloudflare Dashboard, go to **Workers & Pages -> Create Application -> Pages**.
2. Connect your Git repository or upload the `mobile_web` directory.
3. Deploy!

### Option 3: Instant Local / Direct Mobile Access
- You can host this folder via any static web server:
  ```powershell
  python -m http.server 3000 --directory kg-server/mobile_web
  ```
- Or access the built-in Gradio mobile UI directly by tapping the `*.gradio.live` link generated in your Kaggle/Colab notebook cell.

---

## 📱 Features
- **Zero-Ban Profile**: Connects via official Hugging Face `*.gradio.live` tunnels. Never requires banned `cloudflared` or `ngrok` reverse proxies on Kaggle or Colab.
- **Full Preset Switching**: Quickly switch between all 70B, 32B, 14B, 8B, 3B, SDXL, Animagine, and Kokoro TTS presets.
- **Local Persistence**: Conversations, active endpoints, and API keys are saved directly in your phone's browser storage (`localStorage`), ensuring your chats never disappear when the Kaggle notebook restarts.
- **Touch Ergonomics**: Sized with $\ge 44\text{px}$ touch targets, dynamic viewport height (`100dvh`), and iOS safe-area insets.
