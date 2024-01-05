# MicroPython Library Template

A copier template to provide a skeleton for creating a standard MicroPython library.

# To use this template

## Install copier

```bash
> pipx install copier
> pipx inject copier copier-templates-extensions
```

## Create your instance of the template

```bash
> copier https://github.com/pi-mst/micropython_library_template example_output
```

Answer the prompts and your library skeleton will be generated into the `example_output` folder.

## To update

As the template evolves you can re-apply your template (non-destructively):

```bash
> copier update
```

## Output structure

```bash
📁 example_output
├── 📄 [library_name].py --------------- # Your Library file, if a single file library was selected
├── 📁 [library_name] ------------------ # Your library package, if a multi file library was selected
│   └── 📄 __init__.py ----------------- # Empty init ready to be filled
├── 📁 doc ----------------------------- # Documentation for this library
├── 📁 test ---------------------------- # Unit test code
│   └── 📄 test_my_new_library.py ------ # Unit test example
├── 📁 lib ----------------------------- # Dependencies (typically required to run examples or run tests)
├── 📁 examples ------------------------ # Example usage of this library
├── 📄 .gitignore ---------------------- # A standard .gitignore file
├── 📄 .gitlab-ci.yml ------------------ # Continuous Integration configuration for Gitlab
├── 📄 .copier-answers.yml ------------- # Answers are recorded here
└── 📄 pylintrc ------------------------ # PyLint configuration
```

## pre-commit

Pre-commit is used to perform a number of checks before code can be committed and pushed.
