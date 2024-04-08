核心：
Xray-core 
sing-box: 基于sagernet开发的通用代理平台

协议组合： 
vless（reality，Vision，TCP，WS，gRPC）
VMess（ TCP, WS） websocket
Trojan（TCP, gRPC）
Hysteria（sing-box）：基于 QUIC 的 TCP 和 UDP 代理，专为速度、安全性和抗审查性而设计；基于QUIC协议，卖点是Brutal，一种拥塞控制算法，可以通过用户手动制定所需速率来抵抗丢包
Tuic（sing-box）: 最近流行的一个基于QUIC的国产简单协议，卖点是BBR拥塞控制算法
NaiveProxy（sing-box）：[Browser → Naïve client] ⟶ Censor ⟶ [Frontend → Naïve server] ⟶ Internet；NaïveProxy 使用 Chromium 的网络堆栈来模拟常规 Chrome 浏览器和标准前端服务器之间的流量；

客户端：
window: v2rayN
android: NekoBox for Android , v2ryaNG
linux: NekoRay/NeroBox for PC
IOS： showrocket/ Yet Another Shadow Socket
MAC：Clash/Yet Another Shadow Socket/v2rayU

;mac/windows:Furious ; Android: NekoBoxForAndroid ; IOS:Streisand 


