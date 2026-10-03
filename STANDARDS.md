# Plex Studios Repository Standard

This document defines the default presentation and documentation standard for Plex Studios repositories.

The goal is consistency: every Plex Studios project should feel like part of one professional product family while still keeping its own identity.

## Core Presentation Rules

- Use the product name exactly as branded.
- Keep README layouts consistent across repositories.
- Use concise, technical language rather than marketing-heavy filler.
- Avoid excessive emojis, novelty badges, decorative separators, or generic Minecraft-resource styling.
- Keep headings predictable so users can scan every Plex repository the same way.
- Use the same terminology across README, Wiki, changelog, marketplace pages, and in-game documentation.
- Do not advertise unimplemented features.
- Clearly distinguish tested compatibility from intended compatibility.
- Keep screenshots and banners visually consistent with the Plex Studios visual system.
- Keep paid-source repositories private while allowing public documentation and support where appropriate.

## README Structure

Project READMEs should normally follow this order:

1. Project identity
2. Short value proposition
3. Compatibility
4. Overview
5. Features
6. Installation
7. Commands and permissions
8. Configuration
9. Integrations or placeholders
10. Documentation
11. Building from source when public
12. Support
13. License
14. Plex Studios footer

Not every section is required for every project, but the order should remain stable.

## Project Identity

The top of each README should contain:

- Project name
- One concise value proposition
- Compatibility information
- A project banner or social-preview image when available

Avoid cluttering the header with many badges.

Recommended compatibility badges are limited to useful information such as:

- Paper version
- Java version
- License
- Build status

## Writing Style

Use:

- Clear technical English
- Short paragraphs
- Direct feature descriptions
- Consistent command, permission, placeholder, and configuration formatting

Avoid:

- Overclaiming
- Excessive hype
- Repeating the same feature in several sections
- Generic phrases such as "the ultimate plugin"
- Unsupported performance claims
- Unverified compatibility claims

## Feature Lists

Features should describe actual behavior.

Good:

- SQLite-backed player streak persistence
- Optional PlaceholderAPI integration
- Transactional configuration reload

Avoid:

- Blazing fast
- Best in class
- Ultimate performance
- Zero lag

unless there is a precise, supportable technical meaning.

## Commands and Permissions

Use Markdown tables.

Example:

| Command | Description | Permission |
| --- | --- | --- |
| `/example` | Opens the example interface | `plex.example` |

Permissions should state their default where useful.

## Configuration

Keep README configuration examples short.

Large configuration references belong in the Wiki or PlexDocs.

README should explain:

- where the configuration file lives
- the most important defaults
- where the complete reference is documented

## Documentation Strategy

Use three documentation layers.

### README

The quick product overview.

It should answer:

- What is this?
- What does it do?
- What does it require?
- How do I install it?
- Where do I go next?

### GitHub Wiki

Use for complex projects that need substantial project-specific documentation.

Recommended Wiki structure:

- Home
- Installation
- Quick Start
- Configuration
- Commands and Permissions
- Integrations
- Placeholders
- Storage or Data
- Advanced Usage
- Troubleshooting
- FAQ

Only include pages relevant to the project.

### PlexDocs

The public cross-project documentation hub.

Use PlexDocs for:

- central product navigation
- shared concepts
- public documentation for paid projects
- compatibility matrices
- cross-project integration guides
- documentation that should remain available even when source is private

## Wiki Style

Wiki pages should:

- start with one sentence explaining the page purpose
- use H2 sections for major topics
- keep examples focused
- use tables for commands, permissions, placeholders, and setting references
- link back to Home and relevant neighboring pages
- avoid duplicating the entire README
- avoid duplicating changelog entries

## Changelog

Every project should maintain `CHANGELOG.md`.

Use release headings and factual change entries.

Do not write release notes for versions that have not been released unless clearly marked as Unreleased or Development.

## Support Files

Public projects should normally provide:

- `README.md`
- `CHANGELOG.md`
- `CONTRIBUTING.md`
- `SUPPORT.md`
- `SECURITY.md` when appropriate
- issue templates
- pull request template
- CI workflow when the project can be built automatically

## Visual Consistency

Plex Studios uses a shared premium visual system.

All repositories should use compatible:

- typography
- spacing
- banner composition
- icon treatment
- screenshot framing
- accent-color logic
- naming conventions

Each product may have its own accent while remaining visibly part of the Plex Studios family.

Avoid generic blocky Minecraft-resource artwork unless it is intentionally part of the product identity.

## Repository Naming

Use the official product name directly.

Preferred:

```text
PlexVariables
PlexAware
PlexKillstreaks
PlexMenus
PlexBridge
PlexDocs
```

Avoid descriptive suffixes unless they serve a real purpose.

## Paid Projects

For paid projects:

- source repository may remain private
- public documentation may live in PlexDocs
- public support/issue repositories may be created separately if useful
- never expose private implementation details simply to provide documentation

## Compatibility Claims

Always separate:

- intended compatibility
- compile-time compatibility
- automated test coverage
- real runtime-tested versions

Never imply a version was tested when it was not.

## Plex Studios Footer

Public repositories should end with a small, consistent Plex Studios attribution and links to the organization and documentation hub.

Keep it understated.
