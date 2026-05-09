# swarm-apps

<p align="right">
  <a href="./README.md">简体中文</a>
</p>

<p align="center">
  Open-source apps and infrastructure for a local-first, peer-to-peer workflow.
</p>

## About

**swarm-apps** is an ecosystem built around a simple idea:

> Your data should live on your own devices, and your devices should sync directly with each other.

We focus on:

- **Local-first** data ownership
- **Peer-to-peer** networking with no central server requirement
- **Cross-platform** apps for desktop and mobile
- **Open protocols and reusable infrastructure**

## Projects

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmNote">SwarmNote</a></h3>
      <p>A Markdown-first, local-first note-taking app with built-in P2P sync.</p>
      <ul>
        <li>Ordinary local Markdown files</li>
        <li>Direct device sync over libp2p</li>
        <li>Yjs/CRDT powered mergeability</li>
        <li>Tauri + React + Rust + CodeMirror 6</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmNote-RN">SwarmNote-RN</a></h3>
      <p>The mobile companion for SwarmNote, built with Expo and React Native.</p>
      <ul>
        <li>Shared core logic with desktop</li>
        <li>CodeMirror editor via WebView runtime</li>
        <li>Brings your note swarm to Android and iOS</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmDrop">SwarmDrop</a></h3>
      <p>A decentralized file transfer app for sending files across networks.</p>
      <ul>
        <li>No account</li>
        <li>No cloud dependency</li>
        <li>End-to-end encrypted transfer</li>
        <li>Direct device-to-device delivery</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/swarm-p2p">swarm-p2p</a></h3>
      <p>The reusable networking foundation behind the apps.</p>
      <ul>
        <li>mDNS local discovery</li>
        <li>Kademlia DHT for wide-area discovery</li>
        <li>AutoNAT, DCUtR, and Relay</li>
        <li>Request-response APIs for app protocols</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/swarmnote-editor">swarmnote-editor</a></h3>
      <p>A CodeMirror 6 based Markdown editor extracted from SwarmNote.</p>
      <ul>
        <li>Markdown-first editing</li>
        <li>Live preview interactions</li>
        <li>Cross-platform editor core</li>
        <li>Moving toward a reusable OSS editor package</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>More coming</h3>
      <p>The ecosystem is still evolving across apps, editor runtime, and networking infrastructure.</p>
      <ul>
        <li>Apps</li>
        <li>Shared runtime</li>
        <li>Open infrastructure</li>
      </ul>
    </td>
  </tr>
</table>

## Principles

We try to keep the stack aligned around a few principles:

- **Markdown / files remain the source of truth when possible**
- **Host apps inject platform-specific capabilities instead of hardcoding them into the core**
- **Shared semantics first, platform UI second**
- **Open-source by default**

## Follow along

- Browse the repositories above
- Check Releases for downloadable builds
- Open Issues or Discussions in the relevant repo

---

<p align="center">
  Building a swarm of apps that work for your own devices first.
</p>
