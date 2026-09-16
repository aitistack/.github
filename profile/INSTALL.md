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


## Layout tuning

Main profile grid: **43% About / 57% capabilities**. Capability and technology grids use full-width nested tables with balanced columns and zero cell spacing to minimize horizontal overflow.

## Overflow fix

The profile/capability layout uses a 43/57 split, while the right-side cards
use a constrained 50/50 nested table. Dense technology groups are explicitly
broken with HTML line breaks so GitHub's table min-content sizing does not
create a horizontal scrollbar.
