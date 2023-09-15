# action-setup-meson
GH action that sets up the meson environment for workflows that need it.
This action installs meson cross files in docker image for a workflow job.
This may be a prerequisite step before `meson build` step.

## usage

```yaml
    - name: Setup meson
        uses: embedded-devops/action-setup-meson@main
        with:
          token: ${{ secrets.GHE_CI_TOKEN }}
          crossfiles_git: 'outpost/meson-cross-files'
          crossfiles_ref: 'main'
```
