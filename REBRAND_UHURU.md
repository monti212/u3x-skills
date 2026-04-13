# Uhuru Skills Rebrand Migration Guide

This repository is being rebranded for the Uhuru ecosystem.

## Target Brand Structure

- Product family: **Uhuru 3**
- Model versions: **U3.4**, **U3.5**
- Skills layer: **Uhuru Skills**
- Skill IDs:
  - `uhuru-docx`
  - `uhuru-pdf`
  - `uhuru-xlsx`

## New Target Structure

```text
uhuru-skills/
├── skills/
│   ├── uhuru-docx/
│   ├── uhuru-pdf/
│   └── uhuru-xlsx/
└── examples/
```

## Required Follow-up Changes

### 1. Rename tracked folders

- `skills/kimi-docx/` → `skills/uhuru-docx/`
- `skills/kimi-pdf/` → `skills/uhuru-pdf/`
- `skills/kimi-xlsx/` → `skills/uhuru-xlsx/`

### 2. Replace public-facing identity strings

- `Kimi Skills` → `Uhuru Skills`
- `kimi-docx` → `uhuru-docx`
- `kimi-pdf` → `uhuru-pdf`
- `kimi-xlsx` → `uhuru-xlsx`
- `/app/.kimi` → `/app/.uhuru`
- `KimiXlsx` → `UhuruXlsx`
- `KimiDocx.csproj` → `UhuruDocx.csproj`

### 3. Update install references

- `npx skills add thvroyal/kimi-skills`
- replace with:
- `npx skills add monti212/uhuru-skills`

## Positioning

Use the following positioning language:

> Uhuru Skills power advanced document, PDF, and spreadsheet workflows for the Uhuru 3 model family.

> Compatible with Uhuru 3, U3.4, and U3.5.

## Notes

This guide does not delete old files. It defines the target state for the repository migration.
