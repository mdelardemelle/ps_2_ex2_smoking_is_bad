# PS 2, exercise 2: Smoking is bad

Explore smoking and survival using the supplied dataset and Jupyter notebook.

## Setup

1. Install [Pixi](https://pixi.prefix.dev/latest/installation/).
2. Install VS Code and its Python and Jupyter extensions, if needed.
3. Clone this GitHub repository using its **Code** button or `git clone`.
4. Open the cloned repository folder in VS Code and open a new terminal there.
5. Install the project environment:

   ```sh
   pixi install -e smoke
   ```

Windows, Linux, Intel Macs, and Apple Silicon Macs are supported.
`pixi.toml` lists dependencies; `pixi.lock` records resolved package versions.

## Run the analysis

1. Open `smoking_is_bad.ipynb` and select **Select Kernel → Python Environments**.
2. Choose the interpreter in the cloned project's `smoke` environment:
   - Windows: `.pixi/envs/smoke/python.exe`
   - macOS/Linux: `.pixi/envs/smoke/bin/python`
3. If it is not listed, use **Python: Select Interpreter** from the command
   palette, then **Enter interpreter path** to select that interpreter.
4. Restart the notebook kernel and choose **Run All** to run from top to bottom.

Run with the repository folder as the working directory. The notebook reads
`data/smoking_data.csv`, which is included; no separate download is required.
Tables and charts are regenerated when cells run. Saved outputs are removed
before commits by the notebook cleanup hook.

## Contributing (optional for readers)

To activate the configured checks in your local clone, run from its terminal:

```sh
pixi run -e smoke pre-commit install
pixi run -e smoke pre-commit run --all-files
```

Hooks check formatting, code quality, and notebook cleanup. If a hook changes
files, review and stage them again before retrying the commit. Fix any remaining
reported errors. Local environments and editor/cache folders are ignored by Git.
