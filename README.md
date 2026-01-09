# DotAgents

Agent configuration templates for OurSky/Vendatta - providing isolated development environments with AI agent integration.

This repository contains migrated configuration templates from the spec-to-code development workflow, adapted for use with OurSky (Vendatta) agent system.

## Structure

```
.oursky/templates/
├── commands/          # Agent command specifications (design, plan, implement, etc.)
├── rules/            # Coding standards and guidelines (api.md, portal.md)
└── skills/           # Custom agent skills (empty for now)

examples/scopes/      # Example feature scopes demonstrating the workflow
```

## Migration from .another-cursor

This repository migrates the spec-to-code pattern from `.another-cursor/` to OurSky agent config:

- **Commands**: Adapted from Cursor command specifications to work with OurSky agents
- **Rules**: Coding guidelines with paths updated from `.cursor` to `.oursky`
- **Scopes**: Example feature directories showing the workflow in action

All paths have been updated from `.cursor/` to `.oursky/` to work with Vendatta's directory structure.

## Usage

1. Clone this repository
2. Copy the `.oursky/templates/` directory to your project's `.oursky/templates/`
3. Configure your `.oursky/config.yaml` to enable the desired agents
4. Run `oursky dev feature-name` to start development with the spec-to-code workflow

## Commands Available

- `/design` - Create feature specifications
- `/plan` - Generate dependency-ordered tasks
- `/implement` - Execute tasks with memory-first approach
- `/test` - Test features with real app
- `/ci` - Run CI checks and fix issues
- `/summarize` - Generate quick context summaries
- `/consolidate` - Update memory documentation

## Example

See the `examples/scopes/20251126-195612-MultiplePageFileAPI/` for a complete example of the workflow in action.

## Integration with Vendatta

When used with [Vendatta](https://github.com/oursky/vendatta), these templates provide:

- Standardized AI agent commands across Cursor, OpenCode, and Claude
- Consistent coding standards enforcement
- Spec-to-code development workflow
- Isolated development environments

*Powered by OhMyOpenCode*