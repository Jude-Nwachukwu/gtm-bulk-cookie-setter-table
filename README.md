# GTM Bulk Cookie Setter (Smart) Tag Template

## Overview

The **Bulk Cookie Setter (Smart)** Google Tag Manager (GTM) custom tag template enables you to dynamically set cookies in bulk or through an object configuration. You can configure cookie expiration, path, domain, and advanced rules such as skipping undefined or empty values, refreshing lifespan on each execution, and combining bulk and object-based cookie setups for maximum flexibility.

Developed by **Jude Nwachukwu Onyejekwe** for **[DumbData](https://dumbdata.co/)**.

---

## Features

- 🧩 **Flexible Cookie Setup Modes**
  - **Bulk Only:** Set multiple cookies using a table of name-value pairs.  
  - **Object Only:** Set cookies from an object where each key represents a cookie name and its value represents the cookie value.  
  - **Bulk + Object:** Combine both methods for hybrid cookie creation.

- ⚙️ **Advanced Cookie Handling**
  - Automatically replaces spaces in object key names with underscores (`cookie value 1` → `cookie_value_1`).
  - Option to add a **custom prefix** to cookie names when using the Object configuration mode.
  - Configurable expiration duration and lifespan units (seconds, minutes, hours, days).
  - Optional refresh/update of cookie lifespan on every tag execution.
  - Optional skipping of undefined, null, or empty values to prevent invalid cookie entries.

- 🌐 **Customization Options**
  - Define a **custom domain** and **path** for cookies.
  - Automatic fallback to default values (`auto` for domain and `/` for path).

- 🔒 **Compliant & Safe**
  - Fully compatible with GTM’s **sandboxed JavaScript** environment.
  - Built with GTM Core APIs (`setCookie`, `getCookieValues`, `makeString`, `makeNumber`, `Object`, `getType`).
  - Distributed under the **Apache 2.0 License**.

---

## How to Import

1. Download the tag template file (`.tpl` or `.json`) from the repository.  
2. In your GTM workspace, go to **Templates → Tag Templates**.  
3. Click **Import** and upload the template file.  
4. The **Bulk Cookie Setter (Smart)** template will now be available when creating a new tag.

---

## How to Configure

1. **Add a new tag** in GTM using the imported **Bulk Cookie Setter (Smart)** template.  
2. In the **Set Cookie Method** dropdown, choose how you want to set cookies:
   - **Set Cookie with Bulk Only:** Uses the table configuration only.
   - **Set Cookie with Object Only:** Uses the object configuration only.
   - **Set Cookie with Bulk & Object:** Combines both methods.

### 🧱 Bulk Configuration
3. If using a bulk setup:
   - Populate the **Cookie Name and Value Table** with the cookie names and corresponding values you wish to set.

### 🧠 Object Configuration
4. If using object-based cookies:
   - Enter your object variable in **Cookie Object Variable** (e.g., `{{dlv - userData}}`).
   - Optionally enable **Enable Cookie Name Prefix For Object Keys** to prepend a prefix to all object cookie names.
   - If enabled, enter your prefix in **Enter The Cookie Name Prefix** (e.g., `user_`).

### 🕓 Lifespan & Duration
5. Choose the **Cookie Duration** unit and specify the **Cookie Lifespan** (e.g., 30 days).  
6. Enable **Update cookie lifespan on each execution** to refresh expiration each time the tag fires.  
7. Enable **Do not set cookie if value is undefined, null, or empty** to skip invalid entries.

### 🌍 Advanced Configuration
8. (Optional) Under **Advanced Configuration**, specify:
   - A **custom domain** (e.g., `example.com`).
   - A **custom path** (e.g., `/shop`).

9. **Save** your tag, **test** it in Preview Mode, and **publish** your GTM container.

---

## License

This project is licensed under the **Apache License 2.0** — see the [LICENSE](LICENSE) file for details.

---

## About

Developed with ❤️ by **Jude Nwachukwu Onyejekwe** for **[DumbData](https://dumbdata.co/)**.  
For feedback, issues, or contributions, open an issue in the GitHub repository.

---

⭐ **If you find this template useful, please star the repository and share it with the community!**
