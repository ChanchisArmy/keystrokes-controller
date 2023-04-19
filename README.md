# Keystrokes Controller

An executable app that makes a Twitch chat play videogames

## Description

This app creates a communication bridge between the Twitch chat and host keystrokes, allowing viewers to send commands to play on the host PC.

## Visuals

https://www.youtube.com/watch?v=nqbKPCvdPdc

## Requirements

We will be using Flutter to develop the desktop app and the targeted platform is Windows.

* Flutter SDK (https://docs.flutter.dev/get-started/install)
* An IDE that supports Flutter.
* A Windows PC to build the final app.

[More Information](https://docs.flutter.dev/development/platform-integration/desktop#requirements)

## Development

You must first clone the repository:
```
git clone https://github.com/ChanchisArmy/keystrokes-controller
```
(TODO)
## Roadmap

- [ ] Stable Twitch chat connection
- [ ] Control the host keystrokes
- [ ] Filter chat messages
- [ ] Create the Game Commands Manager
- [ ] Create the Queue Manager
- [ ] Get User Profile by Id (cache if it is possible)
- [ ] Interfaces

### Explanation

<img width="516" alt="image" src="https://user-images.githubusercontent.com/87735757/232982111-557e4dbe-f8c4-4a3d-ba6a-539748ebbef9.png">

**Stable Twitch chat connection**

A solid source of truth to listen the chat messages, including usernames and profile images.

**Control the host keystrokes**

Ensure that we will be able to control the keystrokes of a Windows PC through the app

**Filter chat messages**

Filter chat messages to recognize the commands and abstract them into a class/function

**Game Commands Manager**

Using the previous filter abstraction we can create a buffer of commands. Also we can consider creating a good abstraction to allow custom commands for a future phase (i.e chat sends "!car" and will be "X" for the host).

**Queue Manager**

Using the previous filter abstraction we can create specific commands (i.e !join, !leave ...) to register viewers for a game session

**Get User Profiles**

Using the first Twitch connection or another Twitch API to retrieve the images, this is optional and nice-to-have

**Interfaces**

Create a good interface to show buttons, buffer, profiles, and think how to manage queues...
## Authors

<table>
  <tbody>
    <tr>
      <td align="center">
        <a href="https://github.com/johannmorales">
            <img src="https://avatars2.githubusercontent.com/u/30033816?v=4?s=64" width="64px;" height="64px;" alt="johannmorales"/>
            <br />
            <sub><b>johannmorales</b></sub>
        </a>
      </td>
      <td align="center">
        <a href="https://github.com/ngxCoder">
            <img src="https://avatars2.githubusercontent.com/u/87735757?v=4?s=64" width="64px;" height="64px;" alt="ngxCoder"/>
            <br />
            <sub><b>ngxCoder</b></sub>
        </a>
      </td>
    </tr>
  </tbody>
</table>

## License

Copyright (c) ChanchisArmy Corporation. All rights reserved.

Licensed under the [MIT](LICENSE.txt) license.
