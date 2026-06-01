Method 1: Download & Link Locally (Easiest)
Step 1: Download Monaco Editor
Go to: https://www.jsdelivr.com/package/npm/monaco-editor

Click "Download ZIP" or use this direct link:
https://cdn.jsdelivr.net/npm/monaco-editor@0.33.0/min/vs/
Or download from GitHub: https://github.com/microsoft/monaco-editor/releases

Step 2: Extract Files
Extract the ZIP and copy the entire vs folder into thr same folder as the index.html
  Step 3: Change the Path in index.html
Find this line (around line 1800):

require.config({ 
    paths: { 
        'vs': 'https://cdnjs.cloudflare.com/ajax/libs/monaco-editor/0.33.0/min/vs' 
    } 
});
Change it to:

javascript
require.config({ 
    paths: { 
        'vs': './vs' 
    } 
});
Step 4: Done!
Now Monaco Editor loads from your local folder. No internet required! 


  Method 2: Using npm (For Advanced Users)
If you have Node.js installed:

# 1. Open terminal in your project folder
cd Ryuu-Studio-Pro

# 2. Initialize npm (if you haven't already)
npm init -y

# 3. Install monaco-editor
npm install monaco-editor@0.33.0


For the AI to work add a zhipu api key

# 4. Copy the vs folder to your project root
cp -r node_modules/monaco-editor/min/vs ./vs

# 5. Change the path in index.html (same as Method 1 Step 3) 


