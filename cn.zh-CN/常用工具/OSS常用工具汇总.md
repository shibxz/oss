# OSS常用工具汇总 {#concept_owg_knn_vdb .concept}

除控制台外，您还可以使用以下常用工具帮助您更高效地使用OSS。

|工具|简介|
|:-|:-|
|[ossbrowser](intl.zh-CN/常用工具/图形化管理工具ossbrowser/快速开始.md#)|图形化的Object管理工具。 -   图形化界面，使用简单。
-   提供类似Windows资源管理器的功能。
-   支持直接浏览文件。
-   支持文件目录（文件夹）的上传下载。
-   支持文件并发上传、断点续传。
-   支持RAM子账号的图形化Policy授权操作。
-   支持Windows、Linux、Mac平台。

 使用限制：

-   ossbrowser是图形化工具，传输速度和性能不如ossutil。
-   只支持5GB以下的文件上传或复制。

 |
|[ossutil](intl.zh-CN/常用工具/命令行工具ossutil/概述.md#)|Object和Bucket的命令行管理工具。 -   提供方便、简洁、丰富的Object和Bucket管理命令，操作性能好。
-   支持文件并发上传、断点续传。
-   支持文件目录（文件夹）的上传下载。
-   支持Bucket常见管理命令。

 |
|[osscmd（已下线）](intl.zh-CN/常用工具/osscmd（已下线）/快速安装.md#)|Object和Bucket的命令行管理工具。 -   提供完备的Bucket、Object管理命令。
-   支持Windows、Linux平台。

 使用限制：

-   仅适用于Python2.5 - 2.7版本，不支持Python 3.x版本。
-   不再支持OSS新增功能，如低频存储/归档存储、跨区域复制、镜像回源等。

 **说明：** osscmd操作命令已整合到[ossutil](intl.zh-CN/常用工具/命令行工具ossutil/概述.md#)中，工具已于2019年7月31日下线，给您带来不便敬请谅解。

 |
|[ossfs](intl.zh-CN/常用工具/ossfs/快速安装.md#)|Bucket挂载工具。 用于将OSS的Bucket挂载到Linux系统的本地文件系统中，挂载后可通过本地文件系统操作OSS上的Object，实现数据的访问和共享。

 -   支持POSIX文件系统的大部分功能，包括文件读写、目录、链接操作、权限、uid/gid、以及扩展属性（extended attributes）。
-   支持使用OSS的multipart功能上传大文件。
-   支持MD5校验，保证数据完整性。

 使用限制： -   不支持挂载归档型Bucket。
-   编辑已上传文件会导致文件被重新上传。
-   元数据操作，例如`list directory`，因为需要远程访问OSS服务器，所以性能较差。
-   重命名文件/文件夹可能会出错。若操作失败，可能会导致数据不一致。
-   不适合高并发读/写的场景。
-   多个客户端挂载同一个OSS Bucket时，数据一致性由您自行维护。例如，合理规划文件使用时间，避免出现多个客户端写同一个文件的情况。
-   不支持hard link。

 |
|[ossftp](intl.zh-CN/常用工具/ossftp/如何快速安装ossftp.md#)|管理Object的FTP工具。 -   使用FileZilla、WinSCP、FlashFXP等FTP客户端操作OSS。
-   本质是FTP Server，用于接收FTP请求，将对文件、文件夹的操作映射为对OSS的操作。
-   基于Python2.7及以上版本。
-   支持Windows、Linux、Mac平台。

 |
|[ossimport](intl.zh-CN/常用工具/数据迁移工具ossimport/说明及配置.md#)|OSS数据同步工具： -   可将各类第三方数据源文件同步到OSS上。
-   支持分布式部署，可使用多台服务器批量迁移数据。
-   支持TB级以上数据迁移。
-   支持Windows、Linux平台。
-   适用于Java 1.7及以上版本。

 |
|[可视化签名工具](https://bbs.aliyun.com/read/233851.html)|可视化签名工具（第三方工具）。 -   可用于生成数据的签名URL。
-   可调试签名中遇到的问题。当您在实现OSS的签名过程中遇到问题，请与该工具的签名对比，以便快速定位该错误。
-   网页版支持浏览器Chrome、Firefox、Safari。

 |
|[RAM Policy Editor](http://gosspublic.alicdn.com/ram-policy-editor/index.html)|OSS授权策略自动化生产工具。 -   可根据填写的需求自动生成授权策略，您可将自动生成的策略移植到RAM访问控制的[自定义权限](https://ram.console.aliyun.com/policies/new)内。
-   支持浏览器Chrome、Firefox、Safari。

 **说明：** 当您需要生成自定义授权策略时，推荐使用该工具。

 |
|[oss-emulator](https://github.com/aliyun/oss-emulator)|轻量级的OSS服务模拟器。 -   提供与OSS服务相同的API接口，适用于基于OSS应用的调试、性能测试等。
-   基于Ruby 2.2.8及以上版本。
-   支持Windows、Linux平台。

 |

