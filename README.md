# Github Actions

## Nuggetz CMS `on push` and `on schedule` workflows for Github Actions

These workflows use a recent docker image of Nuggetz to build your website, both when you make 
updates, and also on a schedule, so the website content and be refreshed with no user input.

You can customise the actions - for example change the update frequency - just be
mindful of the github actions build minutes available to your account.

### Setup
- Create a `.github/workflows` folder in your repository
- Copy the `push.yml` and `update.yml` files to that folder
- Copy your website to a `src` folder in the repository
- Create a `public` folder, and a `.gitignore` file in that folder
- Add nuggetz components to html files in your `src` folder, commit and push

The result will be new files in the `public` folder, pushed by default to branch `site`.
The nuggetz components will have been transformed, and the files are ready for moving
to your website hosting platform.

