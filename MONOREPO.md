# Awesome Lists Monorepo

This repository contains a collection of **all** awesome lists from the [Awesome](https://github.com/sindresorhus/awesome) project, organized as Git submodules.

## What is this?

The original [Awesome](https://github.com/sindresorhus/awesome) repository is a curated list of awesome lists - essentially a catalog of links to other GitHub repositories, each containing a curated list of resources on a specific topic.

This monorepo takes it a step further by:

1. Including all those individual awesome lists as Git submodules
2. Providing a single repository that contains (or can contain) all the content locally
3. Making it possible to browse all awesome lists offline
4. Allowing you to keep everything updated with a few simple commands

## Repository Structure

- `readme.md` - The original awesome list catalog (maintained by sindresorhus)
- `awesome_lists/` - Directory containing all awesome lists as submodules
- `sync_awesome_lists.sh` - Script used to clone and manage all the awesome lists
- Other files from the original awesome repository

## Stats

- Total size: ~4.5GB
- Number of submodules: ~685
- Covers virtually all topics in software development, data science, and many other fields

## Usage

### Cloning the Repository

To clone this repository with all submodules:

```bash
# Clone the repository
git clone https://github.com/mikelasaddu/awesomelists-monorepo.git

# Initialize and update all submodules (this will download ~4.5GB of data)
cd awesomelists-monorepo
git submodule update --init --recursive
```

### Updating the Repository

To update all awesome lists to their latest versions:

```bash
# Pull the latest changes from the original awesome repository
git pull upstream main

# Update all submodules to their latest versions
git submodule update --recursive --remote

# Or run the sync script to add any new awesome lists
./sync_awesome_lists.sh
```

## Benefits

- **Complete offline access** to all awesome lists
- **Single command updates** for all lists
- **Automatic tracking** of new awesome lists added to the original repository
- **Consistent interface** for browsing all lists
- **Preservation** of awesome lists even if the original repositories disappear

## Acknowledgments

This monorepo wouldn't be possible without the incredible work of [Sindre Sorhus](https://github.com/sindresorhus) and all the maintainers of the individual awesome lists.

## License

Each awesome list included as a submodule maintains its original license. Please refer to each individual repository for license information. 