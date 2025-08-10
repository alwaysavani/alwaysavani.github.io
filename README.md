# Avani Chaskar - Personal Portfolio

This is the source code for my personal portfolio website, built with [Astro](https://astro.build/) and designed for deployment on GitHub Pages.

##  Project Setup

1.  **Clone the repository:**
    ```bash
    git clone <your-repo-url>
    cd <your-repo-name>
    ```

2.  **Install dependencies:**
    ```bash
    npm install
    ```

3.  **Start the development server:**
    ```bash
    npm run dev
    ```
    The site will be available at `http://localhost:4321`.

## ✍️ How to Add Content

Content is managed by adding Markdown files to the `src/content/` directory.

### Adding a New Blog Post

1.  Create a new `.md` file inside the appropriate category folder in `src/content/blog/`.
2.  Add the following frontmatter to the top of the file:

    ```markdown
    ---
    title: "Your Blog Post Title"
    pubDate: YYYY-MM-DD
    description: "A short description of your post."
    category: "Engineering" # Or AI, Projects, Leisure
    tags: ["tag1", "tag2"]
    ---

    Your content starts here...
    ```

### Adding a New Project

1.  Create a new `.md` file in `src/content/projects/`.
2.  Add the following frontmatter:

    ```markdown
    ---
    title: "Project Title"
    description: "A brief description of the project."
    stack: "Tech1, Tech2, Tech3"
    repo: "[https://github.com/your-repo-link](https://github.com/your-repo-link)" # Optional
    demo: "https://your-demo-link"   # Optional
    ---
    ```

##  Deployment to GitHub Pages

1.  **Build the site:**
    ```bash
    npm run build
    ```
    This will create a `dist/` folder with the static files for your website.

2.  **Push to GitHub:**
    Commit and push your changes to the `main` branch.

3.  **Configure GitHub Pages:**
    - Go to your repository's **Settings** > **Pages**.
    - Under **Build and deployment**, select **Deploy from a branch**.
    - Choose the `main` branch and the `/dist` folder as the source.
    - Save the changes. Your website will be deployed to `https://<your-username>.github.io/<your-repo-name>/`.