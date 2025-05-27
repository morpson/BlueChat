# BlueChat

A simple GitHub Pages site that serves as a podcast RSS feed for opus audio files.

## Setup Instructions

1. Fork this repository
2. Enable GitHub Pages in your repository settings (Settings > Pages)
3. Upload your opus audio files to the `/audio` folder
4. Update the podcast.xml file with your episode information
5. Commit and push your changes

## Adding New Episodes

To add a new episode:

1. Upload the opus file to the `/audio` folder
2. Add a new `<item>` entry in the podcast.xml file with:
   - Title
   - Description
   - Publication date
   - File URL
   - File size (in bytes)
   - Duration
   - Unique GUID
3. Update the index.md file to list the new episode
4. Commit and push your changes

## Subscribing

Users can subscribe to your podcast by adding the following URL to their podcast app:

```
https://morpson.github.io/BlueChat/podcast.xml
```

## Notes

- Opus files are supported by most modern podcast players
- Make sure your GitHub Pages site is properly configured to serve the files
- Consider adding a cover image (cover.jpg) to make your podcast more visually appealing