# Flex plugins

Open **View → Customize** to browse installed plugins and skills. Flex includes Meme Pack (original reaction cutaways, sounds, skill and style) and a DaVinci Resolve FCPXML file-exchange example. They are available offline and can be reinstalled from the browser.

To add a community plugin, choose **Add** and enter its public GitHub repository URL. Flex previews a compatible stable release containing matching `plugin.json` and `plugin.zip` assets. Code plugins require publisher trust and can access your computer; content packages provide declarations and assets without executable entry points. Local folders support author development. Version 1 has no custom frontend components.

The Python package `flex-plugin-sdk` supplies registration and public host services. The source repository's `sdk/README.md` and `plugins/` examples document authoring. Engine validates and commits project changes. Skills and styles never grant editing permissions, and used assets remain available after uninstalling their plugin.

Resolve exchange supports a limited cut-and-audio subset, with explicit unsupported-feature errors and review before import. Live Resolve operation, Premiere and direct YouTube uploads are not included.

`data/plugin-registry.json` is the curated community discovery list. It is initially empty; the included examples are discovered from the installed app. Each future entry needs a unique lowercase `id`, `name`, `description`, `author`, `type`, `category` and `repo` (`owner/repository`). The repository must publish compatible stable release assets. Registry additions and plugin releases are reviewed and published separately.
