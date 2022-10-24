# Rust Zoom

**NOTE** This is still a wip!!! I am making this a public project so that I can share it with my community.

# How to test?

## Setup 
Technically you could test this with a single computer, but it is more fun if you use 2+.

## Steps

1. Open chrome://flags on all the computers that you want to use to test the tele-conferencing system, add the ip of the computer that you will use as the server to the Insecure origins treated as secure list.
<img width="1840" alt="Screen Shot 2022-10-24 at 8 18 15 AM" src="https://user-images.githubusercontent.com/1176339/197534920-6bcc495d-ba14-441a-9ea5-00d3b3b7c738.png">

2. Start the servers on the computer that you intent to use as the server using `make up` (requires docker).

3. Connect all computers to `http://<server-ip>/meeting/<username>/<meeting-id>`

4. Make sure that you "allow" access to your mic and camera:
<img width="1840" alt="Screen Shot 2022-10-24 at 8 23 50 AM" src="https://user-images.githubusercontent.com/1176339/197536159-61f0d9c8-c8fa-454c-8f40-404ed52dca98.png">

5. Click connect on both browsers, and enjoy:

![Oct-24-2022 08-28-17](https://user-images.githubusercontent.com/1176339/197537123-1cfaa463-b5c8-4036-be1f-f710799a9a58.gif)

## 👉 Join our Discord Community
You can join our Discord Community, here is the [invite link](https://discord.gg/JP38NRe4CJ).

## 👨‍💻 Project Structure

Contains 3 sub-projects

1. actix-api: actix web server
2. yew-ui: Yew frontend
3. types: json serializable structures used to communicate the frontend and backend.

# Dockerized workflow

1. Install docker
2. Run one of the supported make commands

```
make test
make up
make down
make build
```
