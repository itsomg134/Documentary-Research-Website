# Documentary Research Website

A modern, academic-style web interface for discovering and researching documentary films. This project presents a clean, searchable database interface with filtering capabilities, citation tools, and a focus on research-grade documentary content.


## Overview

This static HTML/CSS/JavaScript website simulates a documentary research platform, allowing users to:
- Search through a curated collection of documentary films
- Filter by subject matter (climate, politics, science, arts, etc.)
- View detailed metadata for each documentary (director, year, region, source archive)
- Access citation tools for academic referencing
- Browse related archival sources

## Features

- **Advanced Search Interface** - Combined search bar with category filtering
- **Subject-Based Browsing** - Interactive pill-style filters for quick topic exploration
- **Documentary Cards** - Rich metadata display including:
  - Title and year
  - Director/producer
  - Geographic focus
  - Source archive/network
  - Brief abstract
- **Research Tools** - Citation buttons and source links for each entry
- **Responsive Design** - Adapts seamlessly from desktop to mobile
- **Interactive Elements** - Live filtering simulation and citation previews

## Technologies Used

- **HTML5** - Semantic document structure
- **CSS3** - Modern layouts with Flexbox and Grid, custom properties, responsive design
- **JavaScript** - Interactive UI elements (filter pills, citation simulation)
- **Font Awesome 6** - Icon library for visual enhancement
- **Google Fonts (Inter)** - Clean, readable typography

## Project Structure

```
documentary-research-site/
├── index.html          # Main website file (contains all HTML, CSS, and JS)
├── README.md           # This documentation file
└── assets/             # (Optional) For custom images/covers
```

The entire application is contained in a single `index.html` file for simplicity and easy deployment.

## Getting Started

### Local Development

1. **Clone or download** this repository
2. **Open the file** in your browser:
   ```bash
   cd documentary-research-site
   open index.html  # On macOS
   # OR
   start index.html # On Windows
   # OR simply double-click the file
   ```
3. **No build process required** - it's pure HTML/CSS/JS

### Customization

#### Adding Your Own Documentary Entries

Each documentary is represented by a `.doc-card` div. To add a new entry:

```html
<div class="doc-card">
    <div class="card-img" style="background-image: linear-gradient(...), url('YOUR-IMAGE-URL');">
        <span class="year-badge"><i class="far fa-calendar"></i> YEAR</span>
    </div>
    <div class="card-content">
        <span class="card-category">CATEGORY · NETWORK</span>
        <div class="card-title">TITLE</div>
        <div class="card-meta"><i class="fas fa-user"></i> DIRECTOR · <i class="fas fa-globe"></i> REGION</div>
        <div class="card-desc">DESCRIPTION/ABSTRACT</div>
    </div>
    <div class="card-footer">
        <a href="#" class="source-link"><i class="fas fa-landmark"></i> SOURCE LABEL <i class="fas fa-up-right-from-square"></i></a>
        <button class="save-btn"><i class="far fa-bookmark"></i> cite</button>
    </div>
</div>
```

#### Modifying Filter Categories

Update the `.topic-pills` section:

```html
<div class="topic-pills">
    <span class="pill active"><i class="fas fa-leaf"></i> YOUR TOPIC</span>
    <!-- Add more pills as needed -->
</div>
```

#### Styling Adjustments

The main color scheme uses:
- Primary blue: `#153e5a`
- Accent orange/red: `#c44536`
- Background: `#f4f7fb`

These can be modified in the CSS `:root` section.

## Future Enhancements

Potential improvements for production use:

- [ ] Connect to real database/API
- [ ] Implement full-text search functionality
- [ ] Add user accounts and saved collections
- [ ] Export citations in multiple formats (BibTeX, RIS, APA, MLA)
- [ ] Integrate with streaming/archive APIs (PBS, BBC, NFB)
- [ ] Add advanced filtering by year, runtime, language
- [ ] Implement dark mode toggle

## Responsive Behavior

The interface adapts to different screen sizes:
- **Desktop**: Full 3-4 column grid layout
- **Tablet**: 2-column grid with adjusted padding
- **Mobile**: Single column, stacked search elements

## Contributing

Contributions are welcome! If you'd like to enhance this project:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is open source and available under the [MIT License](LICENSE).

## Acknowledgments

- Placeholder images via [placecats.com](https://placecats.com)
- Icons by [Font Awesome](https://fontawesome.com)
- Font Inter by [Google Fonts](https://fonts.google.com)

##  Contact

Project Link: [https://github.com/yourusername/documentary-research-site](https://github.com/yourusername/documentary-research-site)

---

*Built for documentary researchers, students, and enthusiasts* 🎬🔍
