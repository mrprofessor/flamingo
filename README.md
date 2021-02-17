# Flamingo

A bland theme for boring people.

## Example
  - https://rudra.dev

## Probably useful stuff

1. Add the site variables for some links to work. Also needed for seo tags.

    ```toml
    [params]
      author = "your name"
      description = "Blog about this and that."
      sitename = "My cool blog"
      github = "https://github.com/username"
      twitter = "@username"
      favicon = "/images/favicon.ico"
      resume = "https://example.com/resume.pdf"
    ```

2. For the projects page to work, there must be a `projects.md` file or a `projects/_index.md` in `content/` folder.
  - The contents of the file
    ```md
      +++
      title = "Projects"
      layout = "projects"
      draft = false
      +++
    ```
 - Additionally the projects data can be added in the `config.toml`
    ```toml
      # Projects list
      [[params.projects]]
        name = "project1"
        description = "First project 📚"
        demoLink = "https://example.com/project1/"
        sourceLink = "https://github.com/username/project1"


      [[params.projects]]
        name = "project2"
        description = "Second project 📚"
        demoLink = "https://example.com/project2/"
        sourceLink = "https://github.com/username/project2"
    ```

3. The theme supports [utterances](https://utteranc.es/) comments by default. This can be easily replaced with discourse or whatever in `partials/comments.html`.

4. SEO stuff can be added to the `partial/meta.html`


## TODOs
  - Include an example site.
  - Better docs.
