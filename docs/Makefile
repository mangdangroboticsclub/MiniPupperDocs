# Minimal makefile for Sphinx documentation
#

# You can set these variables from the command line, and also
# from the environment for the first two.
SPHINXOPTS    ?=
SPHINXBUILD   ?= sphinx-build
SOURCEDIR     = .
BUILDDIR      = _build

# Put it first so that "make" without argument is like "make help".
help:
	@$(SPHINXBUILD) -M help "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)

rtd:
	python3 -m sphinx -T -E -b html -d "$(BUILDDIR)/doctrees" -D language=en "$(SOURCEDIR)" "$(BUILDDIR)/html" $(SPHINXOPTS) $(O)

rtd-ja:
	python3 -m sphinx -T -E -b html -d "$(BUILDDIR)/doctrees" -D language=ja "$(SOURCEDIR)" "$(BUILDDIR)/html" $(SPHINXOPTS) $(O)

rtd-all:
	python3 -m sphinx -T -E -b html -d "$(BUILDDIR)/doctrees/en" -D language=en "$(SOURCEDIR)" "$(BUILDDIR)/html/en" $(SPHINXOPTS) $(O)
	python3 -m sphinx -T -E -b html -d "$(BUILDDIR)/doctrees/ja" -D language=ja "$(SOURCEDIR)" "$(BUILDDIR)/html/ja" $(SPHINXOPTS) $(O)

intl-ja:
	sphinx-build -b gettext "$(SOURCEDIR)" "$(BUILDDIR)/gettext" $(O)
	sphinx-intl update -p "$(BUILDDIR)/gettext" -l ja $(O)

.PHONY: help Makefile rtd rtd-ja rtd-all intl-ja

# Catch-all target: route all unknown targets to Sphinx using the new
# "make mode" option.  $(O) is meant as a shortcut for $(SPHINXOPTS).
%: Makefile
	@$(SPHINXBUILD) -M $@ "$(SOURCEDIR)" "$(BUILDDIR)" $(SPHINXOPTS) $(O)
