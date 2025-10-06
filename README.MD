# Turkish Ministry of Education 10th Grade Curriculum Repository

## Overview

This repository contains Turkish Ministry of Education (MEB) 10th grade textbooks and solution guides in structured formats. Materials are organized into two categories: raw textbook pages extracted from official publications and solution guides scraped from educational websites with accompanying images.

## Subjects

The repository covers seven subjects from the 10th grade curriculum:

| Subject          | Turkish Name      | System Folder Name  |
| ---------------- | ----------------- | ------------------- |
| Geography        | Coğrafya          | `cografya`          |
| Literature       | Edebiyat          | `edebiyat`          |
| Physics          | Fizik             | `fizik`             |
| English Workbook | İngilizce Çalışma | `ingilizce_calisma` |
| English Textbook | İngilizce Ders    | `ingilizce_ders`    |
| Chemistry        | Kimya             | `kimya`             |
| Mathematics      | Matematik         | `matematik`         |

## Structure

```
├── raw/
│   ├── cografya/
│   │   ├── 1.pdf
│   │   └── 2.pdf
│   ├── edebiyat/
│   ├── fizik/
│   ├── ingilizce_calisma/
│   ├── ingilizce_ders/
│   ├── kimya/
│   └── matematik/
│
└── solutions/
    ├── cografya/
    │   ├── 1/
    │   │   ├── page.md
    │   │   ├── image_1.webp
    │   │   └── image_2.jpg
    │   └── 2/
    │       ├── page.md
    │       ├── image_1.webp
    │       └── image_2.jpg
    ├── edebiyat/
    ├── fizik/
    ├── ingilizce_calisma/
    ├── ingilizce_ders/
    ├── kimya/
    └── matematik/
```

## Data Format

### Raw Textbooks

**Location:** `/raw/{subject_name}/`  
**Format:** Individual PDF pages (1.pdf, 2.pdf, 3.pdf, ...)  
**Source:** Official MEB/EBA platforms and affiliated educational websites  
**Processing:** Programmatically split from complete textbooks into single-page PDFs

### Solution Guides

**Location:** `/solutions/{subject_name}/{page_number}/`  
**Format:** Markdown files with embedded images  
**Contents:**

- `page.md` - Solution content
- `image_*.webp` or `image_*.jpg` - Solution images referenced via Markdown syntax

**Source:** Generally available educational answer key websites  
**Processing:** Web-scraped content with automated filtering, formatting, and image extraction

## Data Collection Methodology

### Textbook Acquisition

Textbooks were downloaded from official MEB/EBA platforms and affiliated educational websites, then programmatically split into individual pages while maintaining original PDF quality.

### Solution Guide Extraction

Solutions were collected using custom web scrapers targeting Turkish educational websites. The process included:

- Automated content filtering to remove advertisements and navigation elements
- Conversion to clean Markdown with proper structure
- Image downloading and embedding with relative paths

## License & Legal Disclaimer

> [!WARNING]
> All textbooks included here are the intellectual property of the Turkish Ministry of Education (MEB).  
> Solution guides are compiled from publicly accessible educational sources. This repository is intended solely for educational and non-commercial use.  
> If you are a copyright holder and believe your material has been included inappropriately, please open an issue on GitHub to request its removal.  
> This repository itself does not carry a specific license; all third-party materials remain subject to their original respective licenses.
