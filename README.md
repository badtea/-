# -
开发中遇到的辣鸡奇葩问题。脑子怕记不住。放网上

跟以后的自己说：没时间整理了，爱看不看

1.遇到一个很操蛋的问题，drawerlayout+navController，fragment不能复用。重复oncreate。是个很弱智的东西，该问题导致NavigationView点击菜单切换fragment每次都会重新创建fragment，走oncreate
问了个相同问题的https://stackoverflow.com/questions/67157734/jetpack-navigation-drawer-always-recreate-fragment
这个问题可以解决，但是会严重增加代码，以及逻辑复杂性，还不如用回以前的方法切换fragment
2.使用navigationView.setupWithNavController，会导致navigationView.setNavigationItemSelectedListener回调失效。跟navigationView是否在drawerlayout最下面没有关系。总得来说目前jetpack navigation组件是一个很烂的玩意   2021 05.10
