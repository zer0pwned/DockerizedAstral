# Dockerlized Astral

[**Astral**](https://github.com/astralapp/astral), an open source application that allows you to organize your GitHub Stars with ease. Astral can be used with free hosted version or self hosted instance. However, a dockerlized Astral is not provided so I create this project to share my Astral dockerfile. 

---

## Installation

### Prerequisites
- [Create a new GitHub OAuth App](https://developer.github.com/apps/building-oauth-apps/creating-an-oauth-app/) so you can plug in your API keys.

### Modification
- Modify `.env` file with your Github App ID/Secret/Callback URI
- Modify `docker-compose.yml` with your mysql data path

### Run
- Run `docker-compose build up -d` to have your Astral dockerlized!


### Note
- My `docker-compose.yml` is configured to map `Caddy` port to 8180 on host so I can use my Nginx to proxy all request with HTTPS. You should modify it based on your demand.
