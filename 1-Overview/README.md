# Overview

在前言，我們說明提供的部署方式有 6 種，分別如下：

1. 使用 Kubernetes yaml 部署 free5GC
2. 使用 Helm 部署 free5GC
3. 搭配 CRD 與 Operator 來部署 free5GC
4. 使用 Operator Lifecycle Manager (OLM), CRD 與 Operator 來部署 free5GC
5. 加入管理 SDN 網路的 ONOS ，來整合 free5GC 搭建整個 SDN 5G 的環境
6. 使用 XOS 並建立 free5GC synchronizer 與 Service 來部署 free5GC

以下分別介紹

### 使用 Kubernetes yaml 部署 free5GC

#### 架構

如下圖所示，此部署方式最為單純。就是在 K8s 上面放上 free5GC 5 個 function 而已，且用單純的 K8s resource 方式部署。  
![](https://i.imgur.com/OVAxVQY.png)  
但在網路的架構上，我們會需要在 pod 中建立另外一個 Network interface ，架構如下圖所示。  
![](https://i.imgur.com/BdC3Qef.png)  

#### 說明

使用 Kubernetes yaml 來部署 free5GC。透過 `kubectl create -f` 指令方式部署。

### 使用 Helm 部署 free5GC

#### 架構

如下圖所示，此部署方式最為單純。就是在 K8s 上面放上 free5GC 5 個 function 而已。  
![](https://i.imgur.com/OVAxVQY.png)  
但在網路的架構上，我們會需要在 pod 中建立另外一個 Network interface ，架構如下圖所示。  
![](https://i.imgur.com/BdC3Qef.png)  

#### 說明

使用 Helm 來部署 free5GC。透過 `helm install` 指令方式部署。

### 搭配 CRD 與 Operator 來部署 free5GC

#### 架構

#### 說明

### 使用 Operator Lifecycle Manager (OLM), CRD 與 Operator 來部署 free5GC

#### 架構

#### 說明

### 加入管理 SDN 網路的 ONOS ，來整合 free5GC 搭建整個 SDN 5G 的環境

#### 架構

#### 說明

### 使用 XOS 並建立 free5GC synchronizer 與 Service 來部署 free5GC

#### 架構

#### 說明

