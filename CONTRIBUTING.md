# Contributing to ActixLab

## Branching

Always create a branch from `main` before starting work:

```bash
git checkout main
git pull origin main
git checkout -b yourname/track-name
```

Examples:

- `frank/01-hello-actix`
- `mike/02-crud-api`
- `frank/03-auth-jwt`

## Track folders

Each folder under `rust-backend-lab/` is a track.

Examples:

- `rust-backend-lab/01-hello-actix/`
- `rust-backend-lab/02-crud-api/`
- `rust-backend-lab/03-auth-jwt/`

## Working in the same track without conflict

If two people want to explore the same track independently, create separate subfolders inside the track:

```text
rust-backend-lab/02-crud-api/
  frank/
  mike/
```

or separate Rust crates with clear names:

```text
rust-backend-lab/02-crud-api/
  frank-crud-api/
  mike-crud-api/
```

If two people are collaborating on one shared implementation in the same track, split ownership by files/modules and avoid editing the same file at the same time.

## Commits and pushes

Commit often with small messages:

```bash
git add .
git commit -m "feat: add todo create endpoint"
git push -u origin yourname/track-name
```

Then open a pull request into `main`.

## Rules

- Do not commit `.env` files or secrets.
- Do not work directly on `main`.
- Pull latest changes before new work.
- Prefer one track per branch.
