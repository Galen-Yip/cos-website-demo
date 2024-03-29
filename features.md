COS 主要提供以下功能：

<table>
   <tr>
      <th colspan=2>功能</td>
      <th>说明</td>
   </tr>
   <tr>
      <td rowspan=2>操作</td>
      <td nowrap="nowrap">存储桶操作</td>
      <td>支持创建、查询、删除、清空存储桶，具体操作请参见 <a href="https://cloud.tencent.com/document/product/436/13309">存储桶管理</a> 目录下的文档</td>
   </tr>
   <tr>
      <td>对象操作</td>
      <td>多种存储类型：根据对象访问频度的高低，COS 提供三种对象的存储类型：标准存储、低频存储、归档存储，详情请参见 <a href="https://cloud.tencent.com/document/product/436/33417">存储类型</a><br>对象/文件夹：上传、查询、下载、复制和删除操作，具体操作请参见 <a href="https://cloud.tencent.com/document/product/436/13321">对象管理</a> 目录下的文档</td>
   </tr>
   <tr>
      <td rowspan=6>数据管理</td>
      <td>生命周期</td>
      <td>对象存储 COS 支持用户设定规则，对指定对象在某个时间（天数）后进行自动删除或转换存储类型，详情请参见  <a href="https://cloud.tencent.com/document/product/436/17028">生命周期概述</a></td>
   </tr>
   <tr>
      <td>静态网站</td>
      <td>将存储桶配置成静态网站托管模式，并通过存储桶域名访问该静态网站，详情请参见  <a href="https://cloud.tencent.com/document/product/436/32670">托管静态网站</a></td>
   </tr>
   <tr>
      <td>清单</td>
      <td>对象存储 COS 可根据用户的清单任务配置，每天或者每周定时扫描用户存储桶内指定的对象或拥有相同对象前缀的对象，并输出一份清单报告，以 CSV 格式的文件存储到用户指定的存储桶中，详情请参见 <a href="https://cloud.tencent.com/document/product/436/33703">清单功能概述</a></td>
   </tr>
   <tr>
      <td nowrap="nowrap">存储桶标签</td>
      <td>存储桶标签可以作为管理存储桶的一个标识，便于用户对存储桶进行分组管理。用户可以对指定的存储桶进行标签的设定、查询和删除操作，详情请参见 <a href="https://cloud.tencent.com/document/product/436/34834">存储桶标签概述</a></td>
   </tr>
   <tr>
      <td>事件通知</td>
      <td>COS 结合云函数 SCF（Serverless Cloud Function）实现当 COS 资源发生变动（例如新文件上传、文件删除）时，用户可以及时接收通知消息，详情请参见 <a href="https://cloud.tencent.com/document/product/436/35526">事件通知</a></td>
   </tr>
   <tr>
      <td>监控与告警</td>
      <td>对象存储 COS 的读写请求量、流量等数据是基于 <a href="https://cloud.tencent.com/doc/product/248">云监控</a> 来进行统计和展示的。用户可以在云监控的 <a href="https://console.cloud.tencent.com/monitor/product/COS">控制台</a> 查看到 COS 的读写请求量、流量等详细的监控数据，详情请参见 <a href="https://cloud.tencent.com/document/product/436/31903">监控与告警</a></td>
   </tr>
   <tr>
      <td rowspan=2>异地容灾</td>
      <td>版本控制</td>
      <td>版本控制用于实现在相同存储桶中存放同一对象的多个版本。用户在为某一存储桶开启版本控制功能后，可以根据版本 ID 检索、删除或还原存放在存储桶中的对象。这有助于恢复被用户误删或应用程序故障而丢失的数据，详情请参见 <a href="https://cloud.tencent.com/document/product/436/19883">版本控制概述</a></td>
   </tr>
   <tr>
      <td nowrap="nowrap">跨地域复制</td>
      <td>用户可以通过配置跨地域复制规则，在不同存储地域的存储桶中自动、异步地复制增量对象，实现数据的异地容灾与备份，详情请参见 <a href="https://cloud.tencent.com/document/product/436/19237">跨地域复制概述</a></td>
   </tr>
   <tr>
      <td rowspan=2>数据安全</td>
      <td>加密</td>
      <td>对象存储 COS 在数据写入数据中心内的磁盘之前，支持在对象级别上应用数据加密的保护策略，并在访问数据时自动解密，详情请参见 <a href="https://cloud.tencent.com/document/product/436/18145">服务端加密概述</a></td>
   </tr>
   <tr>
      <td>防盗链</td>
      <td>对象存储 COS 支持防盗链配置，用户可以通过控制台的防盗链功能配置黑/白名单，对数据资源进行安全防护，详情请参见  <a href="https://cloud.tencent.com/document/product/436/6226">防盗链实践</a></td>
   </tr>
   <tr>
      <td rowspan=4>访问管理</td>
      <td>跨域访问</td>
      <td>COS 提供 HTML5 标准中的跨域访问设置，帮助实现跨域访问。针对跨域访问，COS 支持响应 OPTIONS 请求，并根据开发者设定的规则向浏览器返回具体设置的规则，具体操作请参见 <a href="https://cloud.tencent.com/document/product/436/13318">设置跨域访问</a></td>
   </tr>
   <tr>
      <td>存储桶策略</td>
      <td>用户可以为存储桶添加策略，可实现允许或禁止某个账号、某个来源 IP（或 IP 段）访问 COS 资源，具体操作请参见 <a href="https://cloud.tencent.com/document/product/436/33369">添加存储桶策略</a></td>
   </tr>
   <tr>
      <td>访问控制</td>
      <td>用户可以对存储桶和对象的访问权限进行管理，当收到某个资源的请求时，COS 将检查相应的 ACL 以验证请求者是否拥有所需的访问权限，详情请参见 <a href="https://cloud.tencent.com/document/product/436/30749">访问控制基本概念</a> 和 <a href="https://cloud.tencent.com/document/product/436/11714">授权子账号访问 COS</a> </td>
   </tr>
   <tr>
      <td>CDN 加速</td>
      <td>COS 结合 CDN 加速服务，可将存储桶中的内容进行大范围的下载、分发，特别适用于相同内容反复下载的使用场景，详情请参见 <a href="https://cloud.tencent.com/document/product/436/18669">CDN 加速概述</a></td>
   </tr>
   <tr>
      <td>工具</td>
      <td nowrap="nowrap">多种管理工具</td>
      <td>COS 提供 COSBrowser、COSCMD、COS Migration 等多种实用工具，可方便用户进行数据管理或数据迁移，详情请参见 <a href="https://cloud.tencent.com/document/product/436/6242">工具概览</a></td>
   </tr>
   <tr>
      <td>API/SDK</td>
      <td nowrap="nowrap">多种开发语言</td>
      <td>COS 提供多种开发语言：Andriod、C、C++、C#、Go、iOS、Java、JavaScript、Node.js、PHP、Python、小程序 SDK，详情请参见 <a href="https://cloud.tencent.com/document/product/436/6474">SDK 概览</a></td>
   </tr>
</table>