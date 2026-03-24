1. Install PyPDF2

```python
from PyPDF2 import PdfWriter

writer = PdfWriter()

# add a blank page
writer.add_blank_page(width=300, height=300)

# inject javascript
writer.add_js("app.alert('PDF JS Executed!');")

with open('js_in.pdf', 'wb') as f:
  writer.write(f)
```
