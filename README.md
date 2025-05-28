# BlueChat

A simple GitHub Pages site that serves as a podcast RSS feed for MP3 audio files.

## Setup Instructions

1. Fork this repository
2. Enable GitHub Pages in your repository settings (Settings > Pages)
3. Upload your MP3 audio files to the `/audio` folder
4. Update the podcast.xml file with your episode information
5. Commit and push your changes

### File Structure

```
/
├── audio/              # Audio files directory
│   └── episode1.mp3
├── episodes/           # Episode artwork
│   └── ep1-artwork.jpg      # Latest episode artwork is used as main podcast artwork
└── podcast.xml         # RSS feed file
```

Note: The main podcast artwork automatically uses the latest episode's artwork, so there's no need for a separate artwork file.

## Adding New Episodes

To add a new episode:

1. Upload the MP3 file to the `/audio` folder
2. (Optional) Add episode-specific artwork to the `/episodes` folder
   - Image should be square (minimum 1400 x 1400 pixels)
   - Use JPG or PNG format
   - Name it consistently (e.g., `ep1-artwork.jpg`, `ep2-artwork.jpg`)
3. Add a new `<item>` entry in the podcast.xml file with:
   - Title
   - Description
   - Publication date
   - File URL
   - File size (in bytes)
   - Duration
   - Unique GUID
   - Episode artwork (optional) - add an `<itunes:image>` tag with the URL to your episode-specific image
3. Update the index.md file to list the new episode
4. Commit and push your changes

## Subscribing

Users can subscribe to your podcast by adding the following URL to their podcast app:

```
https://morpson.github.io/BlueChat/podcast.xml
```

## Notes

- MP3 files are universally supported by all podcast players
- Make sure your GitHub Pages site is properly configured to serve the files
- The podcast's main artwork automatically updates to use the latest episode's artwork
- Each episode's artwork should be square (minimum 1400 x 1400 pixels)