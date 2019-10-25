# Base template for React

## Task
Implement SearchMovie component to fetch movies data from API.
Use http://www.omdbapi.com/ (You need to register get API key)
1. Create component `SearchMovie` which should have text field and  button
1. When user enter movie title and click on search button, request to `http://www.omdbapi.com/?apikey=[yourkey]&t=:title` should be sent.
1. If film has been found map data to same object as in `NewMovie` component.
Pass this object to `onAdd` callback from props. Clear input value.
1. If film is not found show error message below input. Clear error after next submit.
1. (\*) Modify `addMovie` in `App` to ignore films with imdbId which exists.

## Workflow

- Fork the repository with task
- Clone forked repository 
    ```bash
    git clone git@github.com:<user_name>>/<task_repository>.git
    ```
- Run `npm install` to install dependencies.
- Then develop

## Development mode 

- Run `npm run start` to start `http-server` on `http://localhost:3000`
    When you run server the command line window will no longer be available for 
    writing commands until you stop server (`ctrl + c`). All other commands you 
    need to run in new command line window.
- Follow [HTML, CSS styleguide](https://mate-academy.github.io/style-guides/htmlcss.html)
- Follow [the simplified JS styleguide](https://mate-academy.github.io/style-guides/javascript-standard-modified)
- When you finished `Deploy on gh-pages`

## Deploy on gh-pages

- Build the project
  ```bash
  $ npm run build
  ```
- Commit and push all recent changes
  ```bash
  $ git add .
  $ git commit -m 'commit message'
  $ git push origin master
  ```
- Execute `npm run deploy`. This command will push the `/build` folder to branch
  `gh-pages` in your remote repository. 
- Add links to your demo in readme.md.
  - `[DEMO LINK](https://<your_account>.github.io/<repo_name>/)` - this will be a 
  link to your index.html
- Commit and push all recent changes again.
- Create `Pull Request` from forked repo `(<branch_name>)` to original repo 
(`master`).
- Add a link at `PR` to Google Spreadsheets.

## Project structure

- `src/` - directory for css, js, image, fonts files
- `build/` - directory for built pages

You should be writing code in `src/` directory.

### Demo link

Add link here: `[DEMO LINK](https://<your_account>.github.io/<repo_name>/)`