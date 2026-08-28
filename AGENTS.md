# Repository Guidelines

## Project Structure & Module Organization

This repository collects Quanser academic documentation and examples:

- `0_libraries/` contains shared MATLAB, Python, QLabs, and real-time model libraries.
- `1_setup/` contains setup scripts, Python requirements, and product setup guides.
- `2_quick_start_guides/`, `3_user_manuals/`, and `4_concept_reviews/` contain learning and reference material.
- `5_research/`, `6_teaching/`, `7_outreach/`, and `8_user_content/` contain examples, labs, demonstrations, and contributions.
- `docs/` contains repository-level setup documentation; `README.md` is the entry point.

Keep new examples in the most specific product/topic directory, and keep supporting images or models beside the content that uses them.

## Build, Test, and Development Commands

There is no repository-wide build system. From the repository root on Windows:

```powershell
.\1_setup\step_1_check_requirements.bat
py -3.13 -m venv .venv
.\.venv\Scripts\python.exe -m pip install -r .\1_setup\requirements.txt
```

Run `configure_python.bat` and/or `configure_matlab.bat` only for machine setup; they modify environment configuration. For a Python smoke test, run the relevant example (for example, `py path\to\example.py`) or use `py -m compileall path\to\changed\python`. Open and run changed `.slx`/`.mdl` models in the supported MATLAB/Simulink, QUARC, or QLabs environment.

## Coding Style & Naming Conventions

Use four spaces in Python and preserve the existing MATLAB style. Follow nearby naming conventions: lowercase `snake_case` for Python scripts, descriptive product-prefixed model names, and numbered directories for ordered guides. Keep filenames and links consistent with existing casing and spaces. No repository-wide formatter or linter is configured.

## Testing Guidelines

Validation is targeted rather than framework-based. Run the affected Python example or hardware/virtual-device test, and perform a MATLAB/Simulink smoke run for changed models. Record language/runtime versions and whether hardware, QUARC, or QLabs was used. Do not treat generated `__pycache__/`, `slprj/`, `.slxc`, or downloaded model files as source changes unless intentionally adding a required asset.

## Commit & Pull Request Guidelines

Recent commits use concise, descriptive, path-specific subjects such as `Update configure_python.bat ...` or `Fixed filename issue`. Keep commits focused and mention the product or directory affected. Pull requests should explain the user-facing change, link the relevant issue, list validation (including software versions and hardware/virtual context), and include screenshots or logs for documentation or visual changes. Update `changelog.txt` for releases or materially changed published resources.

## Safety & Configuration Tips

Follow product manuals before running hardware examples. Prefer virtual validation where available, do not commit credentials or machine-specific paths, and review `git status` before committing to exclude setup logs and generated artifacts.
