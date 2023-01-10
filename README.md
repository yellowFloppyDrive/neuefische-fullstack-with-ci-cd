# Steps

    # Install flyctl (https://fly.io/docs/hands-on/install-flyctl/)
    flyctl auth signup
    
    flyctl auth login
    flyctl auth token
    flyctl launch # fly.toml
    flyctl secrets set MONGO_URI='mongodb+srv://root:<password>@neuefische-cluster.hts873n.mongodb.net/neuefische-fullstack-demo?retryWrites=true&w=majority'
    flyctl secrets list
    # Setup GitHub Workflow
    https://fly.io/docs/app-guides/continuous-deployment-with-github-actions/
    git push
    
    flyctl deploy
    flyctl status
    flyctl open <optional-path>

## Gotchas:

- 256MB RAM - OOM Errors
- CPU 1x - Slow app
- 160GB Limit - May deduct money from your credit card
- Caching - May need to wait for the production app to update after deployment