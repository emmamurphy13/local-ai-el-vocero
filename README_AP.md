![Reporte especial hero image](images/reporte_especial.jpg)

# Weather Bot — El Vocero (AP-style) 🗞️

Associated Press/Local News — Weather Bot monitors National Hurricane Center (NHC) and National Weather Service (NWS) feeds, identifies alerts that affect Puerto Rico, generates Spanish story fragments and email notifications, and can post directly to El Vocero's Blox CMS.

---

## Four quick takeaways ✅

- **Automated monitoring:** Continuously fetches NHC and NWS feeds and looks for predefined, news‑worthy scenarios.
- **Localized output:** Parses alerts, translates to Spanish (optional DeepL), and renders story fragments from `templates/story_templates/`.
- **Safe by default:** Includes `test_files/` for local testing and requires explicit `-p/--post` and `-e/--email` flags to actually post/send; parsed ID files prevent duplicate processing.
- **Deployment notes:** Requires SMTP and Blox credentials and may need IP whitelisting; logging and translation are configurable via environment variables.
