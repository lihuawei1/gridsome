创建 Gridsome 静态网站项目步骤

1.npm install --global @gridsome/cli

2.gridsome create my-gridsome-site//这样很难成功，因为gridsome依赖一个第三方库sharp，sharp是一个处理图片的插件（压缩图片，转换格式）很难安装，有c++文件，依赖libvips

3.解决安装sharp，在githup  sharp仓库中，点击sharp.pixelplumbing.com，在install中找到Chinese mirror 

4.安装 npm config set sharp_binary_host "https://npm.taobao.org/mirrors/sharp"
npm config set sharp_libvips_binary_host "https://npm.taobao.org/mirrors/sharp-libvips"

5.解决c++环境变量问题，在githup  node-gyp仓库中 ,npm install -g node-gyp,安装完以后不能直接使用，不同的平台需要不同的环境 所有平台都需要安装python 

6.gridsome create my-gridsome-site创建项目

Gridsome 中 #GraphQL查询集合中的数据
 http://localhost:8081/___explore

# query{
#   post(id:1){
#     id
#     title
#   }
# }
查询一条
# query{ 
# allPost{
#   edges{
#     node{
#       id
#       title
#     }
#   }
# }
# }
查询全部



git clone *** --depth=1 下载最新版本
strapi  是一个通用的内容管理系统，管理博客，用户，用户评论



https://vercel.com/login  //部署的服务器平台，傻瓜操作


