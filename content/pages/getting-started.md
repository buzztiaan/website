Title: Getting Started
Slug: getting-started
Summary: Getting started implementing the SpaceAPI for your hackerspace.
SortOrder: 20

If you want to implement the SpaceAPI for your hackerspace you need to do the
following:

 - [ ] Host the JSON file and a logo somewhere
 - [ ] Create a PR to TODO and add your space to the directory

# Hosting

The most minimal soution is to just [statically
host](https://en.wikipedia.org/wiki/Static_web_page) the JSON file, for example
on GitHub or GitLab or your own server.

A most minimal JSON file with just the required fields looks like that:

    :::json
    {
      "api": "0.13",
      "space": "$foospace",
      "logo": "https://foospace.example.com/logo.png",
      "url": "http://foospace.example.com",
      "location": {
        "lon": 1.337,
        "lat": 42.001
      },
      "state": {
        "open": null
      },
      "contact": {
        "email": "info@foospace.example.com",
      },
      "issue_report_channels": [
        "email"
      ]
    }


## Static Hosting On GitHub

TODO

## Static Hosting On GitLab

TODO

## Dynamic Hosting

If you want to support dynamic data in your API like sensor values, you need a
way to update the JSON data. While you could just change the values in your
statically hosted file, this may be impractical especially if you have values
that change a lot.

There are different implementation of servers which serve the SpaceAPI and
provide an API to update sensor values. See the [SpaceAPI
Community](https://github.com/spaceapi-community/) repositories or the [Apps
page](./apps.html) for some examples.
