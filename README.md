# python-docx

_python-docx_ is a Python library for reading, creating, and updating Microsoft Word 2007+ (.docx) files.

This fork has been updated with [these](https://github.com/python-openxml/python-docx/compare/master...jdthorpe:python-docx:master) changes to make `python-docx` compatible with [`Simplify-Docx`](https://github.com/microsoft/Simplify-Docx).

## Installation

Install directly from git::

```
pip install git+https://github.com/dalmia/python-docx.git
```

Or you can install locally after cloning the repository:

```
git clone git@github.com:dalmia/python-docx.git
cd python-docx
pip install .
```

## Example

```python
>>> from docx import Document

>>> document = Document()
>>> document.add_paragraph("It was a dark and stormy night.")
<docx.text.paragraph.Paragraph object at 0x10f19e760>
>>> document.save("dark-and-stormy.docx")

>>> document = Document("dark-and-stormy.docx")
>>> document.paragraphs[0].text
'It was a dark and stormy night.'
```

More information is available in the [python-docx documentation](https://python-docx.readthedocs.org/en/latest/)
