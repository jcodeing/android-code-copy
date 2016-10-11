# Hot

使用频率较高的代码片段

{% method %}
## 单例-静态内部类

懒加载

{% sample lang="java" %}

```java
// ============================@Static Singleton@============================
private ClassName() {
}

private static class SingletonHolder {
    static final ClassName INSTANCE = new ClassName();
}

/**
 * @return instance
 */
public static ClassName i() {
    return SingletonHolder.INSTANCE;
}
```

{% endmethod %}

{% method %}
## 监听-OnXxListener

{% sample lang="java" %}

```java
// ============================@OnXxListener@============================
public interface OnXxListener {
    void onXx(String str);
}

private OnXxListener onXxListener;

public void setOnXxListener(OnXxListener onXxListener) {
    this.onXxListener = onXxListener;
}
```

{% endmethod %}