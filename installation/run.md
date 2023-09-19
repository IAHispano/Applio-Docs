# Run Applio

+++ Script
Open the file `go-applio.bat` and choose the appropriate option according to your case!
+++ Manually
**NVDIA:**

```bash
python infer-web.py --pycmd python --port 7897
```

**AMD or Intel:**

```bash
python infer-web.py --pycmd python --port 5000 --dml
```

+++