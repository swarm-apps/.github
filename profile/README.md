# swarm-apps

<p align="right">
  <a href="./README.en.md">English</a>
</p>

<p align="center">
  面向本地优先与点对点协作的一组开源应用与基础设施。
</p>

## 关于

**swarm-apps** 围绕一个很简单的想法构建：

> 你的数据应该留在你自己的设备上，而你的设备应该可以彼此直接同步。

我们关注的是：

- **本地优先** 的数据所有权
- **点对点** 网络，而不是强依赖中心服务器
- 覆盖桌面端与移动端的 **跨平台应用**
- 可复用、可开放演进的 **协议与基础设施**

## 项目

<table>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmNote">SwarmNote</a></h3>
      <p>一个 Markdown-first、本地优先、内置 P2P 同步的笔记应用。</p>
      <ul>
        <li>普通本地 Markdown 文件</li>
        <li>基于 libp2p 的设备直连同步</li>
        <li>通过 Yjs/CRDT 保证可合并</li>
        <li>Tauri + React + Rust + CodeMirror 6</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmNote-RN">SwarmNote-RN</a></h3>
      <p>SwarmNote 的移动端伙伴应用，基于 Expo 与 React Native 构建。</p>
      <ul>
        <li>与桌面端共享核心逻辑</li>
        <li>通过 WebView 复用 CodeMirror 编辑器</li>
        <li>让你的手机加入笔记 swarm</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/SwarmDrop">SwarmDrop</a></h3>
      <p>一个去中心化的跨网络文件传输应用。</p>
      <ul>
        <li>无需账号</li>
        <li>无需云端依赖</li>
        <li>端到端加密传输</li>
        <li>面向设备到设备直连传输</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/swarm-p2p">swarm-p2p</a></h3>
      <p>这些应用背后的可复用 P2P 网络基础层。</p>
      <ul>
        <li>mDNS 局域网发现</li>
        <li>Kademlia DHT 广域发现</li>
        <li>NAT 穿透与中继兜底</li>
        <li>面向应用协议的请求响应 API</li>
      </ul>
    </td>
  </tr>
  <tr>
    <td width="50%" valign="top">
      <h3><a href="https://github.com/swarm-apps/swarmnote-editor">swarmnote-editor</a></h3>
      <p>从 SwarmNote 中抽离出来、基于 CodeMirror 6 的 Markdown 编辑器。</p>
      <ul>
        <li>Markdown-first 编辑模型</li>
        <li>Live Preview 交互</li>
        <li>面向桌面与移动宿主的跨平台编辑器核心</li>
        <li>正在演进为可复用开源编辑器包</li>
      </ul>
    </td>
    <td width="50%" valign="top">
      <h3>More coming</h3>
      <p>这个生态仍在持续演进，覆盖应用层、编辑器运行时和网络基础设施。</p>
      <ul>
        <li>应用</li>
        <li>共享运行时</li>
        <li>开放基础设施</li>
      </ul>
    </td>
  </tr>
</table>

## 设计原则

我们尽量让整个技术栈围绕这些原则展开：

- 能保持 **Markdown / 文件是真相源** 的地方，就不引入额外抽象
- 平台相关能力由宿主应用注入，而不是硬编码进核心层
- 优先共享 **交互语义**，再分别适配平台 UI
- 尽可能坚持 **开源优先**

## 关注进展

- 浏览上面的仓库
- 在各项目 Releases 中查看可下载版本
- 在对应仓库通过 Issues 或 Discussions 参与交流

---

<p align="center">
  为你自己的设备，先构建一组真正协同工作的 swarm apps。
</p>
