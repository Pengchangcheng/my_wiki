# 抓取bing首页图片
```python
# -*- coding=utf-8 -*-

import datetime
import os
import re
from urllib import parse

import requests


def crawl_pic(file):
    # base url
    url = 'https://cn.bing.com'
    # 请求头
    headers = {
        'User-Agent': 'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_1) '
                      'AppleWebKit/605.1.15 (KHTML, like Gecko) Version/13.0.3 Safari/605.1.15'
    }

    r = requests.get(url=url, headers=headers)
    # 正则查找
    a = re.findall(r'id="bgLink" rel="preload" href="(.*?)" as="image"', r.text)
    if a:
        picture_url = parse.urljoin(url, a[0])
        print(f'当前图片地址：{picture_url}')
        r_picture = requests.get(url=picture_url, headers=headers)
        write_file(file, r_picture.content)

# 写入文件
def write_file(file, content):
    with open(file, 'wb') as f:
        f.write(content)


if __name__ == '__main__':
    path = 'D:/bing/'
    # 判断文件夹
    if not os.path.exists(path):
        os.mkdir(path)

    today = datetime.date.today()
    path += f'{today}.jpg'
    crawl_pic(path)
```
</br>

[参考](https://mp.weixin.qq.com/s/GiiHMvw651EJ-KnsLgZW2w)