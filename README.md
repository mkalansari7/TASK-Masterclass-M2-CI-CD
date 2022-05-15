# CI/CD

Time to dive into GitHub actions.

## Steps

1. Fork and clone [this repository](https://github.com/JoinCODED/TASK-Masterclass-M2-CI-CD).
2. Add a `.github/` folder in the root directory of the repository.
3. Add a `workflows/` folder inside the `.github/` folder.
4. Add a `main.yml` file inside of `workflows/`.
5. Setup python using https://github.com/actions/setup-python.
6. Add a pipeline to run the tests.
7. Add another pipeline to "Lint with Black", using `black --check .`.
8. Add another pipeline to "Lint with isort", using `isort --check-only .`.
9. Add another pipeline to "Lint with flake8", using `flake8 . --count --select=E9,F63,F7,F82 --show-source --statistics`.

## Bonus

Customize the pipeline to run on `push` and `pull_request`s only to the `main` branch.
