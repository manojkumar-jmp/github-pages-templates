# Static Website Generator

This project is a simple static website generator using [Jinja2](https://palletsprojects.com/p/jinja/) templating and Bootstrap 4 for styling.

## Features

- Templated HTML pages with Jinja2
- Bootstrap 5.3.3 styling
- Modular header and footer includes
- Easy to extend with new pages

## Getting Started

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
   ```

2. **Set up a virtual environment (optional but recommended):**
   ```sh
   python -m venv myenv
   .\myenv\Scripts\activate  # On Windows
   source myenv/bin/activate      # On macOS/Linux
   ```

3. **Install dependencies:**
   ```sh
   pip install jinja2 staticjinja
   ```

4. **Build the site:**
   ```sh
   staticjinja build --srcpath templates --outpath dist --static static
   ```
   This will create a dist directory with the rendered HTML files and a copy of style.css
   
## Adding Pages

- Create a new template in the `templates/` directory, extending `_base.html`.
- Add your content in the `{% block body %}` section.
- Rebuild the site with `staticjinja build`.

## License

This project is licensed under the MIT License.
