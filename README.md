# whatweb-plus
whatweb bug 修复及功能增强 

使用说明:

痛点重谈-Web指纹识别与解决方案

https://mp.weixin.qq.com/s/lHIJmIWbm8ylK6yjjmmNkg

Whatweb-NOVASEC超级增强版介绍：

缺陷1：特征标记【已完善】

whatweb作为一个知名度较高的开源指纹识别工具，其请求头中拥有特定的标志。需要进行修改，使其默认支持动态的请求方式。

缺陷2：运行环境【已完善】

whatweb是使用ruby开发的指纹识别工具，在国内基本Windows的情况下，很少用拥有ruby环境的工程师。因此需要将其封装为一个可执行的文件。

增强1：功能增强【已完善】

在识别特征的方式中提到，目前的部分指纹识别工具也支持mmh3 hash。而whatweb本身仅支持md5的方式，我对其修改实现了mmh3 hash识别方式。

使用方式和md5规则完全一样，会添加:md5规则，就会添加:mmh3规则。

增强2：功能修复【已完善】

另外,测试过程中发现github上最新版的whatweb0.55有bug，

md5值计算出来与实际的md5值不同，对此也进行了修复。

增强3：指纹库增强【已完善】

指纹识别的核心是特征库，只有足够的特征才能满足渗透工作中的日常所需。因此除了whatweb自带的指纹以外，我基本覆盖了所有公开指纹库，转换为指纹识别工具的指纹库，并对所有同名插件，进行了合并处理，对相似名称插件进行了初步分析和合并

【目前全部指纹库5000+】

主要合并了以下工具的指纹库：

    tidesec所有指纹-已合并

    wappalyzer指纹-已合并

    Ehole+Finger+Fscan+glass红队指纹-已合并

    WAF指纹识别规则-已合并



