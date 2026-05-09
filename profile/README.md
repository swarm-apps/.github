# swarm-apps

<p align="center">
  Open-source apps and infrastructure for a local-first, peer-to-peer workflow.<br/>
  面向本地优先与点对点协作的一组开源应用与基础设施。
</p>

## About / 关于

**EN**

**swarm-apps** is an ecosystem built around a simple idea:

> Your data should live on your own devices, and your devices should sync directly with each other.

We focus on:

- **Local-first** data ownership
- **Peer-to-peer** networking with no central server requirement
- **Cross-platform** apps for desktop and mobile
- **Open protocols and reusable infrastructure**

**中文**

**swarm-apps** 围绕一个很简单的想法构建：

> 你的数据应该留在你自己的设备上，而你的设备应该可以彼此直接同步。

我们关注的是：

- **本地优先** 的数据所有权
- **点对点** 网络，而不是强依赖中心服务器
- 覆盖桌面端与移动端的 **跨平台应用**
- 可复用、可开放演进的 **协议与基础设施**

## Projects / 项目

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmNote">SwarmNote</a></h3>
      <p><strong>EN:</strong> A Markdown-first, local-first note-taking app with built-in P2P sync.</p>
      <p><strong>中文：</strong>一个 Markdown-first、本地优先、内置 P2P 同步的笔记应用。</p>
      <ul>
        <li>Ordinary local Markdown files / 普通本地 Markdown 文件</li>
        <li>Direct device sync over libp2p / 基于 libp2p 的设备直连同步</li>
        <li>Yjs/CRDT powered mergeability / 通过 Yjs/CRDT 保证可合并</li>
        <li>Tauri + React + Rust + CodeMirror 6</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmNote-RN">SwarmNote-RN</a></h3>
      <p><strong>EN:</strong> The mobile companion for SwarmNote, built with Expo and React Native.</p>
      <p><strong>中文：</strong>SwarmNote 的移动端伙伴应用，基于 Expo 与 React Native 构建。</p>
      <ul>
        <li>Shared core logic with desktop / 与桌面端共享核心逻辑</li>
        <li>CodeMirror editor via WebView runtime / 通过 WebView 复用 CodeMirror 编辑器</li>
        <li>Android and iOS note swarm / 让你的手机加入笔记 swarm</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmDrop">SwarmDrop</a></h3>
      <p><strong>EN:</strong> A decentralized file transfer app for sending files across networks.</p>
      <p><strong>中文：</strong>一个去中心化的跨网络文件传输应用。</p>
      <ul>
        <li>No account / 无需账号</li>
        <li>No cloud dependency / 无需云端依赖</li>
        <li>End-to-end encrypted transfer / 端到端加密传输</li>
        <li>Direct device-to-device delivery / 面向设备到设备直连传输</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/swarm-p2p">swarm-p2p</a></h3>
      <p><strong>EN:</strong> The reusable networking foundation behind the apps.</p>
      <p><strong>中文：</strong>这些应用背后的可复用 P2P 网络基础层。</p>
      <ul>
        <li>mDNS local discovery / mDNS 局域网发现</li>
        <li>Kademlia DHT / Kademlia DHT 广域发现</li>
        <li>AutoNAT, DCUtR, Relay / NAT 穿透与中继兜底</li>
        <li>Request-response APIs / 面向应用协议的请求响应 API</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/swarmnote-editor">swarmnote-editor</a></h3>
      <p><strong>EN:</strong> A CodeMirror 6 based Markdown editor extracted from SwarmNote.</p>
      <p><strong>中文：</strong>从 SwarmNote 中抽离出来、基于 CodeMirror 6 的 Markdown 编辑器。</p>
      <ul>
        <li>Markdown-first editing / Markdown-first 编辑模型</li>
        <li>Live preview interactions / Live Preview 交互</li>
        <li>Cross-platform editor core / 面向桌面与移动宿主的跨平台编辑器核心</li>
        <li>Moving toward a reusable OSS editor package / 正在演进为可复用开源编辑器包</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>More coming</h3>
      <p><strong>EN:</strong> The ecosystem is still evolving across apps, editor runtime, and networking infrastructure.</p>
      <p><strong>中文：</strong>这个生态仍在持续演进，覆盖应用层、编辑器运行时和网络基础设施。</p>
      <ul>
        <li>Apps / 应用</li>
        <li>Shared runtime / 共享运行时</li>
        <li>Open infrastructure / 开放基础设施</li>
      </ul>
    </td>
  </tr>
</table>

## Principles / 设计原则

**EN**

We try to keep the stack aligned around a few principles:

- **Markdown / files remain the source of truth when possible**
- **Host apps inject platform-specific capabilities instead of hardcoding them into the core**
- **Shared semantics first, platform UI second**
- **Open-source by default**

**中文**

我们尽量让整个技术栈围绕这些原则展开：

- 能保持 **Markdown / 文件是真相源** 的地方，就不引入额外抽象
- 平台相关能力由宿主应用注入，而不是硬编码进核心层
- 优先共享 **交互语义**，再分别适配平台 UI
- 尽可能坚持 **开源优先**

## Follow along / 关注进展

- Browse the repositories above / 浏览上面的仓库
- Check Releases for downloadable builds / 在各项目 Releases 中查看可下载版本
- Open Issues or Discussions in the relevant repo / 在对应仓库通过 Issues 或 Discussions 参与交流

---

<p align="center">
  Building a swarm of apps that work for your own devices first.<br/>
  为你自己的设备，先构建一组真正协同工作的 swarm apps。
</p>
