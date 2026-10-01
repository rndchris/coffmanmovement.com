# Christopher Coffman | Personal Portfolio

The source code and deployment architecture for my personal web portfolio, bridging my work as a contemporary choreographer, strength coach (CSCS), and technical consultant.

**Live Site:** [coffmanmovement.com](https://coffmanmovement.com)

## Architecture & Philosophy

This project was built with a strict focus on performance, minimal dependencies, and clean architecture. Rather than relying on heavy JavaScript frameworks or CMS bloat, the site is constructed using semantic, vanilla HTML5, CSS3, and ES6 JavaScript. 

The aesthetic is built around a custom implementation of the **glassmorphism** design trend, utilizing CSS `backdrop-filter` and carefully managed alpha transparencies to create a dynamic, single-page application (SPA) feel without the overhead of a virtual DOM.

### Key Technical Features
* **Zero-Dependency Frontend:** Fully responsive, lightweight UI built entirely with vanilla CSS and JavaScript.
* **Advanced CSS:** Implementation of true glassmorphism, fluid flexbox layouts, and `drop-shadow` alpha wrapping for transparent media.
* **Dynamic DOM Manipulation:** Custom toggle-to-hide navigation that selectively renders content panes and footer blocks based on user interaction state.
* **SEO & Metadata:** Fully integrated Open Graph tags, Twitter Cards, and JSON-LD structured data for rich search engine indexing.

## Deployment 

The application is designed to be highly portable and is containerized for deployment using Docker and Nginx Alpine. 

### Local Development Setup

1. Clone the repository:
   ```bash
   git clone [https://github.com/rndchris/portfolio-website.git](https://github.com/rndchris/portfolio-website.git)
   cd portfolio-website
   ```

2. Spin up the container using Docker Compose:
   ```bash
   docker-compose up -d
   ```

3. The site will be available locally at `http://localhost:8080`.

*(Note: Ensure your `docker-compose.yml` routes port 80 inside the Nginx container to your preferred local port).*

## Repository Structure
* `/` - Root directory containing the primary `index.html` and deployment configurations.
* `/assets/images/` - Contains all static visual assets, including the custom SVG favicons, background photography, and transparent `.png` headshots.

## License & Usage

The **source code** (HTML, CSS, JS layout logic) is publicly available for review and inspiration. 

However, all **content**, including the code, choreography, and written copy, is the exclusive property of Christopher Coffman. Visual media—including background photography, headshots, and choreography videos—is appropriately credited and used with permission from the respective photographers and videographers. No content from the site may be reused or distributed without explicit permission.