# Image Downloader Automation

This repository automates the process of downloading images from Google Custom Search API for a list of titles.

## Setup

1. Go to your repository on GitHub.
2. Navigate to **Settings → Secrets and variables → Actions**.
3. Add the following secrets:
   - `GOOGLE_API_KEY` → Your Google API key
   - `SEARCH_ENGINE_ID` → Your Google Custom Search Engine ID

## Usage

- Add your titles to `titles.txt`.
- The GitHub Actions workflow will:
  - Read each title.
  - Fetch 2 images from Google Custom Search API.
  - Rename them with the title name.
  - Save all images in a zip file `images.zip` as an artifact.

## Run Workflow

1. Go to the **Actions** tab.
2. Select `Image Downloader` workflow.
3. Click **Run workflow**.
4. After it finishes, download `images.zip` from artifacts.
