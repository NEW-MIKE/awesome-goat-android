JDK问题是每一个刚接触JAVA的童鞋需要解决的问题，在学习别人的项目的过程中，正确的认知JDK减少我们遇到的问题。   

IDEA 调整自身JDK：ctrl+shift+a -> Switch Boot JDK ->choose version ……      
而JDK则在 Java1.0 到 Java9 对应每一个版本号 ：JDK1.0、JDK1.2 ... JDK1.8、JDK1.9，Java10以后JDK对应名称为：JDk10、JDK11、JDK12      

场景：在github上面通过git下载工程，导入到IDEA中:    
1,导入的工程不支持java11，因为使用了gradle4.6    
2，设置IDEA runtime java1.8 结果出现了不能识别其java的错误。    

根据这些信息进行推测，单独在环境里面配置，是不行的，一定要到IDEA的本地目录上去改动，或者直接替换掉。     

换做了原生是java1.8的android studio ，

总结：操作系统的环境变量，IDE自带的编译器版本，别人项目对于新版的不兼容，是会导致这一类问题，    
对以后的建议：出现了问题，将问题进行立项，做到一个问题只解决一次。    

