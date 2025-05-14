# ISS Tracker

The **ISS Tracker** is a Python application that tracks the International Space Station (ISS) as it orbits Earth.
The script checks if th ISS is overhead and if it is nighttime in the user's location.
If both conditions are met, it sends an email notification to the user.

## Features

- Tracks the **ISS** location using the **Open Notify API** (http://api.open-notify.org/).
- Determines if it's night at the specified location using the
  Sunset and sunrise times API (https://sunrise-sunset.org/api)
- Sends an email notification when the ISS is overhead and it's night.

## Technologies Used

- `Python 3.12.2`
- Requests library for API calls
- `SMTP` (Simple Mail Transfer Protocol) for sending emails
- `os` for managing environment variables

## Environment Variables

- `MY_EMAIL`: Your email address used to send notifications.
- `PASSWORD`: An App Password generated in your Google Account
  (used instead of your regular Gmail password when connecting through third-party applications).
- `RECIPIENT_EMAIL`: The email address that will receive the ISS notification

