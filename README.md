# emma Documentation

emma documentation - Powered by [Mintlify](https://mintlify.com)

## Development

Install the [Mintlify CLI](https://www.npmjs.com/package/mintlify) to preview the documentation changes locally.

```bash
npm i -g mintlify
```

Run the following command at the root of your documentation (where `docs.json` is):

```bash
mintlify dev
```

## Publishing Changes

Changes will be deployed automatically when pushed to the main branch.

## Project Structure

```
emma-docs/
├── docs.json              # Site configuration
├── llms.txt               # LLM-friendly documentation index
├── introduction.mdx       # Home page
├── quickstart.mdx         # Quickstart guide
├── changelog.mdx          # Release notes
├── guides/                # User guides
│   ├── overview.mdx
│   ├── best-practices.mdx
│   └── troubleshooting.mdx
├── integrations/          # Integration guides
│   ├── overview.mdx
│   └── slack.mdx
├── api-reference/         # API documentation
│   ├── overview.mdx
│   └── authentication.mdx
└── images/                # Static assets
```

## Key Features

- **llms.txt**: LLM-friendly index for AI assistants to discover documentation
- **Tabs**: Documentation and API Reference tabs for easy navigation
- **Search**: Built-in search functionality
- **Feedback**: Thumbs up/down rating on pages
- **Components**: Cards, Steps, Tabs, Accordions, and more

## Adding New Pages

1. Create a new `.mdx` file in the appropriate directory
2. Add frontmatter with `title` and `description`
3. Add the page path to `docs.json` navigation
4. Update `llms.txt` with the new page

## Mintlify Components

This documentation uses various Mintlify components:

- `<CardGroup>` / `<Card>` - Feature cards
- `<Steps>` / `<Step>` - Step-by-step guides
- `<Tabs>` / `<Tab>` - Tabbed content
- `<AccordionGroup>` / `<Accordion>` - Collapsible sections
- `<Note>` / `<Warning>` - Callout boxes
