# Getting started
Run `npm install`

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

### Building the project
Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `-prod` flag for a production build.

## Functionality Overview
General functionality:

1. Authenticate users via JWT (login/signup pages + logout button on settings page)
2. CRU* users (sign up & settings page - no deleting required)
3. CRUD Articles
4. CR*D Comments on articles (no updating required)
5. GET and display paginated lists of articles
6. Favorite articles
7. Follow other users

### The general page breakdown looks like this:

Home page (URL: /#/ )
List of tags
List of articles pulled from either Feed, Global, or by Tag
Pagination for list of articles
Sign in/Sign up pages (URL: /#/login, /#/register )
Uses JWT (store the token in localStorage)
Authentication can be easily switched to session/cookie based
Settings page (URL: /#/settings )
Editor page to create/edit articles (URL: /#/editor, /#/editor/article-slug-here )
Article page (URL: /#/article/article-slug-here )
Delete article button (only shown to article's author)
Render markdown from server client side
Comments section at bottom of page
Delete comment button (only shown to comment's author)
Profile page (URL: /#/profile/:username, /#/profile/:username/favorites )
Show basic user info
List of articles populated from author's created articles or author's favorited articles.

### For data fetching 
I am using open api : ` https://conduit.productionready.io/api `