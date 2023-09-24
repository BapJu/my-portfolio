---
title: Spotify Manager
publishDate: 2023-09-01 12:30:00
img: /assets/spotify_namanger_site.png
img_alt: Image of the web site
description: |
  Creation of a web application for Spotify playlist management
tags:
  - HTML / CSS
  - Django framework (Python)
  - Celery task
  - JS / JQuery
  - OAuth / API
---
### 1. Context and Challenge:
A music professional uses Spotify as their primary distribution vector, leveraging musical SEO through playlists. Manually managing these hundreds of playlists was previously a cumbersome process, requiring close to 48 hours of manual work.

### 2. Infrastructure and Technical Stack:
- **Hosting**: Hosted on cPanel, running on the RedHat Linux operating system.
- **Back-end**: Built on the robust Django framework.
- **Authentication**: User authentication managed through Django's built-in authentication system.
- **Integration with Spotify**: OAuth 2.0 integration with Spotify's API for secure track fetching.

### 3. Main Features:

#### - Real-Time Data Fetching:
Post-authentication, the system extracts playlist metadata via Spotify's OAuth 2.0.

#### - Playlist Manipulation:
  - **Individual**: Interface allowing detailed modifications on each playlist.
  - **Batch Processing**: Bulk modifications for optimized management.

#### - Track Management:
  - Addition via copy-paste and matching with the Spotify catalog through asynchronous API calls.

#### - Drag-and-Drop Interface:
  - Built using JS and jQuery, this interface provides an intuitive reordering of tracks.
  - Capability to export in Excel format (.xlsx) for offline tracking.
  - Import configurations from an Excel file to load a previously defined playlist structure.

#### - Task Orchestration:
  - Scheduling modifications using Celery (a task queue) with Redis (as a broker).
  - Planning for track additions or removal at specific dates and times.

#### - Monitoring Dashboard:
  - Consolidated view of scheduled tasks, with cancellation capability.

### 4. Results and Benefits:
This all-in-one solution allows music professionals to maximize their presence on Spotify while minimizing the time spent on manual management. Efficiency is enhanced by leveraging cutting-edge technologies and a UX tailored for the user's specific needs.
