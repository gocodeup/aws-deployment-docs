# Updating Server Repositories

This document provides instructions on how to pull changes from your Github repository onto your production server. If you have not completed the deployment process, please visit the [deployment guide](../docs/1.step-one.md).

1. Log into your server
    - `ssh -i .ssh/codeup-aws.pem ubuntu@IP_ADDRESS`
2. `cd` into your project repository directory
3. `git pull origin main`
4. `pm2 reload all`

> ***It is recommended to run `pm2 log` after you have restarted the server so you can determine if there are any breaking changes.***