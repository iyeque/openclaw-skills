# PDF Reader examples

## Extract a bounded section

```bash
python3 skills/pdf-reader/reader.py extract report.pdf --max_pages 10
```

## Find evidence with page numbers

```bash
python3 skills/pdf-reader/reader.py search report.pdf --query "revenue" --max_pages 50
```

Results include matching pages, counts, and bounded context. Processing stops at 500 pages by default.
