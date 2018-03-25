####
Added support for more styles. Thank you Ottoville for this excellent work and Saxonce example.

# DOCX2HTML
This project is aim to create perfect conversion from docx fileformat to html with XSLT stylesheet.

Guidelines for project:
- Apperance is done with pure CSS3
- Maintain HTML5 sematics (Tricky one with nested lists)
- Do not lose information shipped in document.
- What you see in MS word, is what you see in HTML.

So far following features are supported:

- Pages (Sections, Page size, page orientation, forced page breaks, headers, footers)
- Paragraphs ( indents, paddings) 
- Lists (also nested list with right indents)
- Text styles: italic, underline, bold, color, font, background, kerning, alignment etc
- Images
- Tables
- Form items (textbox, checkbox)
- Block-level structured document tag
- Classes

The XSLT has been tested with Saxonce XSLT processor, but it should work with any XSLT 2.0 processor. In order to do conversion DOCX file need to be unzipped and docx2html.xsl stylesheet applied to document.xml file. Notice that current status of browsers native XSLT processors are lacking so many features that it is not possible to use them with this XSLT file.

See example of using Saxonce XSLT processor to [transform docx to html](https://github.com/ottoville/DOCX2HTML.XSL/wiki/Saxonce-example)

In case your DOCX file is not converted in way it should, please file an issue. Attach an example docx file into the issue.
