# Typora PicGO 配置
<br>

```shell
偏好设置->图象:  
    选择: 插入图片时->上传图片
    选中: 1.对本地位置的图片应用上述操作
          2.对网络位置的图片应用上述操作
```    
<br><br><br>   
      
## windows
```
上传服务->PicGo(app)
路径    ->直接选中PicGo.exe
```
<br><br><br>




## Linux
```
选择: PicGo-Core(command line)
点击  "下载或更新"
```

```
[注意：github  默认使用 githubPlus插件]
```
<br><br>






#### 配置PicGo

```
cd /home/用户名/.config/Typora/picgo/linux
```

```
picgo set uploader
```


```
repo : 用户名/仓库名
brach : 分支名(一般是main或master)
token :
path : 放图片的文件夹名/
customUrl : https://cdn.jsdelivr.net/gh/用户名/仓库名
origin ：github
```

```
picgo use uploader
```

<br/><br>
**配置文件模板**
<br>

```
{
  "picBed": {
    "current": "github",
    "github": {
      "repo": "用户名/仓库名",
      "branch": "main",
      "token": "",
      "path": "放图片的文件夹名/",
      "customUrl": "https://cdn.jsdelivr.net/gh/用户名/仓库名"
    },
    "uploader": "github",
    "transformer": "path"
  },
  "picgoPlugins": {
    "picgo-plugin-github-plus": true
  }
}
```

**Github Token获取**
```
个人头像 -> Settings -> Developer settings -> Personal access tokens -> 
Generate a personal access token -> 设置名字和权限 -> 复制Token
```

