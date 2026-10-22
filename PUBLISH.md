# Publish to GitHub Pages (needs a working `gh` login)

    gh auth login            # device flow in the browser, once
    cd ~/Code/tokentalk-site
    gh repo create tokentalk-site --public --source=. --push
    gh api -X POST repos/babosx/tokentalk-site/pages -f 'source[branch]=master' -f 'source[path]=/'

Privacy URL for the Play listing: https://babosx.github.io/tokentalk-site/privacy.html
