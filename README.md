# Automated-Social-Media-Content-Pipeline

**Brief description of workflow: **
Schedule Trigger → pulls rows from a Google Sheet → checks for "Pending" status → limits records
Data Prep → converts to Unix timestamp → edits fields → calculates time intervals → filters with IF node
Image Generation → uses Gemini AI to generate an image → processes with JavaScript code → converts to file
Google Drive Storage → searches for existing folder → if folder exists, uploads image directly; if not, creates a new folder first → then uploads image → merge paths together
Facebook Posting → schedules a Facebook post with the generated image
Sheet Update → updates the Google Sheet rows (two separate sheet updates, likely marking status as "Posted" or logging results)

<img width="1868" height="418" alt="image" src="https://github.com/user-attachments/assets/aefb8183-19d6-461e-af59-85c9a7125603" />
