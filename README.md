# buy.ubuntu.com
Code for buy.ubuntu.com site

## Local development

- Clone this repo
- Visit https://canonical-staging.myshopify.com/admin
  - Click "Apps" in the left-hand nav
  - At the bottom of the page, click "Manage private apps"
  - From the list that appears, click "buy-ubuntu-theme-dev"
  - Reveal and copy the contents of the password field
- In the root of the repo, create a `config.yml` with the following content:

```yml
development:
  password: <INSERT COPIED PASSWORD>
  theme_id: "32041336909"
  store: canonical-staging.myshopify.com
```

- Run `npm install`, followed by `npm run start:dev`
- If you're updating SCSS, you'll need to run `npm run watch-scss` in a separate terminal.
