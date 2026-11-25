# Vid-tube

A responsive, YouTube-inspired video platform front-end built with plain HTML, CSS, and JavaScript. No frameworks, no build step.

## Features

- **Home page** with a banner and a responsive grid of video cards (thumbnail, channel avatar, title, channel name, views and upload time)
- **Sticky top navigation bar** with logo, search box, voice-search icon, and upload, notification, and profile icons
- **Collapsible sidebar** with shortcut links (Home, Explore, Subscription, Library, History, Playlist, Message) and a subscribed-channels list
- **Sidebar toggle**: clicking the menu icon shrinks the sidebar to icons only and widens the main content
- **Video player page** (`play-video.html`) layout styles: player, video info, publisher row, description, comments, and a related-videos sidebar
- **Responsive design**: layout adapts at widths of 900px and below (sidebar hidden, simplified navbar, single-column content)

## Tech Stack

| Layer     | Technology                  |
| --------- | --------------------------- |
| Structure | HTML5                       |
| Styling   | CSS3 (Flexbox, Grid, media queries) |
| Behavior  | Vanilla JavaScript          |
| Dev tool  | VS Code Live Server         |

## Project Structure

```
Vid-tube/
├── index.html        # Home page
├── play-video.html   # Video player page
├── style.css         # Styles for all pages (including the player page)
├── script.js         # Sidebar toggle logic
├── settings.json     # VS Code Live Server config (port 5503)
└── images/           # Icons, logos, thumbnails, and avatars
```

## Getting Started

### Prerequisites

- A modern web browser
- (Optional) [VS Code](https://code.visualstudio.com/) with the [Live Server](https://marketplace.visualstudio.com/items?itemName=ritwickdey.LiveServer) extension

### Run Locally

1. Clone or download the project:
   ```bash
   git clone <your-repo-url>
   cd Vid-tube
   ```
2. Make sure the `images/` folder is in the project root alongside `index.html`.
3. Open the project:
   - **With Live Server:** right-click `index.html` and choose **Open with Live Server**. The project is configured to run on port `5503`, at `http://127.0.0.1:5503`.
   - **Without Live Server:** double-click `index.html` to open it in your browser.

## Usage

- Click the **menu icon** (top left) to collapse or expand the sidebar.
- Click a video title or thumbnail to open the player page.
- Resize the browser below 900px to see the mobile layout.

## Customization

- **Add videos:** copy a `.vid-list` block in `index.html` and update the thumbnail, avatar, title, channel, and stats.
- **Change colors and sizing:** edit `style.css`. The accent color is `#ed3838` (active sidebar link) and the card text color is `#5a5a5a`.
- **Change the Live Server port:** edit `liveServer.settings.port` in `settings.json`.

## Roadmap

- [ ] Working search
- [ ] Real video playback and data (backend or API)
- [ ] Functional sidebar links and subscriptions
- [ ] Comments, likes, and subscribe actions

## License

This project is for learning and practice. Add a license of your choice (for example MIT) before distributing.
