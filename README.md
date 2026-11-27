# auto-commit

A small GitHub Actions workflow that makes one automated commit every day.

## How it works

- `.github/workflows/autocommit.yml` runs on a schedule (daily at 16:00 UTC).
- Each run updates the `LAST_UPDATED` file with the current date and pushes a commit.
- It can also be started manually from the **Actions** tab with **Run workflow**.

## Set it up yourself

1. Create your own repo (do not fork).
2. Copy `.github/workflows/autocommit.yml` into it.
3. Change the `user.name` and `user.email` lines in the workflow to your own.
4. Change the cron line to your preferred time (cron uses UTC).

## Note

These commits are automated and do not represent manual work.
