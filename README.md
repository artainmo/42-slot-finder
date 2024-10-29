# 42-slot-finder

Bot that verifies if correction slots are to be found on a specific 42 school project.

This project I initially made with [artygo8](https://github.com/artygo8) in this [repository](https://github.com/artygo8/FindSlots-42), I re-uploaded it on my profile for [obsidian transfer](https://github.com/artainmo/github_to_obsidian).

## Usage

  Set environment

  ```
  make env
  ```

  Launch

  ```
  make
  ```

  Once launched, you will get the instructions.

## Explained

This program uses selenium to launch a Firefox browser.

It will then refresh the page to find correction slots every 42 seconds and notify with a sound and eventually email when there is an available slot on the page.

It also shows progress in the terminal like so : `.....!.` where `.` means that there are no available slots and `!` means the bot found a slot on the page.

## Current requirements

 - **python selenium**      `# main part, actual bot`
 - **python time**          `# waiting`
 - **python chime**         `# for the sound notifications`
 - **python signal**        `# for proper interruption handling`
 - **python dotenv**        `# to keep track of email credentials in .env`
 - **Firefox**              `# browser used by the bot`
 - **geckodriver**          `# needed by Selenium`
