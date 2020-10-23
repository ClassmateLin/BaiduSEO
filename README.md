# 百度搜索点击脚本免费版

## 免费版说明如下:

- 需要安装chrome浏览器和下载对应版本的chromedriver。
- 百度搜索关键词，支持下拉选择关键词。
- 支持翻页查找, 概率随机点击非指定站点，点进去立马退出。
- 翻页或者浏览进行鼠标移动，页面下拉等操作模拟真实用户。
- 找到指定站点进行浏览下拉，点击内链。

- 使用方法如下:

- 安装好chrome和下载对应版本的chromedriver。

- `pip install -r requirements.txt` 安装项目依赖.

- 代码需要修改关键词列表, 网站域名, chromedriver路径，main.py代码如下:

```python
from search import PcSearch
from browser import Browser


if __name__ == '__main__':
    keys = [    # 定义关键词
        '资源分享',
        'python教程'
    ]
    site = 'fenlanli.com'  # 指定站点
    browser = Browser(driver_path='./chromedriver.exe')  # 定义chromedriver的路径
    app = PcSearch(browser=browser, keys=keys, site=site)
    app.run()
```

- `python main.py` 运行即可。


## 更多资源

请关注个人网站: `https://www.classmatelin.top`
