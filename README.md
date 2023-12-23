此程序首先是通过8684爬取公交路线名，然后用名称向高德开发平台请求关键字搜索服务，获取详细信息（如：站点信息，坐标，运行时间等），最后在地图上输出一条线路的路线图网上有很多类似的博客教程，但都过时了目前一个都运行不了
秉承着互联网的分享精神（我自己也是在网上找找改改代码的）所以我通过写博客分享出去

test文件为爬取主程序，爬取的线路名会生成data_（city）.txt 我放了一个济南的提供参考，程序自带一个检查是否有重复文件的判断，不建议忽略该功能。取会导致重复数据固定在txt里，另外！8684爬取到的信息不完全准确，请注意

注意事项：无论是8684网站抓取的关键字、还是高德开发平台的url都有更新的可能，不保证永远可用，如果无法运行优先是否是以上问题高德开发平台个人认证者每日请求的配额少得可怜，我为了能一次获取一个城市数据，找了12个人帮我申请key，同时调用这12个key，为了保护他人隐私我将这12个key删除了，自己申请key写进去吧，在111行mykey    （（其实用这个办法获取城市全部的公交信息本身就不现实，我自己实在是没回头路了，才想出用12个人的key的昏招））

生成的公交详细信息保存在城市公交路线.csv 我放了一个济南的提供参考

最后map.py是生成路径图的，同理需要高德开发平台的key（我把我自己的key留在上面了，应该可以直接运行测试），生成在map文件夹（自己在根目录新建一个文件夹） ）里的http文件，不知道为什么打开很慢需要挂梯子（同上放了一个参考文件）

另外：get_line(7).py文件是一个包含了pyqt界面的集合代码，毕竟我做这个的初衷是为了课程设计，界面及搜索等功能设计的很简陋（仅支持模糊搜索）。我没时间做到了，外加这不是我负责的内容懒得弄了有兴趣的可以自己完善一下，爬取部分的代码与之前一致，仅暴力整合进去了而已。没有兴趣的下载，用test.py即可

个人课设作品，才疏学浅，请多见谅。如需解答联系：wang.aoze.mail@gmail.com

The following is a Chinese machine translation, please understand：


This program first crawls the bus route name through 8684, then requests keyword search services from the Gaode development platform using the name to obtain detailed information (such as station information, coordinates, running time, etc.), and finally outputs a route map of a route on the map. There are many similar blog tutorials online, but they are outdated and currently none can run
Adhering to the spirit of sharing on the Internet (I myself also search for code changes online), I share them through writing a blog
The test file is used to crawl the main program, and the crawled circuit names will generate data_ I have provided a reference for Jinan in (city). txt, and the program comes with a check for duplicate files. It is not recommended to ignore this function. Fetching will cause duplicate data to be fixed in txt, and also! The information crawled by 8684 is not entirely accurate, please note
Attention: Whether it is the keywords crawled by the 8684 website or the URLs of the Gaode development platform, there is a possibility of updating, and it is not guaranteed to be always available. If it cannot be run, priority should be given to the above issues. The daily quota requested by the Gaode development platform's individual authenticators is pitifully low. In order to obtain city data at once, I asked 12 people to help me apply for keys and call these 12 keys at the same time, In order to protect the privacy of others, I have deleted these 12 keys and applied for them myself. Please write in the mykey on line 111. (Actually, it is not practical to use this method to obtain all the public transportation information in the city. I really have no way back, so I came up with a trick to use the keys of 12 people.)
The generated bus details are saved in the city bus route. csv, and I have provided a reference for Jinan
Finally, map. py is used to generate a path map. Similarly, it requires a key from the Gaode development platform (I left my own key on it, so I should be able to run tests directly), and an HTTP file is generated in the map folder (create a new folder in the root directory). I don't know why opening it is slow and requires hanging a ladder I as mentioned above, a reference file is also included （To English readers: Hanging a ladder refers to climbing over a wall to the outside internet in China, and you probably don't need to do this）
Additionally: get_ The line (7). py file is a collection of code that includes the pyqt interface. After all, my original intention for doing this was for course design, and the interface and search functions were designed very rudimentary (only supporting fuzzy search). I don't have time to do it, and I'm too lazy to handle the content that's not my responsibility. If you're interested, you can improve it yourself. The crawling part of the code is the same as before, it's just a violent integration. If you are not interested in downloading, just use test.py
I apologize for my lack of knowledge and talent in my personal course design. For answers, please contact: wang.aoze.mail@gmail.com
