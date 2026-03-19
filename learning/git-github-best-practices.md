# Git and GitHub Best Practices

These notes are for Odin Project practice. Keep them nearby while you work so Git feels like a habit, not a mystery.

## The big idea

- Use Git to save meaningful checkpoints.
- Use branches for new work.
- Keep commits small and easy to understand.
- Push often so your work is backed up.
- Use GitHub to share work, review changes, and collaborate.

## Safe workflow

1. Start from a clean state.
   - Run `git status` before you begin.
   - If something unexpected is already changed, pause and understand it first.
2. Make one focused change at a time.
   - Small changes are easier to test, explain, and fix.
3. Check your work before committing.
   - Use `git diff` to review what changed.
   - Run tests or reload the app if your project has them.
4. Commit when the change is complete.
   - Save a checkpoint before moving on.
5. Push your branch to GitHub.
   - This protects your work and makes collaboration easier.

## Branching habits

- Use a new branch for each task or feature.
- Name branches clearly.
  - Good: `feature/navbar`, `fix/login-error`, `docs/readme-update`
  - Less clear: `stuff`, `new-branch`, `test`
- Stay on `main` or `master` only when you are doing setup or very small solo changes.
- If your work gets messy, create a fresh commit checkpoint before continuing.

## Commit habits

- Write commits like short answers to the question "What did I do?"
- Use the imperative mood:
  - `Add contact form validation`
  - `Fix broken login redirect`
  - `Update README examples`
- Keep each commit focused on one idea.
- Avoid commits like:
  - `stuff`
  - `changes`
  - `final`

## Good GitHub habits

- Push branches regularly.
- Open pull requests when you want feedback or need to merge.
- Use PR descriptions to explain:
  - what changed
  - why it changed
  - how you tested it
- Review your own PR before asking others to review it.
- Leave clear comments if a part of the code needs special attention.

## When something goes wrong

- If you changed the wrong file, check `git diff` before you panic.
- If you forgot a file, add it with `git add`.
- If a commit message is bad, make the next commit better instead of stressing about perfection.
- If you are unsure, stop and inspect with `git status`, `git diff`, and `git log --oneline`.

## Beginner rules to remember

- Never run commands you do not understand just because they are on the internet.
- Commit before big experiments.
- Push before switching computers or stopping for the day.
- Read the output Git gives you. It usually tells you what to do next.

## Odin-friendly mindset

- Treat Git practice like coding practice.
- Expect to make mistakes.
- Learn from the output, not from guessing.
- Use the repo as a safe place to build confidence.
