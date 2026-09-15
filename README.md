# FSU Professor Finder

A lightweight tool for Florida State University students to look up professors and RateMyProfessors ratings by course code — no account needed, no app to install.

## What it does

Enter any FSU course code (e.g. `MAC1105`, `PSY2012`) and the tool searches for professors currently teaching that course at FSU, pulling ratings, difficulty scores, student tags, and tips from RateMyProfessors.

You can add as many courses as you like, search them all at once, and remove any you don't need.

## How to use it

1. Open the link shared with you
2. Enter the access code
3. Type a course code into the box and click **Add Course**
4. Click **Search** on any card, or **Search All** to run them together

## Tech notes

- The front end is a single HTML file hosted on GitHub Pages
- Course searches are handled by a Cloudflare Worker that calls the Anthropic API with live web search — no data is stored
- The Anthropic API key lives only in the Worker and is never exposed to the browser

## Accuracy

Results are sourced live from the web at the time of your search. Always cross-check professor availability against the [FSU course schedule](https://registrar.fsu.edu) and verify ratings directly on [RateMyProfessors.com](https://www.ratemyprofessors.com).
