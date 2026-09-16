# AitiStack GitHub Organization Profile

Copy this `profile/` directory into the organization's `.github/` repository:

```text
.github/
└── profile/
    ├── README.md
    ├── design-tokens.css
    └── assets/
        └── profile.png
```

## Layout

The profile intentionally uses a wider **48% About** column and a **52% capability** column.

The four capability panels are stacked vertically instead of being forced into a
nested two-column grid. This prevents GitHub's Markdown table min-content sizing
from creating horizontal overflow.

The Technical Arsenal cards are also stacked vertically so the complete README
remains responsive and does not introduce a horizontal scrollbar.

Only the actual profile photograph is an image asset. The layout itself is
native Markdown/HTML.

Replace `./resume.pdf` in `README.md` with your preferred resume link/file.
