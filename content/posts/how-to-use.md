+++
title = 'How to Use My REST API'
date = 2025-11-30T21:49:07-05:00
draft = false
tags= ["tutorial", "web-development"]
categories= ["programming"]
description= "Post on how to operate my REST API"
author= "Kady Schawe"
readingTime= "5 min"
+++

# My Music-API

## Introduction

In this post, I will cover what my REST API does and how to use it.

## Prerequisites

 Before reading this post, I would advice to look through my music-api document in projects.

### What does my API solve?

I built my REST API to keep and store information regarding a music related database.
Through this REST API, one is able to keep track of users, employees, playlists, top songs, top artists, and more.

With an increase in the amount of users and employees, the information regarding each user and artist is neatly organized and easily retrieved.

### How to use it

For each of my API's can perform all CRUD operations.

First you can clone the repository

```bash
git clone https://github.com/schawek2/music-api.git
cd music-api
```

Then you can start it with docker either by using the setup.sh or doing:
```bash
docker-compose up -d
```

Once this is done, the RESTful API is now available on http://localhost:8080

## Links

 - **GitHub Repository**: [github.com/schawek2/music-api](https://github.com/schawek2/music-api)

