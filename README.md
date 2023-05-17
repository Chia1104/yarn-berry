# yarn-berry

## Installation

### Install Corepack

The preferred way to manage Yarn is through Corepack, a new binary shipped with all Node.js releases starting from `16.10`. It acts as an intermediary between you and Yarn, and lets you use different package manager versions across multiple projects without having to check-in the Yarn binary anymore.

### Node.js >=16.10

Corepack is included by default with all Node.js installs, but is currently opt-in. To enable it, run the following command:

```bash
corepack enable
```

### Node.js <16.10

Corepack isn't included with Node.js in versions before the 16.10; to address that, run:

```bash
npm i -g corepack
```

### Updating the global Yarn version

#### Node.js ^16.17 or >=18.6

```bash
corepack prepare yarn@stable --activate
```

#### Node.js <16.17 or <18.6

Take a look at the latest Yarn release, note the version number, and run:

```bash
corepack prepare yarn@<version> --activate
```

### Initializing your project

Just run the following command. It will generate some files inside your current directory; add them all to your next commit, and you'll be done!

```bash
yarn init -2
```
