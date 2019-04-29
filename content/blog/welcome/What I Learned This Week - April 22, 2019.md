---
title: What I Learned This Week - April 22, 2019
date: "2019-04-29T16:07:56+00:00"
description: "What I learned deploying my first full stack app."
---

## What I Did This Week

This week, I worked on deploying my Flashcards app to an old domain that I had from another project, mountfluency.com. Prior to this, I had no experience deploying a back end API, nor have I deployed a full stack app.

I deployed my static files to Netlify a few weeks ago, which was much easier than tackling the back end. [This](https://www.youtube.com/watch?v=kR06NoSzAXY) tutorial by Jason Lengstorf was extremely useful ([written link](https://lengstorf.com/code/deploy-nodejs-ssl-digitalocean/), if you prefer).

## What I Learned

In deploying my API and database, _here’s what I learned this week:_

- Creating a [DigitalOcean](digitalocean.com) droplet with a non-root user, and setting up SSH to connect to the server via my terminal.

- How to point my Google Domain’s name servers to [Netlify](netlify.com), and from Netlify, creating an A record that points api.mountfluency.com to my DigitalOcean droplet.

- Encrypting my site with a certificate from [LetsEncrypt](https://letsencrypt.org/) (including using a Diffie-Hellman Key Exchange).

- How to configure NGINX as a reverse proxy for my API.

- How to use Express’s CORS module to allow my front end to make requests to my back end.

- Using PostgreSQL to create a database for my application via psql on the command line (and using the ALTER command to fix mistakes I made setting up certain columns).

- Using ENV variables to configure “production” and “development” modes. In production, the API connects with my production database, and in development, it connects to the database served locally on my computer.

- Using PM2 to keep my app running full-time, and using pm2 monit and pm2 logs to debug deployment issues.

## My Plan for Next Week

- Fix form validation bugs that break the back end.

- Start using the site to learn German!

- Redesign the About page.

- Make a sketch for a new website idea.
