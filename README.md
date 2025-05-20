````markdown
# 📄 Automated Resume Builder

A command-line tool to generate beautiful, customizable resumes using structured data, templates and Large Language Models to customize your resume for the job you want. Write your resume once in JSON/YAML and export it as PDF, HTML, or LaTeX with consistent formatting and style and tailored to the job you want.

---

## ✨ Features

- 🔧 Write your resume once in `JSON` or `YAML`
- 🎨 Choose from multiple built-in templates (LaTeX/HTML)
- 🖨️ Export to PDF or HTML
- 🧩 Template-driven: Easy to customize look and feel
- 🚀 Fast CLI workflow for quick edits and rebuilds
- 🌍 Access to cutting edge models to tailor to the job

---

## 📦 Installation

```bash
git clone https://github.com/yourusername/resume-builder.git
cd resume-builder
pip install -r requirements.txt
````

> Requires Python 3.7+

---

## 🛠 Usage

### 1. Prepare your data

Create a file called `resume.json` or `resume.yaml`:

```json
{
  "name": "John Doe",
  "title": "Software Engineer",
  "contact": {
    "email": "john@example.com",
    "github": "johndoe",
    "linkedin": "john-doe"
  },
  "education": [
    {
      "degree": "B.Sc. in Computer Science",
      "institution": "XYZ University",
      "year": "2020"
    }
  ],
  "experience": [
    {
      "title": "Backend Developer",
      "company": "Acme Corp",
      "duration": "2020–2023",
      "description": "Worked on APIs, microservices, and internal tooling."
    }
  ]
}
```

---

### 2. Generate your resume

```bash
python builder.py --input resume.json --template modern --output resume.pdf
```

* `--input`: Path to your resume data
* `--template`: Choose a template (e.g. `modern`, `classic`, `minimal`)
* `--output`: Output file name and format (PDF/HTML)

---

## 🧪 Templates

Available templates:

* `modern` – sleek and clean layout
* `classic` – traditional look
* `minimal` – single-column minimal design

To create your own template, copy one from the `templates/` folder and modify it.

---

## 🧰 Project Structure

```
resume-builder/
│
├── builder.py           # Main CLI tool
├── templates/           # LaTeX and HTML templates
├── sample_resume.json   # Example resume data
├── utils/               # Helper functions (e.g., validation, parsing)
└── README.md
```

---

## ✅ TODO

* [ ] Add LinkedIn/GitHub profile scraping integration
* [ ] Web interface (Flask or Streamlit)
* [ ] Live preview mode
* [ ] Export to DOCX

---

## 🤝 Contributing

Pull requests are welcome! If you’d like to contribute a new template or improve the builder, feel free to fork the repo and submit a PR.

---

## 📄 License

MIT License. See `LICENSE` file for details.

---

## 🙌 Credits

Created by [Your Name](https://github.com/rburketaylor)

```

---

Let me know if you'd like to include a specific template preview or if you're using a particular library like `Jinja2`, `WeasyPrint`, or `LaTeX`. I can tailor it further.
```
