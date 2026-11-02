# PS 2, exercise 2: Smoking is bad

Install [Pixi](https://pixi.prefix.dev/latest/installation/), clone this repo,
and open its folder in VS Code with the Python and Jupyter extensions.

From the repository folder:

```sh
pixi install -e smoke
```

Open `smoking_is_bad.ipynb`, select the project's `smoke` Python kernel,
and choose **Run All**. Keep the repository folder as the working directory.
Data is included in `data/smoking_data.csv`.

Kernel path: `.pixi/envs/smoke/python.exe` on Windows;
`.pixi/envs/smoke/bin/python` on macOS/Linux.

Before contributing:

```sh
pixi run -e smoke pre-commit install
pixi run -e smoke pre-commit run --all-files
```
