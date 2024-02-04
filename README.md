# Vuejs-Workshop

## Installation Guide

### First Step

First go to https://nodejs.org/en this website and install NodeJs. Any version will be fine but LTS is recommended!

![NodeJs Website](https://private-user-images.githubusercontent.com/79584803/302106741-64255427-c39e-4e15-be9a-c4b7dce54398.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDcwNTQyNjAsIm5iZiI6MTcwNzA1Mzk2MCwicGF0aCI6Ii83OTU4NDgwMy8zMDIxMDY3NDEtNjQyNTU0MjctYzM5ZS00ZTE1LWJlOWEtYzRiN2RjZTU0Mzk4LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDAyMDQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwMjA0VDEzMzkyMFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTgyNTBjN2Q4MjA3ODE2ZDBjOWQ3YmQzNTA3MzlkMjNmZjQ4MjkxMzkzODUyNzAzMzcxMGViYTlmZjVmYzQ1YWUmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.Z0kVaYlxDH5hbdAVJ8Rw0w3HcFmH7kme4Ue1LbPu2PU)

#### MacOS users only!!!

MacOS users if you are familiar with homebrew you can install using this command:

```bash
brew install node
```

### Second Step

Second, go to this https://git-scm.com/ and install git on your machine. Choose the latest version will do.

#### MacOS users only!!!

MacOS users for git it is already installed by default. So there is no need to install again.

![Git Website](https://private-user-images.githubusercontent.com/79584803/302106952-55935e9e-da5b-42bf-85aa-ca4b1ac61c5c.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDcwNTQ0NzQsIm5iZiI6MTcwNzA1NDE3NCwicGF0aCI6Ii83OTU4NDgwMy8zMDIxMDY5NTItNTU5MzVlOWUtZGE1Yi00MmJmLTg1YWEtY2E0YjFhYzYxYzVjLnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDAyMDQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwMjA0VDEzNDI1NFomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTNiNmRlZWY4YzgyN2QwNTFlYjNmMzRhZDUwNjJmYzA1NmVhM2Y5NGM2MzRlMTQyYjFlNGZjYmJlNzE1YTBkYmImWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.bHBHyQ1s8QIkcKvXmGhVqQ4Tg7DAkrwXVe02YCEVBds)

After installing git, you would have to setup a bit for your git to work. Open up your terminal and type the below in:

```bash
git config --global user.name "John Doe"
git config --global user.email johndoe@example.com
```

If you don't have a Github account please do sign up for one as well! Simply click the `Sign In` button on your top right or you may click on this [link](https://github.com/login?return_to=https%3A%2F%2Fgithub.com%2Fgdsc-apu%2Fvuejs-workshop) that links to there as well.

### Third Step

Then open your terminal in vscode or cmd in windows and run the command below:

```bash
npm create vue@latest vuejs-workshop
```

After that choose the options accordingly with this image below:

![installing vuejs in terminal](https://private-user-images.githubusercontent.com/79584803/302106314-99fb64d9-7576-4bb1-be84-0a317603ea04.png?jwt=eyJhbGciOiJIUzI1NiIsInR5cCI6IkpXVCJ9.eyJpc3MiOiJnaXRodWIuY29tIiwiYXVkIjoicmF3LmdpdGh1YnVzZXJjb250ZW50LmNvbSIsImtleSI6ImtleTUiLCJleHAiOjE3MDcwNTM4ODksIm5iZiI6MTcwNzA1MzU4OSwicGF0aCI6Ii83OTU4NDgwMy8zMDIxMDYzMTQtOTlmYjY0ZDktNzU3Ni00YmIxLWJlODQtMGEzMTc2MDNlYTA0LnBuZz9YLUFtei1BbGdvcml0aG09QVdTNC1ITUFDLVNIQTI1NiZYLUFtei1DcmVkZW50aWFsPUFLSUFWQ09EWUxTQTUzUFFLNFpBJTJGMjAyNDAyMDQlMkZ1cy1lYXN0LTElMkZzMyUyRmF3czRfcmVxdWVzdCZYLUFtei1EYXRlPTIwMjQwMjA0VDEzMzMwOVomWC1BbXotRXhwaXJlcz0zMDAmWC1BbXotU2lnbmF0dXJlPTQ0MDhhMzE3YmNmNTQ1YzhiYjY5ZTUzNmIwNzMxNzMzZWYyZjExYjY5YWJmYTI5MjkzNDI3Zjc1OWFlZTVjY2YmWC1BbXotU2lnbmVkSGVhZGVycz1ob3N0JmFjdG9yX2lkPTAma2V5X2lkPTAmcmVwb19pZD0wIn0.LRdQHkMGvvKqy6bZBWenOwe4DABPJNCPC9RYfB2NnPY)

# And.. You are ready to go !!!

Hi I'm Wei Hup, GDSC Web Development Department Lead and will be your speaker for this workshop.

Hope that you guys can learn a thing or two from this workshop and I'm open to feedbacks after the workshop ends. 🤗

# Side note !!! Important

This workshop as it is focused on VueJs, I will not be teaching much about how to setup with Git and Github. I will only be doing it if time allows. You can ping me in Whatsapp or Discord if there is anything you want to ask still.
