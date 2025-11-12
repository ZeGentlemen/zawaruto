---
{"dg-publish":true,"permalink":"/fun/linux/pdf-to-md-py/","tags":["guide"],"noteIcon":"","created":"2025-11-06T10:32:10.480+05:00","updated":"2025-11-12T14:26:37.082+05:00"}
---

- [ ] make a script that does it for you

# Create the virtual environment so pip is allowed to run
```
cd ~/pdf_to_md
python -m venv venv
source venv/bin/activate
pip install pymupdf
python pdf_to_md.py
```

>*note pipx doesn't work in this context because it's isolated and pdf_to_md.py is just a file not available on pipx

# Stopping
```
deactivate
```
# Reusing it afterwards
```
cd ~/pdf_to_md
source venv/bin/activate
python pdf_to_md.py
```