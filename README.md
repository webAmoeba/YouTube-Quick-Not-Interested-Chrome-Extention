# YouTube Quick Not Interested

A lightweight Chrome extension that adds a **Not Interested** button to every YouTube thumbnail, giving you full control over the videos that appear in your feed.

Store links (pending review):
- Microsoft Edge Add-ons: [TBD]
- Firefox Add-ons (AMO): [TBD]
---

## Table of Contents
1. [Features](#features)  
2. [Installation](#installation)  
3. [Usage](#usage)  
4. [Development](#development)  
5. [Contributing](#contributing)  
6. [License](#license)

---

## Features

| Feature                | Details                                                                                         |
|------------------------|-------------------------------------------------------------------------------------------------|
| Two quick actions      | **Not interested** and **Don't recommend channel** buttons appear on each thumbnail.           |
| Native-looking icons   | Uses the same symbols as YouTube's own menu actions.                                             |
| Consistent placement   | Buttons sit in the top-left corner of each card.                                                |
| Hotkeys                | Alt+W - Not interested (History: remove), Alt+Q - Don't recommend channel.                      |
| History support        | On History page, the primary action removes the video from watch history.                       |
| Infinite-scroll ready  | Buttons attach to thumbnails loaded dynamically as you scroll.                                  |
| Resilient to UI changes| A mutation observer re-attaches buttons if YouTube updates its markup.                          |

---

## Installation

### Install in Chrome from Microsoft Edge Add-ons

1. Open the Edge Add-ons listing in Chrome (link above).  
2. Click **Get** (or **Add to Chrome**).  
3. If prompted, allow installation from other stores.  

### Developer Mode

1. **Clone** or **download** this repository.  
2. Open **`chrome://extensions/`** in Chrome.  
3. Enable **Developer mode** (top-right toggle).  
4. Click **Load unpacked** and select the project folder.  
5. Pin the extension icon for quick access (optional).

---

## Usage

1. Go to **YouTube**.  
2. Hover a video card - two buttons appear in the top-left corner.  
3. Click the action you want:
   - **Not interested** - hide the video and train recommendations.  
   - **Don't recommend channel** - stop recommendations from this channel.  
   - On **History** page the primary button removes the video from history.  
4. Hotkeys:
   - **Alt+W** - Not interested (History: remove)  
   - **Alt+Q** - Don't recommend channel

---

## Development

- No build step or dependencies.  
- Source files live in the project root.  
- Content script: `content.js`  
- Stylesheet: `styles.css`

Pull requests are welcome - see [Contributing](#contributing).

---

## Contributing

1. Fork the repo.  
2. Create a feature branch:  
   ```bash
   git checkout -b feature/my-feature
   ```  
3. Commit your changes with clear messages.  
4. Push to your branch and open a pull request.  

Please match the existing code style and include relevant tests or demo notes.

---

## License

Distributed under the **MIT License**. See the [LICENSE](LICENSE) file for details.
