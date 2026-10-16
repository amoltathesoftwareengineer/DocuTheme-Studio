# DocuTheme Studio

**Create clean, responsive, and customizable documentation websites for Python projects.**

DocuTheme Studio is a Python-based documentation theme project designed to help developers build organized and visually appealing documentation websites. It focuses on readability, navigation, responsive layouts, and customization.

## Features

- **Responsive Layout:** Design documentation pages for desktop, tablet, and mobile screens.
- **Custom Styling:** Configure colors, typography, spacing, and page layouts.
- **Navigation System:** Organize documentation with structured navigation menus.
- **Code Presentation:** Display Python examples with readable code blocks.
- **Search-Friendly Structure:** Organize content to make topics easier to locate.
- **Reusable Components:** Create consistent page elements across documentation.
- **Python Integration:** Support integration with Sphinx documentation projects.
- **Customizable Configuration:** Adjust theme settings to suit different projects.
- **Developer Documentation:** Include setup guides, usage instructions, and API documentation.

## Technology Stack

- Python
- Sphinx
- HTML
- CSS
- Jinja templates
- Pytest

## Project Structure

```text
DocuTheme-Studio/
├── docutheme_studio/
│   ├── __init__.py
│   ├── theme.py
│   └── templates/
├── static/
│   ├── css/
│   │   └── style.css
│   └── js/
├── tests/
│   └── test_theme.py
├── docs/
├── pyproject.toml
├── requirements-dev.txt
├── .gitignore
├── LICENSE
└── README.md
```

## Requirements

- Python 3.10 or newer
- pip
- Git (recommended)

## Installation

Clone the repository:

```bash
git clone https://github.com/amoltathesoftwareengineer/DocuTheme-Studio.git
cd DocuTheme-Studio
```

Create and activate a virtual environment on Windows:

```powershell
python -m venv .venv
.venv\Scripts\Activate.ps1
```

Install the project and its development dependencies:

```bash
python -m pip install --upgrade pip
pip install -e .
pip install -r requirements-dev.txt
```

## Usage

The theme is intended to be integrated into a Sphinx documentation project once its theme registration and configuration are implemented.

A Sphinx project can select an installed theme through its `conf.py` configuration:

```python
html_theme = "docutheme_studio"
```

The theme name must match the name registered by the package. The registration entry point and theme configuration must be implemented before this example will work.

## Building Documentation

After configuring the Sphinx documentation project, build the HTML documentation with:

```bash
python -m sphinx -b html docs docs/_build/html
```

## Running Tests

Run the automated tests with:

```bash
python -m pytest
```

## Customization

The project can be extended with:

- Custom color schemes and typography
- Navigation and sidebar layouts
- Responsive page components
- Code block styling
- Configurable header and footer sections
- Additional documentation templates

## Development Roadmap

- [ ] Implement the core theme package.
- [ ] Create theme templates and configuration.
- [ ] Develop responsive CSS styles.
- [ ] Register the theme with Sphinx.
- [ ] Add automated tests.
- [ ] Build an example documentation website.
- [ ] Add installation and customization guides.
- [ ] Configure continuous integration.

## License

Choose and add an appropriate open-source license before distributing the project.

## Author

**Amol Tathe**

GitHub: https://github.com/amoltathesoftwareengineer
