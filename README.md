![Logo](/frontend/src/Images/logo.png)

![GitHub package.json version](https://img.shields.io/github/package-json/v/damnvulnerablecryptoapp/damnvulnerablecryptoapp?style=flat-square&label=Version)
![GitHub Workflow Status](https://img.shields.io/github/workflow/status/DamnVulnerableCryptoApp/DamnVulnerableCryptoApp/Build?style=flat-square&label=Build)
![GitHub](https://img.shields.io/github/license/damnvulnerablecryptoapp/damnvulnerablecryptoapp?style=flat-square&label=License)
![GitHub repo size](https://img.shields.io/github/repo-size/damnvulnerablecryptoapp/damnvulnerablecryptoapp?style=flat-square&label=Repo%20Size)
![Docker Image Size (latest by date)](https://img.shields.io/docker/image-size/damnvulnerablecryptoapp1/damnvulnerablecryptoapp?style=flat-square&label=Docker%20Image)
![GitHub contributors](https://img.shields.io/github/contributors/damnvulnerablecryptoapp/damnvulnerablecryptoapp?style=flat-square&label=Contributors)
![GitHub commit activity](https://img.shields.io/github/commit-activity/m/damnvulnerablecryptoapp/damnvulnerablecryptoapp?label=Commit%20Activity&style=flat-square)


## Why?

If you try to learn a little bit more about crypto, either because you want to know how the attacks work or just because you want to do safe code, you end up diving really fast into the math behind the algorithms, and for a lot of people this is a NO.

**This project was created with some key points in mind:**
* Real world examples of the crypto attack vectors
* No need to write code to exploit a vulnerability that you are still trying to understand
* No challenge without a solution
* Dead simple documentation. No complex math, no complex formulas. Good old english
* A common place to test different attack vectors
* Make easy for everyone to understand crypto, attacks and preventions.
* Go straight to the point, the challenges are no brain teasers, just a scenario with a crypto vuln. 


## Build
(Make sure you have node installed)

```bash
npm install -g yarn

# This will install necessary dependencies
# (in frontend and backend)
yarn run build-with-deps

# In case you already have dependencies 
# or want to install them manually you can build it with:
# yarn run build
```


## Run

```bash
yarn run start
```

You can change the port with an environment variable: 

```bash
PORT=4000 yarn run start
```


## Docker

### From DockerHub

You can download the latest docker image with:

```bash
docker pull damnvulnerablecryptoapp1/damnvulnerablecryptoapp
```

### Build

If you prefer to build the docker image yourself run:

```bash
npm install -g yarn

yarn build:docker
# or just:
# docker build -t dvca .
```

### Run

By default port 4000 is being exported,
So you can map it to your own port:

```bash
docker run -p 4000:4000 -t dvca
```


# Developing

If you want to to develop new features, or just run without building the app you can start by installing dependencies with:

```bash
# installs deps  both for FE and BE
yarn run install-deps
```

Then you need to run independently the frontend and the backend apps.

## Backend

```bash
cd backend 
yarn start:dev
```

if you want to change the port (default is 4000) you can set an environment variable:

```bash
PORT=3000 yarn start
```

If you changed the server port you need to specify it when booting the frontend, again, as an environment variable:
```bash
REACT_APP_SERVER_PORT=5000 yarn start
```

## Frontend

```bash
cd frontend
yarn start
```

# Documentation
You can find project's documentation on [github wiki](https://github.com/DamnVulnerableCryptoApp/DamnVulnerableCryptoApp/wiki)

# Some other nice projects crypto related
* [Crypton](https://github.com/ashutosh1206/Crypton)
* [RSACtfTool](https://github.com/Ganapati/RsaCtfTool)
* [CryptoHack](http://cryptohack.org/)
* [Cryptopals](https://cryptopals.com/)
* [MysteryTwister C3](https://www.mysterytwisterc3.org/en/)



# License

DamnVulnerableCryptoApp is [MIT](https://tldrlegal.com/license/mit-license) licensed 

# Screenshots

![printscreen1](/docs/screenshots/1.png)
![printscreen2](/docs/screenshots/2.png)
![printscreen3](/docs/screenshots/3.png)
![printscreen4](/docs/screenshots/4.png)
