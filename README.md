# Project Title

**Responsive Navigation and UI Enhancements**

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Code Structure](#code-structure)
7. [Contributing](#contributing)
8. [License](#license)
9. [Contact Information](#contact-information)

---

## Project Overview

This project implements a responsive navigation system and UI enhancements for a web application. It incorporates a modern design with smooth scrolling, sticky navigation, and mobile-friendly features, improving the overall user experience. 

The CSS and JavaScript provided create an engaging and interactive interface, making navigation intuitive and accessible across various devices.

## Features

- **Responsive Design:** Adjusts layout and styling based on screen size.
- **Mobile Navigation:** Toggle functionality for mobile devices, enabling a user-friendly menu.
- **Smooth Scrolling:** Enhances user experience by allowing smooth transitions to different sections of the page.
- **Sticky Navigation:** Keeps the navigation bar fixed at the top when scrolling down.
- **Flexbox Gap Polyfill:** Addresses flexbox gap property issues in Safari, ensuring consistent spacing across browsers.
- **Dynamic Year Display:** Automatically updates the displayed year in the footer.

## Technologies Used

- **HTML5:** Structure of the web pages.
- **CSS3:** Styling of the components and layout.
- **JavaScript:** Interactivity and dynamic behavior of the webpage.
- **Flexbox:** Layout management for a responsive design.

## Installation

To get started with this project, follow these steps:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/project-name.git
   ```

2. **Navigate to the Project Directory:**

   ```bash
   cd project-name
   ```

3. **Open the HTML file:**

   Open the `index.html` file in your preferred web browser to view the project.

## Usage

- **Navigation:** Click on the menu icon on mobile devices to toggle the navigation menu. The links will smoothly scroll to the relevant sections.
- **Sticky Navigation:** As you scroll past the hero section, the navigation bar becomes fixed at the top of the viewport.
- **Dynamic Year:** The current year is automatically displayed in the footer, enhancing the relevance of the footer content.

## Code Structure

The project consists of the following key files:

- **index.html:** The main HTML file that structures the web page.
- **styles.css:** Contains all the CSS styles for the project, including layout, colors, typography, and responsive behavior.
- **script.js:** Implements JavaScript functionalities for mobile navigation, smooth scrolling, sticky navigation, and flexbox gap checks.

### Key Code Snippets

- **CSS Grid for Testimonials and Gallery:**
  ```css
  .testimonials {
      display: grid;
      grid-template-columns: 1fr 1fr;
      row-gap: 4.8rem;
      column-gap: 8rem;
  }
  ```

- **Smooth Scrolling Animation:**
  ```javascript
  allLinks.forEach(function (link) {
      link.addEventListener("click", function (e) {
          e.preventDefault();
          const href = link.getAttribute("href");
          if (href === "#") window.scrollTo({ top: 0, behavior: "smooth" });
          if (href !== "#" && href.startsWith("#")) {
              const sectionEl = document.querySelector(href);
              sectionEl.scrollIntoView({ behavior: "smooth" });
          }
      });
  });
  ```

## Contributing

Contributions are welcome! If you have suggestions for improvements or new features, please fork the repository and submit a pull request. Ensure that your code adheres to the existing style and is well-documented.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact Information

For questions, suggestions, or feedback, please reach out to:

- **Name:** Victor Idam
- **Email:** [your-email@example.com](mailto:your-email@example.com)
- **GitHub:** [your-github-username](https://github.com/your-github-username)
