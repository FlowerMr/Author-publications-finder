
# 📚 Author Publications Finder

A Python tool to search and aggregate academic publications (articles and books) for a given author from multiple sources: OpenAlex, CrossRef, and arXiv. It includes open access information and PDF links where available.

This project showcases my skills in API integration, data aggregation, duplicate removal, and pandas DataFrame manipulation. Built as part of my exploration in academic research tools, it reflects my interest in AI, data science, and research automation, aligning with my pursuit of PhD opportunities.

## Features
- Fetches publications from OpenAlex, CrossRef, and arXiv.
- Normalizes titles to remove duplicates.
- Sorts results by publication year (descending).
- Outputs a clean DataFrame with details: title, authors, year, work type, open access status, PDF URL, source, URL, and DOI.

## Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/FlowerMr/Author-publications-finder.git
   cd Author-publications-finder
   ```
2. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
   Required packages: `requests`, `pandas`, `arxiv`, `rapidfuzz`

## Usage
Run the script and enter the author's name when prompted:
```bash
python author_finder.py
```
Example output for "Yann LeCun":
```
Found 45 works for author 'Yann LeCun':

| title | authors | year | work_type | open_access | pdf_url | source | url | doi |
|-------|---------|------|-----------|-------------|---------|--------|-----|-----|
| ... (sample data) ...
```

## How It Works
- **OpenAlex**: Searches for author ID and fetches top-cited works.
- **CrossRef**: Queries by author name for DOIs and metadata.
- **arXiv**: Retrieves preprints with open access PDFs.
- Aggregates results, removes duplicates based on normalized titles, and sorts by year.

## Limitations
- May miss works if author name variants exist (e.g., try full name or initials).
- API rate limits apply; use responsibly.
- Open access info from CrossRef is limited (assumed False).

## Contributing
Contributions are welcome! Feel free to fork, submit pull requests, or report issues.


## Contact
Author: [Reza Golkar]  
LinkedIn: [https://www.linkedin.com/in/rezagolkar/]  
GitHub: [FlowerMr](https://github.com/FlowerMr)  
