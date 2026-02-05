
# Steganographic Messenger - Progressive Web App (PWA)
    
    ## 🎯 What Is This?
    
    A mobile-ready Progressive Web App that hides secret messages inside normal-looking conversations. Your messages appear completely mundane to anyone reading them, but contain hidden secrets that only the recipient can decode.
    
    ## 📱 How to Install on Your Phone
    
    ### Android (Chrome/Edge/Samsung Internet):
    
    1. Open Chrome browser on your Android phone
    2. Visit the URL where you host these files
    3. Tap the menu button (⋮) 
    4. Select "Install app" or "Add to Home Screen"
    5. Confirm the installation
    6. The app icon will appear on your home screen!
    
    **OR** - When you visit the site, a banner will appear at the bottom saying "Install this app for quick access!" - just tap "Install"
    
    ### iPhone/iPad (Safari):
    
    1. Open Safari browser on your iPhone
    2. Visit the URL where you host these files
    3. Tap the Share button (square with arrow pointing up)
    4. Scroll down and tap "Add to Home Screen"
    5. Name it "StegoMsg" or whatever you prefer
    6. Tap "Add"
    7. The app icon will appear on your home screen!
    
    ## 🚀 How to Use
    
    ### Encoding (Hiding a Message):
    
    1. Open the app and make sure "Encode Message" tab is selected
    2. Type your secret message in "Your Secret Message"
    3. (Optional) Paste a message you received in "Received Message" - this makes your response contextually relevant
    4. Tap "Generate Hidden Message"
    5. Copy the mundane-looking message and send it normally (SMS, WhatsApp, email, etc.)
    
    ### Decoding (Revealing a Message):
    
    1. Switch to "Decode Message" tab
    2. Paste the mundane message you received
    3. Tap "Extract Hidden Message"
    4. Your secret message appears!
    
    ## 🔐 How It Works
    
    The app uses **whitespace steganography**:
    - Single space between words = binary 0
    - Double space between words = binary 1
    - Your text is converted to binary, then hidden in the spacing
    - The mundane text is generated to be contextually relevant to any message you're responding to
    
    ## 📂 Files Included
    
    - `index.html` - Main app file (the PWA)
    - `manifest.json` - PWA configuration (name, icons, colors)
    - `service-worker.js` - Enables offline functionality and installation
    - `icon-192.png` - App icon (192x192)
    - `icon-512.png` - App icon (512x512)
    - `README.md` - This file
    
    ## 🌐 How to Deploy
    
    ### Option 1: GitHub Pages (Free & Easy)
    
    1. Create a new repository on GitHub
    2. Upload all files to the repository
    3. Go to Settings > Pages
    4. Select "main" branch as source
    5. Your app will be live at: `https://yourusername.github.io/repository-name`
    
    ### Option 2: Netlify/Vercel (Free & Fast)
    
    1. Drag and drop all files to netlify.com or vercel.com
    2. Get instant deployment with HTTPS
    3. Share the URL with anyone
    
    ### Option 3: Any Web Host
    
    Upload all files to any web hosting service. Make sure they're served over HTTPS for PWA features to work.
    
    ## ⚠️ Important Notes
    
    - **HTTPS Required**: PWA installation only works on HTTPS sites (not http://)
    - **Context Awareness**: The app tries to match the tone/topic when you paste a received message
    - **Binary Encoding**: Messages are limited by the length of mundane text generated
    - **Security**: This is obfuscation, not encryption. Use additional encryption for truly sensitive data
    
    ## 🎨 Features
    
    ✅ Works offline after first install  
    ✅ Installs like a native app  
    ✅ Mobile-optimized responsive design  
    ✅ Context-aware mundane text generation  
    ✅ Copy to clipboard functionality  
    ✅ No backend required - runs 100% in browser  
    ✅ No data collection or tracking  
    
    ## 🔧 Customization
    
    To change the app theme colors, edit these values in `manifest.json`:
    - `theme_color` - Browser toolbar color
    - `background_color` - Splash screen background
    
    To modify mundane message templates, edit the `mundaneTemplates` object in `index.html`
    
    ## 📄 License
    
    Free to use, modify, and distribute. No attribution required.
    
    ---
    
    **Enjoy your secret conversations! 🕵️**
    
