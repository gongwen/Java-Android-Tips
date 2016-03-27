# Java-Android-Tips

1.[10个实用的但偏执的Java编程技术](http://www.codeceo.com/article/10-useful-paranoid-java-coding.html)

2.[使用泛型方法代替findViewById](http://blog.chengyunfeng.com/?p=541)＜/br＞
  public final <E extends View> E getView(int id) {＜/br＞
        try {＜/br＞
            return (E) findViewById(id);＜/br＞
        }catch (ClassCastException e) {＜/br＞
            throw new ClassCastException(toString());＜/br＞
        }＜/br＞
  }＜/br＞
 
