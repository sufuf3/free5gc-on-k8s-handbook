# 在 Kubernetes 上部署 free5GC 之手冊

存粹部署 free5GC 在 Kubernetes 上有以下 4 種方法：  

1. 使用 Kubernetes yaml 部署 free5GC  
2. 使用 Helm 部署 free5GC  
3. 搭配 CRD 與 Operator 來部署 free5GC  
4. 使用 Operator Lifecycle Manager (OLM), CRD 與 Operator 來部署 free5GC  

另外有加入管理 SDN 網路的 ONOS ，來整合 free5GC 搭建整個 SDN 5G 的環境。此為第 5 種方法。  
以及用 xos 部署 free5GC 的方法，此為第 6 種方法。
  
在本手冊，會針對以上 6 種方法的部署方式分別提供安裝與操作步驟。  
  
- [1. Overview](1-Overview): 在本章，會說明 6 種部署的差異與架構。
- [2. Installation Guide](2-Installation_Guide): 在本章，除了 Kubernetes, Network, Infrastructure 的 setup 方法會獨立用一章節討論外，其他五種方式問分別提供安裝的操作步驟。在這章中，你會建立完整的 free5GC on Kubernetes 平台。
- [3. Using Guide](3-Using_Guide): 佈建好 free5GC 總要知道怎麼再搭配 UE, enodeB 來建構完整的 5G 平台吧！這章就在教會你如何從 UE 連到 free5GC 後可以上網。因為 6 種方式在連接 UE 和 enodeB 都是一樣的，所以這邊不會分別介紹。
- [4. Development Guide](4-Development_Guide): 我們 Setup 好整個 free5GC 的大平台，但當我們想要調整一些元件呢？這邊不會教如何開發 free5GC ，但會針對 6 種方式，在 deploy 上會需要開發或調整的部分，進行相關的說明。

如果你想對 Kubernetes 和 free5GC 有更深入的了解，請參考以下網站：  
- Kubernetes: https://kubernetes.io/
- free5GC: https://www.free5gc.org/
