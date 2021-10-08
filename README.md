# Hermite-doc
 
The HTML entrance to the doc is at `build/html/index.html`.

To modify and re-complie the doc, please install sphinx and readthedocs theme first:

```bash
pip install sphinx
pip install sphinx_rtd_theme
```

The documentation of Hermite-FEP is written in a single file `source/main.rst`, you can directedly edit the `.rst` (reStructureText) file if you are familiar with the grammar, or edit `source/main.md` (the markdown file) and transform it into `.rst` file with `pandoc`:

```bash
pandoc main.md -o main.rst
```

In the root directory of the repo, type

```
make html
```

will re-compile the doc and update `build/*` files.