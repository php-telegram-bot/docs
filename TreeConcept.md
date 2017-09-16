- Home: Brief introduction to the framework

- Let's Play!: (section for "newbies")

  - Introduction: Scope of this section of the docs, knowledge prerequisites - opposed to what is taken for granted in the Core section

  - Environment: Must have stuff and its usage plus suggested software
    - Vagrant setup and usage
    - Composer setup and usage
    - MySQL setup and first initialization with the structure.sql
    - Git clone the example-bot and brief overview of the files and the structure of the framework

  - Registering your bot: Botfather, its usage and options

  - First steps with the code:
    - getUpdates: analysis of the file, and what each part does, initial configuration with bot credentials and mysql database for local use in vagrant
    - Overview of the example commands: self explanatory
    - Creating a custom command: self explanatory
      - Testing the bot: experimenting with the example commands and custom commands locally
    - Webhook: what it is and how it works
      - set.php
        - unset.php
      - hook.php
      - manager.php
      - notes on self signed certificates

- Core
  - Overview of the methods and the classes available
    - Types
    - Methods
    - Inline Query
  - Utilities
    - MySQL
    - Channel integration
    - Botan.io
  - Commands
    - Predefined commands
    - Custom commands
    - Commands configuration
    - Admin Commands
      - Set admins
      - Channel Administration
    - Upload and Download paths and usage of the calls to up\down stuff
    - Logging
