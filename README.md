# docs
Documentation of the PHP Telegram Bot



## Contributing to the Documentation

First thing first, clone the repo.

---

The Documentation is built upon `mkdocs`, in order to contribute, you can either:

:point_right: Directly modify the source with any text editor and do a Pull Request — suggested only if you know what you are doing.


:point_right: Install `mkdocs` **and** the extensions used in this Documentation to have a neat local live preview of the docs before submitting the Pull Request —  highly preferable.


### Setting up the local environment for `mkdocs`

Assuming you already have `pip` (and its dependencies) installed in your system, run the following in your shell:

```bash
$ pip install markdown mkdocs mkdocs-material pymdown-extensions

```
This will install:
* [markdown][1] — official PythonMarkdown extension
* [mkdocs][2] — the documentation builder
* [mkdocs-material][3] — the theme used in the docs
* [pymdown-extensions][4] — neat extensions to do a shitload of cool things :smile:


Once your environment is ready open a shell, head to the root directory were you cloned the repository and run `mkdocs serve`, the Documentation will now be live at the address `http://127.0.0.1:8000`:boom:

Every change you will make to the files will be instantly reflected to the live version. Once satisfied with the changes, commit and PR to the `develop` branch :smiley:


# To Do

###### **In** the Documentation
- Approve a proper TOC
    - Set up TOC
    - Start writing

###### **For** the Documentation
- So far, so good
  - [ ] this isn't the checkbox you were looking for :wave:

# Changelog
`0.0` - Let's do this!


[1]: https://pythonhosted.org/Markdown/
[2]: http://www.mkdocs.org/
[3]: https://github.com/squidfunk/mkdocs-material
[4]: https://github.com/facelessuser/pymdown-extensions
