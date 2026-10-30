# Orca community plugins

Generated catalog of community Orca plugins. Don't edit by hand; list your plugin by adding the GitHub topic `orca-plugin` — see https://onorca.dev/plugins/add/

To use it in Orca: Settings → Plugins → Add marketplace, URL `https://github.com/stablyai/orca-community-plugins.git`, ref `main`.

Community plugins are checked automatically, not reviewed.

## Public record

This repository's history is append-only: `main` refuses force-pushes and deletion. Two files record what was listed and when:

- `identities.json`: each plugin id and the GitHub repository and owner it belongs to, by GitHub's numeric ids. The publisher is the repository owner, like a Go module path. A renamed or transferred repository is held until a maintainer confirms the move, and a deleted-and-recreated repository is refused.
- `releases.lock.json`: every listed `<plugin id>@<version>` with the commit and content hash it was first listed with. Like Go's checksum database, first seen wins: a version never changes, and a moved tag is refused.
