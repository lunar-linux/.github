# lunar-linux/.github

Organization-wide files for [Lunar Linux](https://github.com/lunar-linux) on GitHub.

- [`profile/README.md`](profile/README.md): the introduction shown on the organization's page.
- [`.github/workflows/`](.github/workflows/): reusable workflows for the organization's repositories.

## Reusable workflows

| Workflow | Used by | What it does |
| --- | --- | --- |
| [`notify-website.yml`](.github/workflows/notify-website.yml) | moonbase repositories, on push to `master` | Tells `lunar-web` that modules changed, so the homepage's arrivals board refreshes |

Call them by tag, for example `uses: lunar-linux/.github/.github/workflows/notify-website.yml@v1`.
Compatible changes move the `v1` tag (`git tag -f v1 && git push -f origin v1`); a breaking change
gets a new major tag.

## License

MIT
