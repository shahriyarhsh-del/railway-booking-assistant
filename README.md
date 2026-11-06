# Railway Booking Assistant

Free, open-source, **unofficial** Bangladesh Railway booking rules dashboard and Chrome form helper.

## What works
- GitHub Pages dashboard: create, locally save, import and export booking rules.
- One strictly locked seat class, 1–4 passengers, route, date and preferred train/time.
- Chrome extension: locally store/import rules; inspect current page's non-secret form field metadata; attempt conservative form autofill only when one matching field is identified.
- No server, no accounts, no data collection, no paid dependencies.

## What does not work (yet)
- Verified live booking integration, real-time availability, automated class/seat selection, seat holding, checkout or payment.
- No CAPTCHA/OTP bypass, automated retries or unattended purchase.
- The Railway portal is a dynamic web application. Custom widgets may not be filled. Review everything before proceeding.

## Publish to GitHub Pages
1. Create a **public** GitHub repository (for example `railway-booking-assistant`) in your chosen personal account.
2. Upload the **contents** of this project folder to the repository root.
3. In repository **Settings → Pages**, choose **Deploy from a branch**, branch **main**, folder **/docs**, then Save.
4. Your site will be at `https://YOUR-USERNAME.github.io/railway-booking-assistant/` after GitHub publishes it.

## Install extension on macOS Chrome
1. Download the project ZIP and extract it.
2. In Chrome open `chrome://extensions`, enable **Developer mode**.
3. Click **Load unpacked**, select the `extension` folder (not the project root).
4. Open `https://eticket.railway.gov.bd/` and sign in yourself.
5. Set your rules or import the JSON exported from the Pages dashboard.
6. Click **Inspect fields** to check page compatibility, or **Assist form fill** for conservative field filling.
7. Review the page and complete booking yourself.

## Security and privacy
Never commit credentials, NID, passenger information, payment details or exported private data to the public repository. Rules are saved only in local browser storage; exporting a JSON file places it on your device. The extension only requests access to the official ticketing domain and the active tab. The dashboard does not communicate with Railway servers.

## Limitations
This is a functioning configuration/dashboard + limited form assistant, **not a fully automatic ticket-buying bot**. The portal has not been tested live with this extension. Station widgets and class controls may require manual selection. Use only in accordance with the portal's rules.
