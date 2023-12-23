此程序首先是通过8684爬取公交路线名，然后用名称向高德开发平台请求关键字搜索服务，获取详细信息（如：站点信息，坐标，运行时间等），最后在地图上输出一条线路的路线图网上有很多类似的博客教程，但都过时了目前一个都运行不了

test文件为爬取主程序，爬取的线路名会生成data_（city）.txt 我放了一个济南的提供参考，程序自带一个检查是否有重复文件的判断，不建议忽略该功能。取会导致重复数据固定在txt里，另外！8684爬取到的信息不完全准确，请注意

注意事项：无论是8684网站抓取的关键字、还是高德开发平台的url都有更新的可能，不保证永远可用，如果无法运行优先是否是以上问题高德开发平台个人认证者每日请求的损耗少得可怜，我为了能一次获取一个城市数据，找了12个人帮我申请key，同时调用这12个我将key删除了，自己申请key写进去，在111行

生成的公交详细信息保存在城市公交路线.csv 我放了一个济南的提供参考

最后map.py是生成路径图的，同理需要高德开发平台的key（我把我自己的key留在上面了，应该可以直接运行测试），生成在map文件夹（自己在根目录新建一个文件夹） ）里的http文件，不知道为什么打开很慢需要挂梯子（同上放了一个参考文件）

另外：get_line(7).py文件是一个包含了pyqt界面的集合代码，毕竟我做这个的初衷是为了课程设计，界面及搜索等功能设计的很简陋（仅支持模糊搜索）。我没时间做到了，外加这不是我负责的内容懒得弄了有兴趣的可以自己完善一下，爬取部分的代码与之前一致，仅暴力整合进去了而已。没有兴趣的下载，用test.py即可

个人课设作品，才疏学浅，请多见谅。如需解答联系：wang.aoze.mail@gmail.com

The following is a Chinese machine translation, please understand：


This program first crawls the bus route name through 8684, then requests keyword search services from Gaode development platform using the name to obtain detailed information (such as station information, coordinates, running time, etc.), and finally outputs a route map of a route on the map. There are many similar blogger tutorials online, but they are outdated and currently none can run
The test file is used to crawl the main program, and the crawled circuit names will generate data_ City.txt. I have provided a reference for Jinan, and the program comes with a check for duplicate files. It is not recommended to ignore this function. Fetching will cause duplicate data to be fixed in txt, and also! The information crawled by 8684 is not entirely accurate, please note
Attention: Whether it is the keywords crawled by the 8684 website or the URLs of Gaode development platform, there is a possibility of updating, and it is not guaranteed to be always available. If it cannot be run, priority should be given to whether it is the above problem. The daily loss requested by Gaode development platform personal authenticators is pitifully low. In order to obtain data from one city at a time, I asked 12 people to help me apply for keys, and at the same time, I deleted these 12 keys. I applied for keys myself and wrote them in line 111
The generated bus details are saved in the city bus route. csv, and I have provided a reference for Jinan
Finally, map. py is used to generate a path map. Similarly, it requires Gaode development platform ’s key (I left my own key on it, so I should be able to run the test directly) and generate an HTTP file in the map folder (create a new folder in the root directory). I don't know why opening it is slow and requires hanging a ladder (as mentioned above, a reference file is also included)
Additionally: get_ The line (7). py file is a collection of code that includes the pyqt interface. After all, my original intention for doing this was to design the course, interface, and search functions very rudimentary (only supporting fuzzy search). I don't have time to do it, and I'm too lazy to handle the content that's not my responsibility. If you're interested, you can improve it yourself. The crawling part of the code is the same as before, it's just a violent integration. If you are not interested in downloading, just use test.py

I apologize for my lack of knowledge and talent in my personal course design. If you need answers contact ：wang.aoze.mail@gmail.com
