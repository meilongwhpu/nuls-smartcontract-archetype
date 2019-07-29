# nuls-smartcontract-archetype
在创建智能合约项目时，向IDEA中添加该NULS智能合约archetype,然后选择此archetype生成NULS智能合约项目，生成的项目已自动完成了所需jar包的依赖，开发者只需编写业务代码，再使用maven打包智能合约后将会自动启动智能合约调试平台，开发者可以在此平台上进行智能合约的调试工作。

## 如何建立
### 条件
- JDK1.8版本
- Maven 3.5及以上版本

### 获取来源
     git clone https://github.com/meilongwhpu/nuls-smartcontract-archetype.git

### 建立源头
    $mvn clean install
成功构建maven后，工件将上传到您当地的maven仓库。

## 创建NULS智能合约项目
- 点击IntelliJ IDE的菜单：File->New Project
- 勾选“Create From archetype”
- 点击“Add Archetype”，填写：

         GroupId：io.nuls
         ArtifactId: nuls-smartcontract-archetype 
         Version: 1.1
- 选择生成的“io.nuls:nuls-smartcontract-archetype",点击下一步，创建NULS智能合约项目

## 以原型生成的智能合约项目
- 该智能合约项目为maven项目
- 该智能合约项目中自带样本合约类，并且所有必需的NULS智能合约依赖项都自动添加到项目中
- 该智能合约项目自动依赖了离线智能合约调试平台
- 通过mvn clean pakcage对合约进行打包时，会启动离线智能合约，并且将合约部署到离线智能合约调试平台上
- 无需上传jar包或生成合约十六进制代码，简化合约部署和执行操作
- 该智能合约项目附带一些有用的工具类，便于智能合约的开发


