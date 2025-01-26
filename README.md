# Moklet.org Link Shortener Redirects

## Repository Purpose
This repository contains Netlify configuration for the Moklet link shortener domain `go.moklet.org`, providing flexible URL redirection.

## Netlify Configuration
The `netlify.toml` file defines a comprehensive set of redirect rules to route incoming requests to their appropriate destinations.

### Redirect Rules

#### Main Domain Redirect
- Redirects root path `/` to the main Moklet.org website
- HTTP Status: 301 (Permanent Redirect)

#### Specific Path Redirects
1. `/f/*` → Redirects form-related paths
2. `/twbn/*` → Redirects Twibbon-related paths
6. Catch-all rule: Redirect any paths to the link shortening handler on the main website

### Redirect Behavior
- Most redirects use 301 (Permanent Redirect) status
- Some paths use 200 status with `force = true` for specific resources (rewrite)

## Deployment
Deployed and managed using Netlify for efficient link redirection.

[![Netlify Status](https://api.netlify.com/api/v1/badges/e577be17-21e7-45d3-8e02-36437eb157c0/deploy-status)](https://www.netlify.com)

## Technologies
- Netlify

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

## Contributions
Feel free to submit pull requests if you need to modify or add new redirect rules.
