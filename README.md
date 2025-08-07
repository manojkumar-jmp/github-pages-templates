📘 See [DISCLAIMER](https://github.com/manojkumar-jmp/.github/blob/main/DISCLAIMER.md) for legal and usage disclaimers related to this repository.

# Static Website Generator

This project is a simple static website generator using [Jinja2](https://palletsprojects.com/p/jinja/) templating and Bootstrap 5.3.3 for styling.

Sample Static Website generated using this repo is live [here](https://manojkumar-jmp.github.io/github-pages-templates/). 

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
  ** On Windows**
  
   ![image](https://github.com/user-attachments/assets/d4f8269a-6af4-4887-81a0-92e9cd6fd18d)

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

##### This is a personal project. All views expressed here are mine and are not affiliated with, nor endorsed by, my current or past employers. All sample code is for educational use only.
