# Analyze

## Summary

This project, named "Analyze", provides a comprehensive solution for data processing and automated deployment, fulfilling a specific technical brief. It features a Python script (`execute.py`) designed to analyze tabular data from `data.csv` (which is converted from `data.xlsx`), along with a robust GitHub Actions workflow (`ci.yml`). This workflow automates key development practices: linting the Python code with Ruff, executing the data analysis script, and publishing the resulting `result.json` output directly to GitHub Pages. The live demo page serves as an interactive explanation of this entire setup, showcasing the corrected Python script, the converted data, and the CI/CD configuration in detail.

## Live Demo

[Live Demo](https://shantanu-data.github.io/analyze/)

## Setup

No setup is required to view the live demo. The web application is a static HTML, CSS, and JavaScript file, accessible directly via the provided GitHub Pages URL in any modern web browser.

## How to Use

Navigate to the [Live Demo](https://shantanu-data.github.io/analyze/) link. The web application is a static page that explains the repository's setup and solution. You can interact by scrolling through the sections to view:

*   The original and corrected versions of the `execute.py` script, highlighting the non-trivial error fix and typo correction.
*   The content of the `data.csv` file, demonstrating the conversion from `data.xlsx`.
*   The full configuration of the GitHub Actions workflow (`.github/workflows/ci.yml`), detailing how Ruff, the Python script execution, and GitHub Pages deployment are managed.
*   A summary of all checks fulfilled by this solution.

The page is purely informative and illustrative, demonstrating the implementation of the project brief.

## Code Explanation

The live demo application itself is built as a static web page, designed to explain the solution to the "Analyze" task.

*   **`index.html`**: This is the main HTML file that structures the content of the web page. It utilizes Bootstrap 5.3.3 (via CDN) for a modern, responsive design and includes custom CSS for specific styling. Its primary role is to logically present the various components of the "Analyze" solution, embedding explanations and code snippets for `execute.py`, `data.csv`, and `ci.yml`.
*   **CSS**: Styling is primarily handled by Bootstrap, providing a clean and organized layout. Custom CSS, defined within the `<style>` tags in `index.html`, further refines the appearance. This includes specific styles for `pre` (code blocks), headings, alerts, and custom text highlights, ensuring readability and visual hierarchy.
*   **JavaScript**: Embedded at the end of `index.html`, this script is responsible for dynamically populating various code blocks (`<pre>`) on the page. It hardcodes the content for the fixed `execute.py`, `data.csv` conversion, and `ci.yml` to ensure they are always displayed as part of the solution. Additionally, it attempts to fetch the *original* `execute.py` from a `public/execute.py` path (simulating a comparison to the fixed version), handling loading states and potential errors. This JavaScript ensures the demo page is self-contained and effectively presents all aspects of the implemented solution.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more details.