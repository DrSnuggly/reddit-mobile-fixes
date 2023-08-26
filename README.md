# Reddit mobile fixes

This repository contains fixes for Reddit's mobile web experience, which is notoriously... not great.

## Features

- Make all media post content full-height, so no more chopped-off images in your feeds.
- Prevent inadvertently highlighting / selecting post content, while still allowing for copying / sharing media content directly.
- Hide the **Open App** button in the top menu bar.

## Usage

- Download and install an app that let's you set custom CSS for your web browser, e.g.:
  - iOS:
    - [**StopTheMadness**](https://apps.apple.com/us/app/stopthemadness-mobile/id1583082931)
    - [**Hyperweb**](https://apps.apple.com/us/app/hyperweb/id1581824571)
- Depending on the app, either:
  - Copy and paste the link to the `main.css` file: https://raw.githubusercontent.com/DrSnuggly/reddit-mobile-fixes/main/main.css
  - Copy the contents of the `main.css` file and paste it.

## Known issues

- Reddit sets a custom, static height for each post's content, and these tweaks remove these static
  heights from media posts to allow them to be fully displayed. There can be some vertical layout shifting
  as images are lazy-loaded on scroll — this is because, without the image, the post content height is
  zero, which then expands to fit as the content is loaded.
