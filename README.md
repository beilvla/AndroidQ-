# AndroidQ
关于AndroidQ获取文件路径适配方案向下兼容
重要的事情说三遍
一定要有权限
一定要有权限
一定要有权限
这两个权限在AndroidQ上会默认转为AndroidQ所需要的权限，也可以用AndroidQ的新的权限（androidQ以下没有试过用androidQ的新权限）
  <uses-permission android:name="android.permission.READ_EXTERNAL_STORAGE" />
  <uses-permission android:name="android.permission.WRITE_EXTERNAL_STORAGE" />
  //（需要拍照时使用）
   <uses-permission android:name="android.permission.CAMERA" />

//uri获取绝对路径
String path=ImagePathUtil.getFilePathFromURI(context,uri);

//uri获取文件(使用上面的方法)
File file = new File(ImagePathUtil.getFilePathFromURI(context,uri));

有更好的方法或者想法请提出意见，大家一起进步
