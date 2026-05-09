# swarm-apps

Open-source apps and infrastructure for a local-first, peer-to-peer workflow.

## What we build

**swarm-apps** is a small ecosystem of tools built around a simple idea:

> Your data should live on your own devices, and your devices should sync directly with each other.

We focus on:

- **Local-first** data ownership
- **Peer-to-peer** networking with no central server requirement
- **Cross-platform** apps for desktop and mobile
- **Open protocols and reusable infrastructure**

## Projects

### [SwarmNote](https://github.com/swarm-apps/SwarmNote)
A Markdown-first, local-first note-taking app with built-in P2P sync.

- Notes are ordinary local Markdown files
- Devices sync directly over libp2p
- Yjs/CRDT keeps edits mergeable across devices
- Built with Tauri, React, Rust, and CodeMirror 6

### [SwarmNote-RN](https://github.com/swarm-apps/SwarmNote-RN)
The mobile companion for SwarmNote, built with Expo and React Native.

- Shares the same core logic as the desktop app
- Reuses the same CodeMirror-based editor through a WebView runtime
- Brings your note swarm to Android and iOS

### [SwarmDrop](https://github.com/swarm-apps/SwarmDrop)
A decentralized file transfer app for sending files across networks.

- No account
- No cloud dependency
- End-to-end encrypted transfer
- Built for direct device-to-device delivery over libp2p

### [swarm-p2p](https://github.com/swarm-apps/swarm-p2p)
The reusable networking foundation behind the apps.

- mDNS local discovery
- Kademlia DHT for wide-area discovery
- AutoNAT, DCUtR, and Relay for NAT traversal
- Request-response APIs for app protocols

### [swarmnote-editor](https://github.com/swarm-apps/swarmnote-editor)
A CodeMirror 6 based Markdown editor extracted from SwarmNote.

- Markdown-first editing model
- Live preview interactions
- Cross-platform editor core for desktop and mobile hosts
- Being refactored toward a reusable open-source editor package

## Design principles

We try to keep the stack aligned around a few principles:

- **Markdown / files remain the source of truth when possible**
- **Host apps inject platform-specific capabilities instead of hardcoding them into the core**
- **Shared semantics first, platform UI second**
- **Open-source by default**

## Current direction

Right now the ecosystem is evolving in three complementary layers:

1. **Apps** — user-facing tools like SwarmNote and SwarmDrop
2. **Shared runtime** — reusable editor and mobile/desktop integration layers
3. **Network infrastructure** — the libp2p foundation that makes direct sync possible

## Follow along

- Browse the repositories above
- Check Releases in each project for downloadable builds
- Open Issues or Discussions in the relevant repo if you want to contribute or follow progress

---

Building a swarm of apps that work for your own devices first.
