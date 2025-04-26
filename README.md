作者：神里劈瓜

## 项目介绍
<font style="color:rgb(31, 35, 40);">基于 Vue 3 + Spring Boot + COS + WebSocket 的 </font>**<font style="color:rgb(31, 35, 40);">企业级智联云图库平台</font>**<font style="color:rgb(31, 35, 40);">。</font>

<font style="color:rgb(31, 35, 40);">这个平台的应用场景非常广泛，核心功能可分为 4 大类。</font>

<font style="color:rgb(31, 35, 40);">1）所有用户都可以在平台公开上传和检索图片素材，快速找到需要的图片。可用作表情包网站、设计素材网站、壁纸网站等：</font>

![](https://cdn.nlark.com/yuque/0/2025/png/54472557/1745516445661-71e29b53-bd96-4c8f-a270-bd33739c5442.png)

<font style="color:rgb(31, 35, 40);">2）管理员可以上传、审核、批量抓取和管理图片，并对系统内的图片进行分析：</font>

![](https://cdn.nlark.com/yuque/0/2025/png/54472557/1745516537995-f9061d53-1e3e-4899-9573-40b57046aa29.png)

<font style="color:rgb(31, 35, 40);">3）对于个人用户，可将图片上传至私有空间进行批量管理、检索、编辑和分析，用作个人网盘、个人相册、作品集等：</font>

![](https://cdn.nlark.com/yuque/0/2025/png/54472557/1745516814725-b80eedd9-7a0c-470a-9e78-cd4126dd9d85.png)

<font style="color:rgb(31, 35, 40);">4）对于企业，可开通团队空间并邀请成员，共享图片并实时协同编辑图片，空间资源分析，提高团队协作效率。可用于提供商业服务，如企业活动相册、企业内部素材库等：</font>

![](https://cdn.nlark.com/yuque/0/2025/png/54472557/1745521376258-5ba7b3e2-24c4-48dc-aca7-f2257b886069.png)

![](https://cdn.nlark.com/yuque/0/2025/png/54472557/1745518258662-ceb3959e-d9bb-48ff-a1e0-d06e2e388c04.png)

![](https://cdn.nlark.com/yuque/0/2025/png/54472557/1745520344780-831bb7b6-1f51-42d9-8a7a-c6d6a23d2dfa.png)

![](https://cdn.nlark.com/yuque/0/2025/png/54472557/1745520964543-a31a4657-4249-44fd-bee4-58ef9f294227.png)

<font style="color:rgb(31, 35, 40);">该项目功能丰富，涉及文件存管、内容检索、权限控制、实时协同等企业主流业务场景，并运用多种编程思想、架构设计方法和优化策略来保证项目的高速迭代和稳定运行。</font>



还有更多实用的功能，不妨注册账号体验一下吧~

## <font style="color:rgb(31, 35, 40);">项目架构</font>
![](https://camo.githubusercontent.com/46215679e93c6cc2cc423ccc151a10d7555851b333c5fde2547e7893494710dc/68747470733a2f2f7069632e797570692e6963752f312f313733323639313838393130302d65353632633730392d636666612d343737642d393332392d3164633561633164333563382d32303234313230343134343330343734312d32303234313230343134353334343933352d32303234313230343134353335343233342e706e67)

## 技术选型
### 后端
+ <font style="color:rgb(31, 35, 40);">Java Spring Boot 框架</font>
+ <font style="color:rgb(31, 35, 40);">MySQL 数据库 + MyBatis-Plus 框架 + MyBatis X</font>
+ <font style="color:rgb(31, 35, 40);">Redis 分布式缓存 + Caffeine 本地缓存</font>
+ <font style="color:rgb(31, 35, 40);">Jsoup 数据抓取</font>
+ <font style="color:rgb(31, 35, 40);"></font><font style="color:rgb(31, 35, 40);">COS 对象存储</font>
+ <font style="color:rgb(31, 35, 40);"></font><font style="color:rgb(31, 35, 40);">ShardingSphere 分库分表</font>
+ <font style="color:rgb(31, 35, 40);">Sa-Token 权限控制</font>
+ <font style="color:rgb(31, 35, 40);">DDD 领域驱动设计</font>
+ <font style="color:rgb(31, 35, 40);">WebSocket 双向通信</font>
+ <font style="color:rgb(31, 35, 40);">Disruptor 高性能无锁队列</font>
+ <font style="color:rgb(31, 35, 40);">JUC 并发和异步编程</font>
+ <font style="color:rgb(31, 35, 40);">AI 绘图大模型接入</font>
+ <font style="color:rgb(31, 35, 40);">多种设计模式的运用</font>
+ <font style="color:rgb(31, 35, 40);">多角度项目优化：性能、成本、安全性等</font>

### 前端
+ <font style="color:rgb(31, 35, 40);">Vue 3 框架</font>
+ <font style="color:rgb(31, 35, 40);">Vite 打包工具</font>
+ <font style="color:rgb(31, 35, 40);">Ant Design Vue 组件库</font>
+ <font style="color:rgb(31, 35, 40);">Axios 请求库</font>
+ <font style="color:rgb(31, 35, 40);">Pinia 全局状态管理</font>
+ <font style="color:rgb(31, 35, 40);">其他组件：数据可视化、图片编辑等</font>
+ <font style="color:rgb(31, 35, 40);">前端工程化：ESLint + Prettier + TypeScript</font>
+ <font style="color:rgb(31, 35, 40);">OpenAPI 前端代码生成</font>

<font style="color:rgb(31, 35, 40);"></font>

## <font style="color:rgb(31, 35, 40);">Sa-Token</font><font style="color:rgb(31, 35, 40);">权限控制逻辑图</font>
![](https://cdn.nlark.com/yuque/0/2025/png/54472557/1745520661677-ca0dbdd1-5d64-4f4c-9ef6-7a07190981f6.png)



感谢你的使用！如果你发现任何问题或有功能建议，欢迎通过 825710099@qq.com 联系我，我会尽快回复。:)

