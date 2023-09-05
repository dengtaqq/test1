# Vue 3 + Vite
 都建立在2次封装axios上 

//mock  发请求  mockdata 具体请求的数据 
               mock 拦截mock请求 
              api  封装mock请求 

//实际接口  :   一个api文件,里面配置具体文件需要的各类请求      



 #一 项目起步
         1.新建项目.安装node环境,或yarn环境 安装脚手架cli、vite  已经有了的话直接创建项目,
         vite(只能3)需要多一步:安装依赖
      vue -V cli版本监测 
     vue create 项目名 cli创建项目 




          2. 安装引入ui框架 (elementui、) 按照路由router 
            

          3.组件 : components 放置固定组件:Aside.vue(侧边栏)  Header(头部) Tab ..... 
                 views下各个组件 hone一般为默认打开的内容组件 
                 Main组件 为默认主入口
             
          4.路由router : 配置路由  router配置路由走向, 默认主入口Main组件path为'/'里面children也为'/'  
                        默认导出,mian.js引入 use应用
                        router里面就只管配置,main只引入使用,App组件就一个<router-view>
                        mian组件引入各个固定     变化的组件处<router-view>

                        （之后的内容展示就可以侧头不变，然后看路由变化实现中间变了）
             另外的登录页在router配置里起另外一个对象            
#二 搭建页面架子
         侧边栏 用element 经验进行搭建  
              组件对应数据数据跳转实现： 1.定义一个数组里面是路由名，跳转路径等的多个对象
               2.定义2个方法是否有children 方法里遍历list
                      将有children的对象filter过滤出来  返回出去 也就是拿到
               3.用这2个方法拿出的渲染2个el-sub-menu菜单即可实现  
#三 具体页面搭建 
    熟练使用elementui组件搭建， 
     图表用的是 echarts （安装 在具体组件引入）
     icons图标也要安装引入


#四 数据交互基本用法
 获取组件实例对象
 const { proxy } = getCurrentInstance();

 echarts使用  
 1.组件里放div  配置ref 
2.配置图形要的数据 
3.定义方法,用ref拿到 组件对象.setOption(数据) onMounted挂载 


   









                



               
               
              

