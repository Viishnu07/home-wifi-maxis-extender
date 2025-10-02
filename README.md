# home-wifi-maxis-extender
networking, home-lab, Wi-Fi, maxis, easy-mesh, extender/AP

# 🏠 Extending Home Wi-Fi with Maxis Routers 

## 📌 Introduction
When I shifted into a double-storey house, I noticed poor Wi-Fi coverage in the kitchen and backyard.  
My main Maxis router (Wi-Fi 6, model LG8245X6) was installed on the **1st floor**, but the **kitchen is at the back of the ground floor**.  

Instead of buying a new mesh kit, I reused my **old Maxis router** to extend coverage and improve speed in dead zones.

---

## ⚡ Problem Statement
- Subscribed speed: **100 Mbps**  
- Router placement: **upstairs, near front of house**  
- Issue: **Wi-Fi slows down or drops** at the back kitchen on ground floor.  
- Goal: Extend Wi-Fi coverage using existing hardware.

---

## 🔧 Solution
Reconfigured my old Maxis router (same model) as a **Wi-Fi extender **.  
Also explored its **USB file sharing feature** for simple network storage.

---

## 🛠️ Steps Taken

### 1. Reset Old Router
- Hold the **Reset button** (6–10 seconds) until LEDs blink.
- Router reboots to factory settings.

### 2. EasyMesh Wireless Pairing
- Place old router near the main router.
- On old router: press **WLAN/WPS button for 10 sec** (LED blinks).  
- On main router: press **WLAN/WPS button for 1–2 sec**.  
- Wait for **Internet LED on old router to turn solid** → paired successfully.  
- Move old router to ground floor, halfway point before kitchen.

### 3. Verify Connection (Mac)
- Hold **Option + click Wi-Fi icon** → check **BSSID**.  
- Compare to MAC address label on each router to confirm.  
- Alternatively: unplug old router → Wi-Fi should drop in kitchen if it was the one serving you.

### 4. Placement Tips
- Don’t place the extender inside the dead zone itself.  
- Place it **where Wi-Fi is still good**, so it can rebroadcast properly.  
- Keep away from fridges, microwaves, or thick concrete walls.

---

## 📂 USB File Sharing via Router
- Inserted a **16 GB USB (exFAT)** into **main router’s USB port**.  
- Enabled **FTP Server** from router’s web UI.  
- Connected from Mac:  
  - Finder → Go → Connect to Server → `ftp://192.168.1.1`  
  - Login with configured username/password.  
- Verified file sharing works (basic NAS functionality).

---

## 📊 Results
- **Before:** Kitchen Wi-Fi speed dropped to unusable levels.  
- **After:** Extended router provides ~50 Mbps in kitchen (half of plan speed due to wireless repeating).  
- ✅ Browsing, streaming (even 4K), and gaming all work fine.

*(Add screenshots of Speedtest results here: Upstairs vs Kitchen)*

---

## 🔒 Security Notes
- Changed default admin passwords on both routers.  
- Disabled WAN-side FTP access (LAN-only for safety).  
- Guest network/IoT segregation possible with old router if needed.

---

## 🚀 Future Improvements
- Add a **3rd router** or **powerline adapter** for stronger coverage in backyard.  
- Use **wired backhaul** (if cabling possible) to avoid the 50% repeater speed penalty.  
- Explore using router USB as **media server (DLNA)** for TVs.

---

## 📎 Diagram
*(Add a simple network diagram — main router upstairs → old router downstairs → devices in kitchen)*

---

## ✅ Conclusion
With two Maxis routers configured in EasyMesh mode, I turned a poor-signal double-storey house into a **whole-home Wi-Fi system** without extra cost.  

This setup is ideal for:
- Anyone with an old Maxis router lying around.
- Home users who want extended coverage without buying a new mesh kit.
- Students/techies who enjoy experimenting with home networking.

---
