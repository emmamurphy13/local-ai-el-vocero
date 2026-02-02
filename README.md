## Four main takeaways

COPILOT
- **Automated monitoring:** Continuously fetches NHC and NWS feeds and looks for predefined, news‑worthy scenarios.
- **Localized output:** Parses alerts, translates to Spanish (optional DeepL), and renders story fragments from `templates/story_templates/`.
- **Testability & safety:** Includes `test_files/` for local testing and requires explicit `-p/--post` and `-e/--email` flags to actually post/send; parsed-ID files prevent duplicate processing.
- **Deployment notes:** Requires SMTP and Blox credentials and may need IP whitelisting; logging and translation are configurable via environment variables.
