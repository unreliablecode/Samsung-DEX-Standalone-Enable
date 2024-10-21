# Samsung DeX Standalone Mode Enabler

This guide helps you enable **Samsung DeX Standalone Mode**, which allows DeX to run directly on your phone's display without needing an external monitor. 

### Requirements:
- **Rooted device**:  
  - Either **Magisk** or **KernelSU** works.
- **Root Explorer** (or any root file manager).
  - Enable **superuser access** for Root Explorer.
  - Grant superuser permission via:
    - **Magisk** (if prompted)  
    OR  
    - **KernelSU** (manually allow superuser access).

---

## Steps to Enable DeX Standalone Mode:

1. **Open Root Explorer** and navigate to:
   ```
   /system/etc
   ```

2. **Mount the directory as Read/Write (R/W)** to make changes.

3. **Locate and edit** the following file:
   ```
   floating_feature.xml
   ```

4. **Find this tag** inside the XML file:
   ```xml
   <SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>
   ```

5. **Modify the tag value**. It will look similar to:
   ```xml
   <SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>dual,wireless,dexforpc</SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>
   ```

6. **Add `standalone` to the list** like this:
   ```xml
   <SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>dual,standalone,wireless,dexforpc</SEC_FLOATING_FEATURE_COMMON_CONFIG_DEX_MODE>
   ```

7. **Save the file** and **reboot your phone**.

---

## Result:
After rebooting, **DeX Standalone Mode** will be enabled, allowing you to run DeX directly on your phone's screen without external peripherals. 

### Tested Devices:
- Galaxy S9  
- Galaxy S10e  
- Galaxy S10+  
- Galaxy S20+

Enjoy your new DeX experience! 🚀
