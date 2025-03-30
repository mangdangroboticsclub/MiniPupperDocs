# Mini Pupper - ROS, OpenCV, Open-source, Pi Robot Dog
Mini Pupper will make robotics easier for schools, homeschool families, enthusiasts and beyond.

「Mini Pupperは、学校、家庭学習、愛好家、そしてそれ以外の人々にも、ロボット工学をより身近なものにしてくれることでしょう」 by MangDang

* [English](https://mangdangroboticsclub.github.io/MiniPupperDocs/en/)
* [日本語](https://mangdangroboticsclub.github.io/MiniPupperDocs/ja/)

## Sphinx Document Buildling

This document is written in [reStructuredText](https://www.sphinx-doc.org/en/master/usage/restructuredtext/index.html), designed following Sphinx practice, and hosted on [Read the Docs](https://minipupperdocs.readthedocs.io/en/latest/) and [GitHub Pages](https://mangdangroboticsclub.github.io/MiniPupperDocs/en/).

This document can also be built locally, where the following environment setup would be initially required:

```bash
# Setup Poetry (Python package and project manager)
pip install poetry
```

```bash
# Install the Python packages
poetry install
# Activate virtual env
poetry shell
```

Then the following commands can build a result of HTML documents to view in browsers directly:
```bash
cd ./docs
make rtd
# The details of rtd-ja refers to _Sphinx Document Internationalization_ below.
# make rtd-ja
```

Now the build result files can be opened from `docs/_build/html`.

## Sphinx Document Internationalization

```
# Make Sphinx-generated messages (Japanese version is prebuilt here)
make intl-ja

# Preview Sphinx-generated messages as HTML
make rtd-ja
```
