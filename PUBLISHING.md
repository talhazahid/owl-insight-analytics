# Publishing This Public Repo

## Recommended setup

Do not publish the private OwlInsight app repository.

Create a second GitHub repository instead, for example:

- `owlinsight`
- `owlinsight-public`
- `owlinsight-product`

Then copy the contents of this folder into that new repository.

## What to include

- `README.md`
- `PRODUCT.md`
- `LICENSE.md`
- `assets/`

## What not to include

- app source code
- `.env`
- Prisma schema tied to live production
- auth config
- billing logic
- deployment scripts
- internal admin code

## Suggested first commit

Use a commit message like:

```text
Public product repo for OwlInsight
```

## After publishing

1. Add the live site URL to the GitHub repo description.
2. Pin the repo on your GitHub profile.
3. Add one issue template for feature requests if you want public feedback.
4. Replace the placeholder SVG previews with real screenshots later.
5. Keep the README updated when big features ship.

## Optional next step

Run the export helper from the private repo root:

```powershell
.\scripts\export-public-repo.ps1
```

That creates a clean folder with just the public repo files, ready to push.
