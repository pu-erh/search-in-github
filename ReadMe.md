## Hello, Github

## <a name='TOC'>🐼 Summary</a>

- [Rules](#rules)
- [Overview](#overview)
- [Exercises](#exercises)
- [Credits](#credits)

## <a name='overview'>🦊 Rules</a>

Hi, here are some rules to carry out this story oav;

- You **MUST** create a git repository named `cx-search-in-github`
- You **MUST** create a file called `.author` with your members firstnames and lastnames followed by a newline.

```sh
~/cx-react-pokemon ❯❯❯ cat -e .author
Majdi Toumi$
Dylan De Sousa$
```

> Of course, you can talk about the subject with other developers, peer-learning is
> the key to be a better developer. Don't hesitate to ask questions or help people on Teams.

> Don't forget, there is no useless question :-)

- You **MUST** return the project before Wednesday January 2021, 6 at 20:00
- You **MUST** add `pu-erh` user as a collaborator.
- YOU **MUST** define all functions signature by yourself :)

## <a name='overview'>🐱 Overview</a>

The purpose of theses exercises is simple, play with github API.

## <a name='steps'>🐨 Steps</a>

### 00 Prélude

The purpose is to create a simple API using [**express**](https://expressjs.com/fr/) and a showcase app using **React.js**<br />
You'll have 2 separate projects in the same repository : A **server** and a **client**

## The server

Create a directory called `server` on the `cx-search-in-github` directory

### 01 Bonjour, Github

Create a `postgreSQL` database called `searchGithub`

### 02 Structures

Take a look at the fields `https://api.github.com/users/$USERNAME`<br />
Using sequelize, create tables that we'll allow you to store these attributes.

> replace $USERNAME with anyone from github

Ex:
```json
{
"login": "majdi",
"id": 1158574,
"node_id": "MDQ6VXNlcjExNTg1NzQ=",
"avatar_url": "https://avatars0.githubusercontent.com/u/1158574?v=4",
"gravatar_id": "",
"url": "https://api.github.com/users/majdi",
"html_url": "https://github.com/majdi",
"followers_url": "https://api.github.com/users/majdi/followers",
"following_url": "https://api.github.com/users/majdi/following{/other_user}",
"gists_url": "https://api.github.com/users/majdi/gists{/gist_id}",
"starred_url": "https://api.github.com/users/majdi/starred{/owner}{/repo}",
"subscriptions_url": "https://api.github.com/users/majdi/subscriptions",
"organizations_url": "https://api.github.com/users/majdi/orgs",
"repos_url": "https://api.github.com/users/majdi/repos",
"events_url": "https://api.github.com/users/majdi/events{/privacy}",
"received_events_url": "https://api.github.com/users/majdi/received_events",
"type": "User",
"site_admin": false,
"name": "Majdi Toumi",
"company": "Mhirba",
"blog": "https://majdi.im",
"location": "France",
"email": null,
"hireable": true,
"bio": "Programming Artisan",
"twitter_username": "majditoumi",
"public_repos": 4,
"public_gists": 6,
"followers": 47,
"following": 14,
"created_at": "2011-10-28T19:21:41Z",
"updated_at": "2020-12-06T16:26:30Z"
}
```

### 03 Workflow

The purpose is to have a routes `/users/:username` that will take a username string in params and then call the github api to fetch the public informations.
On fetch, you must store all datas in your **Postgress** database using [**Knex**](http://knexjs.org/)<br />

> Feel free to architect your database and table as you want.
> To fetch an external API take a look at the package `request`, `node-fetch`, etc.

On a new request, you **MUST** check before if you have the user informations in your database.

## The client

### 01 Yo, ui

Well, let's visuzalize github users datas !<br />

You **MUST** initialize your client using [**create react app**](https://fr.reactjs.org/docs/create-a-new-react-app.html#create-react-app) command.
The purpose is to display a simple page that allow a user to type a github username (input) and then validate and display all others informations.

The directory must be `client`

> In this part, no rules, the purpose is to use basic stuff that you learn from React to create a sexy app.

## 02 Bonuses

We love bonuses, so feel free to add anything you want, example:
- Dark Theme
- ...

## <a name='credits'>🐵 Credits</a>

Craft with :heart: in **Paris**.
