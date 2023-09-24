---
title: Spotify Playlist Protection Tool
publishDate: 2023-08-02 00:00:00
img: /assets/Spotify_Playlist_Protection_Tool.png
img_alt: Soft pink and baby blue water ripples together in a subtle texture.
description: |
  Design and develop a web application that safeguards the integrity of a user's Spotify playlists, ensuring their metadata remains consistent even in the face of unwarranted flagging by competitors.
tags:
  - HTML / CSS / JS
  - Django framework (Python)
  - Celery task
  - API
---
## Overview

In the music industry, the visibility and appeal of Spotify playlists play a crucial role in content discoverability. However, non-certified playlists are vulnerable to competitor flags that may result in the undesired alteration of metadata. This project addresses this challenge, ensuring that artists and professionals can maintain their playlist branding without disruption.

## Key Features

1. **Django Web Application**: A user-friendly interface that facilitates Spotify account integration and provides an overview of all user playlists.

2. **Spotify API Integration**: On granting the application necessary permissions, it fetches and stores playlist metadata, such as title, cover image, and description, in the database.

3. **User Customization**: Users can modify and set their preferred metadata for each playlist directly within the application.

4. **Automated Monitoring with Celery & Redis**: For playlists marked as "protected," the application schedules a background task every 5 minutes to verify the consistency of metadata on Spotify against the database.

5. **Real-time Correction**: In the event of a mismatch, the application promptly updates the playlist's metadata on Spotify via the API to match the user's preferred settings.

6. **Optimized API Requests & Multi-Threading**: Given the user's multiple Spotify accounts and numerous playlists, the application employs optimized API requests and multi-threading to reduce the task duration dramatically (from 9 minutes in single thread mode to under 1 second in multi-threaded mode).

## Benefits

- **Brand Consistency**: Assures that the artist's playlists remain branded as intended, enhancing discoverability and listener experience.
- **Efficiency**: Through multi-threading and API request optimization, the application works swiftly, ensuring minimal disruption to the user.
- **Automated Peace of Mind**: Once set, the application autonomously maintains the integrity of the playlists, allowing the artist to focus on their music.
