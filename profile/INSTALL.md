# GitHub Profile Package

Copy the contents of `profile/` into the organization's:

`.github/profile/`

Result:

```text
.github/
└── profile/
    ├── README.md
    ├── design-tokens.css
    └── assets/
        └── profile.png
```

`README.md` is the actual rendered design. It does not use generated screenshots,
hero SVGs, capability SVGs, or screenshot-as-content.

`design-tokens.css` preserves the AitiStack design-token system as the source of
truth for the web/portfolio implementation. GitHub does not load repository CSS
into rendered README content, so the README uses GitHub-supported Markdown and
HTML layout primitives.

Resume link is currently `./resume.pdf`; replace it yourself when ready.
