# Welcome to CodeLaunch Pro!

**CodeLaunch Pro** is a professional bookmarklet executor that runs bookmarklets using **uBlock Origin** through advanced script injection techniques. It's designed for developers and power users who need reliable bookmarklet execution even on sites with strict security policies. CodeLaunch Pro features advanced CSP bypassing capabilities, making it work seamlessly across various platforms and websites.

---

## **How to Setup CodeLaunch Pro**

1. **Installing uBlock Origin**  
   Make sure you have **uBlock Origin** installed on your browser. If you don't, download it [here](https://chromewebstore.google.com/detail/ublock-origin/cjpalhdlnbpafiamejdnhcphjbkeiagm).

2. **Modifying Advanced Settings**  
   - Go to:  
     `chrome-extension://cjpalhdlnbpafiamejdnhcphjbkeiagm/advanced-settings.html`  
   - Find `userResourcesLocation`.  
   - Change it from `unset` to:  
     `https://raw.githubusercontent.com/PoisonedTillDeath/apigroup/refs/heads/main/blob.js`

3. **Modifying Custom Filters**  
   - Go to:  
     `chrome-extension://cjpalhdlnbpafiamejdnhcphjbkeiagm/1p-filters.html`  
   - Add the following line of code:  
     ```
     *##+js(blob.js)
     ```

---

## **How to use CodeLaunch Pro**
1. **Opening CodeLaunch Pro**  
   - Press `CTRL + Shift + ~` to open CodeLaunch Pro.
   - If you are warned that the website you are running it on has a strong **Content Security Policy**, it means that some bookmarklets will not work as expected. Those are mainly the ones that create a script referencing an **external source**.

2. **Adding Bookmarklets**  
   - Locate the **"Enter bookmarklet code here"** text input.  
   - You can either:  
     - Copy and paste the bookmarklet code.  
     - Drag the bookmarklet from your bookmark bar into the input field directly.  
   - Click the green **"Add Bookmarklet"** button.
   - Enter the name you'd like for the bookmarklet. The name can be anything, and it can be changed later.
   - You can add as many bookmarklets as you need into CodeLaunch Pro, and they will save even if you close the window or shut down your device.

3. **Executing Bookmarklets**  
   - Once added, your bookmarklet will appear which consists of four buttons:  
     - **Blue button**: Run the bookmarklet.  
     - **Red button**: Remove the bookmarklet.  
     - **Yellow buttons**: Edit the bookmarklet's name and code.
       
   You might come across a website where CodeLaunch Pro completely fails to load on (such as **Github** or any **Google Subdomain**). This occurs because they have a strong **Content Security Policy** that can't be bypassed easily, though there are very few of them.
---
I hope this helps! :)