# 22B Terminal for Gradient Descent in Mothership

This is a simple, read-only, implementation of terminal 22B in the Mothership adventure, Gradient Descent (https://www.tuesdayknightgames.com/products/gradient-descent).

This entire project has been forked from the ttrpg email terminal created by @jacksonbenete, https://github.com/jacksonbenete/email_terminal. If you are interested in creating your own terminal experience, I highly recommend checking out the original repository!

If you are a Warden, see spoiler-inclusive notes in the WARDEN_README.md file.

You can fork the project and change the code for your own configurations, like terminal name (or sector/station/node if sci-fi), image and messages.

The database is a simple set of JSON files.

You can host it on Github Pages for a free and fast experience and can share the link for your friends and players to use.

<!-- To update this Table Of Contents:
    markdown-toc -i README.md
-->

<!-- toc -->

- [Quick launch](#quick-launch)
- [Login, Mail & Read Functions](#login-mail--read-functions)
- [Other Functions](#other-functions)
- [How to Install](#how-to-install)
- [Acknowledgement](#acknowledgement)

<!-- tocstop -->

## Quick launch

The following command will launch a server at localhost once you've cloned the repo.

```node
python -m http.server
```

Alternatively, the terminal may be available online at https://cormac0.github.io/mosh_terminal/. This isn't garunteed though, since this project is a work-in-progress.

## Login, Mail & Read Functions

The main functions are the `mail` and `read` terminal operations.

Once you `login`, you can call the `mail` function to list the user emails, and you can `read` the mails you want by entering the index code (the correspondent number, letter, or string). 

As this is a simple terminal emulation, you can't delete mails or mark as read. We may be able to work it out in the future, but those basic functions are enough to send some cool mysterious mails to your players' agents, or emulate a character hacking into a company to investigate a clue or something.

---

To login you need to enter `user:password`

![How to login.](docs/login1.png)
---

Note the change in the terminal username

![Note the change in the terminal username.](docs/login2.png)
---

How to list and read mails

![Mail and Read functions.](docs/mail_n_read.png)

## Other Functions

You can try `help` to see a list of other functions available. The `clear` function may be a useful one.

## How to Install

As I've said, you can use Github Pages to do that for you.
If you're not used to Github, first create a Github user by registering in [Github](github.com), so you can "fork" the project to your account by accessing the project page [email_terminal](github.com/jacksonbenete/email_terminal) and by clicking in the "fork" button.

![How to Fork a project.](docs/fork1.png)

Note that those two in red are the only two steps you need to take to get your terminal up and running. You need to click the Fork button, and after a few seconds, the project will be there as one of your own repositories, and then you click the Settings button.

In the settings page, scroll down to the Github Pages section and select the source as the master branch. 

![Github Pages on Settings.](docs/fork2.png)

After a few seconds, you will be able to access your terminal at username.github.io/email_terminal (i.e. jacksonbenete.github.io/email_terminal).

Note that you can create multiple repositories and name those repositories in the Settings for each of your game tables. That way you can have one terminal ready for each setting (or for each organization your players will hack into), ex: 
- username.github.io/spacestationX22
- username.github.io/PenTexCorp
- etc

You just need to share the correct link with your players and wait for them to read the clues and investigate.

## Acknowledgement
- Inspiration taken from the incredible Gradient Descent terminal by @PimPee, https://github.com/PimPee/GradientDescentTerminal, with flavor text from @iason-pap, https://github.com/iason-pap/gradient-descent-terminal-files.
- Forked and inspired by the ttrpg email terminal by @jacksonbenete, https://github.com/jacksonbenete/email_terminal.
