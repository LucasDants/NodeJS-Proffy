<p align="center">
	<img src="https://github.com/Luksdantas/ReactNative-Proffy/blob/main/src/assets/images/landing.png" />
</p>

<h1 align="center">
Proffy API
</h1>

<p align="center">Proffy is a Restfull API of <a href="https://github.com/Luksdantas/ReactJS-Proffy">Proffy Web</a> and <a href="https://github.com/Luksdantas/ReactNative-Proffy">Proffy Mobile</a> </p>


<p align="center">
  <img  src="https://img.shields.io/github/package-json/dependency-version/LuksDantas/NodeJS-Proffy/express" alt="Express Version">
  <img  src="https://img.shields.io/github/package-json/dependency-version/LuksDantas/NodeJS-Proffy/cors" alt="Cors Version">
  <img  src="https://img.shields.io/github/package-json/dependency-version/LuksDantas/NodeJS-Proffy/knex" alt="knex Version">
  <img  src="https://img.shields.io/github/package-json/dependency-version/LuksDantas/NodeJS-Proffy/sqlite3" alt="sqlite3 Version">
  <img  src="https://img.shields.io/github/package-json/dependency-version/LuksDantas/NodeJS-Proffy/dev/typescript" alt="Typescript Version">
</p>

<h1>:memo:About</h1>
<p>Proffy API is a project developed during the <a href="https://nextlevelweek.com.br/">Next Level Week 2</a> presented by <a href="https://www.linkedin.com/school/rocketseat/">Rockeseat</a>.</p>
<p>WEB: <a href="https://github.com/Luksdantas/ReactJS-Proffy">Proffy Web</a></p>
<p>API: <a href="https://github.com/Luksdantas/ReactNative-Proffy">Proffy Mobile</a></p>

<h1>:rocket: Getting started</h1>

```bash

# Clone this repository
$ git clone https://github.com/Luksdantas/NodeJS-Proffy.git

# Access the project folder cmd/terminal
$ cd NodeJS-NPS

# install the dependencies
$ npm install

# Run the application in development mode
$ npm start

# The application will open on the port: 3333 - go to http://localhost:3333

```

<h1>🛠 Proffy API</h1>
<a href="https://github.com/Luksdantas/NodeJS-Proffy/blob/main/Insomnia_2021-03-16.json">Insomnia document</a>

<h2>POST Create Class</h2>
<h3>Request</h3>

`POST /classes`

```
{
  "name": "Lucas Dantas",
	"avatar": "https://avatars.githubusercontent.com/u/55062200?s=460&u=ea1a0fbacb332b79d4068cf99b50533115d141e6&v=4",
  "whatsapp": "85900000000",    
  "bio": "Ensinar é a melhor forma de aprender!",
  "subject": "Física",      
  "cost": 0,
  "schedule": [
    { "week_day": "1", "from": "10:00", "to": "12:00"
    },
    { "week_day": "2", "from": "10:00", "to": "12:00"
    }
  ]
}
```

<h3>Response</h3>

```
```

<h2>GET Classes</h2>
<h3>Request</h3>

`GET /classes?subject=Física&week_day=1&time=10:00`
<h3>Response</h3>

```
[
  {
    "id": 3,
    "subject": "Física",
    "cost": 0,
    "user_id": 3,
    "name": "Lucas Dantas",
    "avatar": "https://avatars.githubusercontent.com/u/55062200?s=460&u=ea1a0fbacb332b79d4068cf99b50533115d141e6&v=4",
    "whatsapp": "85900000000",
    "bio": "Ensinar é a melhor forma de aprender!"
  }
]
```

<h2>POST Create Connection</h2>
<h3>Request</h3>

`POST /connections`

```
{
	"user_id": 3
}
```

<h3>Response</h3>

```

```


<h2>GET Total Connections</h2>
<h3>Request</h3>

`GET /connections`

<h3>Response</h3>

```
{
  "total": 1
}
```

<h1>:bookmark_tabs: License</h1>
 <img  src="https://img.shields.io/github/license/Luksdantas/NodeJS-Proffy" alt="License">
 
 <p>Made with :heart: by Lucas Dantas 👋🏽 <a href="https://www.linkedin.com/in/luksdantas/">Get in Touch!</a></p>
