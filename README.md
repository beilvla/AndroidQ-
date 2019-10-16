# AndroidQ-
关于AndroidQ获取文件路径适配方案向下兼容

//uri获取绝对路径
String path=ImagePathUtil.getFilePathFromURI(context,uri);

//uri获取文件(使用上面的方法)
File file = new File(ImagePathUtil.getFilePathFromURI(context,uri));

有更好的方法或者想法请提出意见，大家一起进步
