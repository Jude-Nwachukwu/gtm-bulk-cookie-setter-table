# GTM Bulk Cookie Setter Tag Template

## Overview

This Google Tag Manager (GTM) custom tag template allows you to set multiple cookies dynamically based on a table of cookie names and their corresponding values. You can configure cookie expiration, path, and domain, with advanced options to skip undefined or empty values and to refresh cookie lifespan upon each tag execution.

Developed by Jude for DumbData.

## Features

- Set multiple cookies from a user-defined table of name-value pairs.
- Configurable expiration periods (seconds, minutes, hours, days).
- Customizable cookie domain and path.
- Option to skip setting cookies when the value is undefined, null, or empty.
- Option to refresh/update cookie lifespan on every tag execution.
- Works within GTM’s sandboxed JavaScript environment.
- Uses Apache 2.0 License.

## How to Import

1. Download the tag template file (`.tpl` or `.json`) from the repository.
2. Open Google Tag Manager.
3. Navigate to **Templates** > **Tag Templates**.
4. Click **Import** and upload the downloaded template file.
5. The template will now be available when you create a new tag.

## How to Configure

1. Add a new tag in GTM using the imported Cookie Setter tag template.
2. Populate the **Cookie Name and Value Table** with the cookie names and their corresponding values you want to set.
3. Set the cookie expiration unit and lifespan (e.g., minutes, hours).
4. (Optional) Set the cookie domain and path or leave default (`auto` domain and `/` path).
5. Enable **Skip setting cookies with undefined/null/empty values** to avoid storing invalid cookies.
6. Enable **Update cookie lifespan on each execution** to refresh expiration on each tag fire.
7. Save and publish your container.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## About

Developed With 😍 by **Jude Nwachukwu Onyejekwe** for **[DumbData](https://dumbdata.co/)**. For support or questions, open an issue in the GitHub repository.

---

Thank you for using this tag template!  
Please star the repo if you find it helpful.
