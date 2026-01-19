# KPAH MOD - Build Guide

## Yêu cầu

- **Java JDK 1.8**: Java 11 trở lên
- **Ant**: Build automation tool plugin
- **ProGuard**: Có sẵn trong thư mục `tools/`
- **Intellij IDE**

## Cấu hình build.xml

Cập nhật các đường dẫn sau trong `build.xml` theo máy của bạn:

```xml
<property name="jdk.home" value="C:\đường\đến\jdk\jre (Java 8)"/>
```

## Build

###
- Bấm nút build bên phải phía trên cùng của IDE là nó tự chạy hết các quy trình, muốn obuscate thì chạy thêm target obfuscate là xong !


## Output Files

- `build/bin/KPAH_MOD.jar` - JAR chưa obfuscate
- `build/dist/KPAH_MOD_obf.jar` - JAR final (obfuscated)

## Ghi chú

- ProGuard sẽ obfuscate code, giảm kích thước file
- JAR sẽ chứa resources từ thư mục `res/`
- Manifest được load từ `app/res/META-INF/MANIFEST.MF`
