# Trigger a ToolForge deployment

This action provides a helper interface executing a deployment on ToolForge

Example usage:

```
  deploy:
    runs-on: ubuntu-latest
    needs: [release]
    steps:
      - uses: cluebotng/ci-toolforge-deploy@main
        with:
          tool: very-cool-tool
          token: ${{ secrets.CI_DEPLOY_TOKEN }}
```
