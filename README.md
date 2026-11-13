# Sthira smoke-test site

Static landing page served by Caddy. Sign-ups post to the Google Apps Script collector set in `public/index.html` (`ENDPOINT`).

## Deploy to Railway

    npm i -g @railway/cli
    railway login
    railway init          # new project, e.g. "sthira-site"
    railway up            # builds the Dockerfile and deploys
    railway domain        # creates a public *.up.railway.app URL

To update the page later: replace `public/index.html`, then run `railway up` again.
