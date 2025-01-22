# AI Engineering template (with uv)

----------------------------------------------------------------------------------------

A template repo for AI Engineering projects (using ``python``) and ``uv``. This
template is like our original AI Engineering [template](https://github.com/VectorInstitute/aieng-template),
but unlike in that template which uses poetry, here we use uv for dependency
management (as well as packaging and publishing).

## 🧑🏿‍💻 Developing

### Installing dependencies

The development environment can be set up using
[uv](https://github.com/astral-sh/uv?tab=readme-ov-file#installation). Hence, make sure it is
installed and then run:

```bash
uv sync
source .venv/bin/activate
```

In order to install dependencies for testing (codestyle, unit tests, integration tests),
run:

```bash
uv sync --dev
source .venv/bin/activate
```

If you're coming from `poetry` then you'll notice that the virtual environment
is actually stored in the project root folder and is by default named as `.venv`.
The other important note is that while `poetry` uses a "flat" layout of the project,
`uv` opts for the the "src" layout. (For more info, see [here](https://packaging.python.org/en/latest/discussions/src-layout-vs-flat-layout/))
