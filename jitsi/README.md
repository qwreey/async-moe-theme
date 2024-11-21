# jitsi meet

![preview image](./preview/Screenshot_From_2024-11-21_04-26-57.png)

> [More images](./preview/gallery.md)

## How to apply

Mount `welcome.html` file to `/usr/share/jitsi-meet/static/welcomePageAdditionalContent.html` to inject html file which includes style and script that modify layout.

In `docker-compose.yml`, try

```yml
services:
  jitsi-web:
    ...
    volumes:
      ...
      - ./welcome.html:/usr/share/jitsi-meet/static/welcomePageAdditionalContent.html
  ...
```
