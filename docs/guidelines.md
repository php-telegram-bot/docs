# Guidelines to contribute

## Markdown
!!! important
    I take for granted tat you know the basic implementation of Markdown already, here there will be the list of extensions used.
    You can check their respective reference following the commented links.


    ??? bug "Extensions list..."

        ```
        markdown_extensions:
            - smarty

            - admonition

            #https://pythonhosted.org/Markdown/extensions/abbreviations.html
            - abbr

            #https://pythonhosted.org/Markdown/extensions/definition_lists.html
            - def_list

            #https://pythonhosted.org/Markdown/extensions/footnotes.html
            - footnotes


            #https://facelessuser.github.io/pymdown-extensions/
            - pymdownx.emoji:
                emoji_generator: !!python/name:pymdownx.emoji.to_png
            - pymdownx.details
            - pymdownx.superfences
            - pymdownx.caret
            - pymdownx.mark
            - pymdownx.escapeall
            - pymdownx.snippets:
                base_path: 'extra'
            - pymdownx.highlight:
                css_class: codehilite
                extend_pygments_lang:
                  - name: php
                    lang: php
                    options:
                      startinline: true
        ```

!!! todo
    Further infos to add
