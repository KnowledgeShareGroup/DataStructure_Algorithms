# DataStructure_Algorithms
Introduction of Data Structure and basic Algorithms

## 数据格式
数据结构要在网络或保存到文件，就必须对其编码和解码；目前存在很多编码格式：JSON，XML，gob，Google缓冲协议等等。Go语言支持所有这些编码格式；在后面的章节，我们将讨论前三种格式。
结构可能包含二进制数据，如果将其作为文本打印，那么可读性是很差的。另外结构内部可能包含匿名字段，而不清楚数据的用意。
通过把数据转换纯文本，使用命名的字段来标注，让其具有可读性。这样的数据格式可以通过网络传输，而且是与操作平台，任何类型的应用都能够读取和输出，不与操作系统和编程语言的类型相关。

**下面是一些术语说明**：
- [1]数据结构 --> 指定格式 = 序列化 Serialization 或 编码 Encoding (传输之前)
- [2]指定格式 --> 数据结构 = 反序列化 Deserialization 或 Decoding (传输之后)  

### JSON数据格式
```
{
    "Person": {
        "FirstName": "Laura",
        "LastName": "Lynn"
    }
}
```
