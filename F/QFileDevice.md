
# **QFileDevice Class**

----------

## **QFileDevice 类提供了读写文件的接口**

|  属性  | 方法|
|------:|:------|
|头文件:|\#include \<QFileDevice>|
|qmake参数：|QT += core|
|引入:|Qt 5.0|
|继承:    |QIODevice|
|派生:| QFile 和 QSaveFile      |

----------

该类在 Qt 5.0 中引入。

**注：**该类的所有方法都是可重入的。

## **简述**

----------
### **公共类型**

|  类型  | 方法|
|------:|:------|
|enum|**[FileError](https://doc.qt.io/qt-5/qfiledevice.html#FileError-enum)** { NoError, ReadError, WriteError, FatalError, ResourceError, …, CopyError }|
|enum|**[FileHandleFlag](https://doc.qt.io/qt-5/qfiledevice.html#FileHandleFlag-enum)** { AutoCloseHandle, DontCloseHandle }|
|flags|**[FileHandleFlags](https://doc.qt.io/qt-5/qfiledevice.html#FileHandleFlag-enum)**|
|enum|**[FileTime](https://doc.qt.io/qt-5/qfiledevice.html#FileTime-enum)** { FileAccessTime, FileBirthTime, FileMetadataChangeTime, FileModificationTime }|
|enum|**[MemoryMapFlags](https://doc.qt.io/qt-5/qfiledevice.html#MemoryMapFlags-enum)** { NoOptions, MapPrivateOption }|
|enum|**[Permission](https://doc.qt.io/qt-5/qfiledevice.html#Permission-enum)** { ReadOwner, WriteOwner, ExeOwner, ReadUser, WriteUser, …, ExeOther }|
|flags|**[Permissions](https://doc.qt.io/qt-5/qfiledevice.html#Permission-enum)**|

----------


### **重写公共函数**
|  函数名  | 类型|
|------:|:------|
| virtual bool | **[atEnd](https://doc.qt.io/qt-5/qfiledevice.html#atEnd)**() const override |
|virtual void |**[close](https://doc.qt.io/qt-5/qfiledevice.html#close)**() override|
|virtual bool |**[isSequential](https://doc.qt.io/qt-5/qfiledevice.html#isSequential)**() const override|
|virtual qint64 |**[pos](https://doc.qt.io/qt-5/qfiledevice.html#pos)**() const override|
|virtual bool |**[seek](https://doc.qt.io/qt-5/qfiledevice.html#seek)**(qint64 *pos*) override|
|virtual qint64 |**[size](https://doc.qt.io/qt-5/qfiledevice.html#size)**() const override|

----------

### **重写保护函数**

|         函数名 | 类型                                                         |
| -------------: | :----------------------------------------------------------- |
| virtual qint64 | **[readData](https://doc.qt.io/qt-5/qfiledevice.html#readData)**(char **data*, qint64 *len*) override |
| virtual qint64 | **[readLineData](https://doc.qt.io/qt-5/qfiledevice.html#readLineData)**(char **data*, qint64 *maxlen*) override |
| virtual qint64 | **[writeData](https://doc.qt.io/qt-5/qfiledevice.html#writeData)**(const char **data*, qint64 *len*) override |

### **公共成员函数**

|  类型  | 函数名|
|------:|:------|
| virual |**[~QFileDevice](https://doc.qt.io/qt-5/qfiledevice.html#dtor.QFileDevice)**()|
|QFileDevice::FileError |**[error](https://doc.qt.io/qt-5/qfiledevice.html#error)**() const|
|virtual QString |**[fileName](https://doc.qt.io/qt-5/qfiledevice.html#fileName)**() const|
|QDateTime |**[fileTime](https://doc.qt.io/qt-5/qfiledevice.html#fileTime)**(QFileDevice::FileTime *time*) const|
|bool |**[flush](https://doc.qt.io/qt-5/qfiledevice.html#flush)**()|
|int |**[handle](https://doc.qt.io/qt-5/qfiledevice.html#handle)**() const|
|uchar * |**[map](https://doc.qt.io/qt-5/qfiledevice.html#map)**(qint64 *offset*, qint64 *size*, QFileDevice::MemoryMapFlags *flags* = NoOptions)|
|virtual QFileDevice::Permissions |**[permissions](https://doc.qt.io/qt-5/qfiledevice.html#permissions)**() const|
|virtual bool |**[resize](https://doc.qt.io/qt-5/qfiledevice.html#resize)**(qint64 *sz*)|
|bool |**[setFileTime](https://doc.qt.io/qt-5/qfiledevice.html#setFileTime)**(const QDateTime &*newDate*, QFileDevice::FileTime *fileTime*)|
|virtual bool |**[setPermissions](https://doc.qt.io/qt-5/qfiledevice.html#setPermissions)**(QFileDevice::Permissions *permissions*)|
|bool |**[unmap](https://doc.qt.io/qt-5/qfiledevice.html#unmap)**(uchar **address*)|
|void |**[unsetError](https://doc.qt.io/qt-5/qfiledevice.html#unsetError)**()|

## **详细说明**

----------

`QFileDevice`是`I/O`设备相关的基类，可以读写文本或二进制类型的文件和资源。`QFile`提供了主要的功能，`QFileDevice`则作为基类与其他文件设备，如`QTempFile`，共享方法，用于操作`QFile`或`QTemporaryFile`打开的文件。

您也可以在 [QFile](https://doc.qt.io/qt-5/qfile.html) 和 [QTemporaryFile](https://doc.qt.io/qt-5/qtemporaryfile.html) 类中找到相关信息。

----------

## **成员类型文档**

###  **enum QFileDevice::FileError**

----------

枚举`error()`方法返回的错误类型。

| 常量                          | 值   | 描述                                   |
| ----------------------------- | ---- | -------------------------------------- |
| QFileDevice::NoError          | 0    | 无错误                                 |
| QFileDevice::ReadError        | 1    | 读文件错误                             |
| QFileDevice::WriteError       | 2    | 写文件错误                             |
| QFileDevice::FatalError       | 3    | 严重错误                               |
| QFileDevice::ResourceError    | 4    | 资源不足（打开的文件过多，内存耗尽等） |
| QFileDevice::OpenError        | 5    | 无法打开文件                           |
| QFileDevice::AbortError       | 6    | 操作中止                               |
| QFileDevice::TimeOutError     | 7    | 超时                                   |
| QFileDevice::UnspecifiedError | 8    | 未知错误                               |
| QFileDevice::RemoveError      | 9    | 文件无法移除                           |
| QFileDevice::RenameError      | 10   | 文件无法重命名                         |
| QFileDevice::PositionError    | 11   | 无法修改文件中的位置                   |
| QFileDevice::ResizeError      | 12   | 无法调整文件大小                       |
| QFileDevice::PermissionsError | 13   | 文件无法访问                           |
| QFileDevice::CopyError        | 14   | 文件无法复制                           |

### **enum QFileDevice::FileHandleFlag  / flags QFileDevice::FileHandleFlags**

----------

枚举了打开文件时特定的附加选项，仅用于文件类操作，而非基类 QIODevice。

| 常量                         | 值    | 描述                                                         |
| ---------------------------- | ----- | ------------------------------------------------------------ |
| QFileDevice::AutoCloseHandle | 0x001 | 传入 [`open()`](https://doc.qt.io/qt-5/qiodevice.html#open)的文件句柄应该被[`close()`](https://doc.qt.io/qt-5/qfiledevice.html#close)关闭，默认行为关闭只刷新缓存，然后由 Qt 应用负责关闭文件句柄。当以文件名打开时，由于Qt总是拥有文件句柄并且必须关闭它，该标志会被忽略。 |
| QFileDevice::DontCloseHandle | 0     | 如果未显式关闭，则在销毁`QFile`对象时，潜在的文件句柄将保持打开状态。 |

FileHandleFlags 类型由 QFlags\<FileHandleFlag> 定义。存储了 FileHandleFlag 值的`或`运算结果。

### **enum QFileDevice::FileTime**

----------

该枚举用于函数 [fileTime()](https://doc.qt.io/qt-5/qfiledevice.html#fileTime) 和 [setFileTime()](https://doc.qt.io/qt-5/qfiledevice.html#setFileTime)。

| 常量                                | 值   | 描述                              |
| ----------------------------------- | ---- | --------------------------------- |
| QFileDevice::FileAccessTime         | 0    | 文件最近访问时间（读或者写）      |
| QFileDevice::FileBirthTime          | 1    | 文件创建时间（Unix 上可能不支持） |
| QFileDevice::FileMetadataChangeTime | 2    | 文件元数据最后更改时间            |
| QFileDevice::FileModificationTime   | 3    | 文件最近修改时间                  |

该枚举在 Qt 5.10 中被引进或修改。

您也可以在 [setFileTime()](https://doc.qt.io/qt-5/qfiledevice.html#setFileTime（）)， [fileTime()](https://doc.qt.io/qt-5/qfiledevice.html#fileTime) 和 [QFileInfo::fileTime()](https://doc.qt.io/qt-5/qfileinfo.html#fileTime) 函数中找到相关信息。

### **enum QFileDevice::MemoryMapFlags**

----------

用于函数 [map()](https://doc.qt.io/qt-5/qfiledevice.html#map) 的特定枚举类型选项。

| 常量                          | 值     | 描述                                                         |
| ----------------------------- | ------ | ------------------------------------------------------------ |
| QFileDevice::NoOptions        | 0      | 无选项                                                       |
| QFileDevice::MapPrivateOption | 0x0001 | 映射的内存是私有的，因此任何修改对于其他进程不可见且不会写入磁盘。内存断开映射时所有的修改将会丢失。未明确在创建映射后对文件所做的修改是否通过映射内存可见。该值在 Qt 5.4 中引入 |

该枚举在 Qt 4.4 中引入。

### **enum QFileDevice::Permission / flags QFileDevice::Permissions**

----------

用于函数 permission() 来报告文件的权限和所有权。这些值可以用`或`运算连接以测试复合的权限和所有权。

| 常量                    | 值     | 描述                   |
| ----------------------- | ------ | ---------------------- |
| QFileDevice::ReadOwner  | 0x4000 | 文件所有者对文件可读   |
| QFileDevice::WriteOwner | 0x2000 | 文件所有者对文件可写   |
| QFileDevice::ExeOwner   | 0x1000 | 文件所有者对文件可执行 |
| QFileDevice::ReadUser   | 0x0400 | 用户对文件可读         |
| QFileDevice::WriteUser  | 0x0200 | 用户对文件可写         |
| QFileDevice::ExeUser    | 0x0100 | 用户对文件可执行       |
| QFileDevice::ReadGroup  | 0x0040 | 用户组对文件可读       |
| QFileDevice::WriteGroup | 0x0020 | 用户组对文件可写       |
| QFileDevice::ExeGroup   | 0x0010 | 用户组对文件可执行     |
| QFileDevice::ReadOther  | 0x0004 | 所有用户对文件可读     |
| QFileDevice::WriteOther | 0x0002 | 所有用户对文件可写     |
| QFileDevice::ExeOther   | 0x0001 | 所有用户对文件可执行   |

**注意：**由于 Qt 所支持的平台不同，可读用户，可写用户和可执行用户的语义与平台有关：在 Unix 系统中，返回文件所有者的权限，而 Windows 系统上则返回当前用户的权限。此行为可能会在将来的 Qt 版本中更改。

**注：**在 NTFS 文件系统上，出于性能原因，所有权和权限的检查被默认关闭。要打开它，可以包含以下代码行：

```c
extern Q_CORE_EXPORT int qt_ntfs_permission_lookup;
```

然后权限检查可以通过递增和递减`qt_ntfs_permission_lookup`来打开和关闭。

```c
qt_ntfs_permission_lookup++; // 打开检查
qt_ntfs_permission_lookup--; // 关闭检查
```

Permission 类型由 QFlags\<Permission> 定义。存储了 Permission 值的`或`运算结合。

## **成员函数文档**



### QFileDevice::~QFileDevice()	[virtual]

----------

销毁文件设备，如有必要，将文件关闭。

### bool QFileDevice::atEnd() const	[override virtual]

----------

重写了父类方法 [QIODevice::atEnd](https://doc.qt.io/qt-5/qiodevice.html#atEnd)() const

如果到达文件末尾返回`true`，否则返回`false`。

对于 Unix 上常规的空文件（如 /proc 下的文件），由于文件系统报告文件的大小为`0`，所以该方法返回`true`。因此从这种文件读取数据时你不能依赖`atEnd()`方法，而要通过调用`call()`直到没有数据可读。

### void QFileDevice::close()	[override virtual]

----------

重新实现：[QIODevice::close](https://doc.qt.io/qt-5/qiodevice.html#close)()

调用 [QFileDevice::flush](https://doc.qt.io/qt-5/qfiledevice.html#flush)() 并关闭文件。忽略刷新时返回的错误。

您也可以在 [QIODevice::close](https://doc.qt.io/qt-5/qiodevice.html#close)() 中找到相关信息。

### [QFileDevice::FileError](https://doc.qt.io/qt-5/qfiledevice.html#FileError-enum) QFileDevice::error() const 	

----------

返回错误状态。

I/O设备状态返回错误码。例如， [`open()`](https://doc.qt.io/qt-5/qiodevice.html#open)返回`false`，读写操作返回`-1`。调用该函数可以找出文件操作失败的原因。

您也可以在 [unsetError](https://doc.qt.io/qt-5/qfiledevice.html#unsetError)() 找到相关信息。

### [QString](https://doc.qt.io/qt-5/qstring.html) QFileDevice::fileName() const	[virtual]

----------

返回文件名。在 [QFileDevice](https://doc.qt.io/qt-5/qfiledevice.html) 中默认实现是返回空字符串。

### [QDateTime](https://doc.qt.io/qt-5/qdatetime.html) QFileDevice::fileTime([QFileDevice::FileTime](https://doc.qt.io/qt-5/qfiledevice.html#FileTime-enum) *time*) const

----------

返回`time`指定的时间。如果不能确定则返回`QDateTime()` （一个无效时间日期）。

该函数在 Qt 5.10 引入。

您也可以在 [setFileTime](https://doc.qt.io/qt-5/qfiledevice.html#setFileTime)()，[FileTime](https://doc.qt.io/qt-5/qfiledevice.html#FileTime-enum) 和 [QDateTime::isValid](https://doc.qt.io/qt-5/qdatetime.html#isValid)()中找到相关信息。

### bool QFileDevice::flush()

----------

将缓存数据刷新到文件，成功返回`true`，否则返回`false`。

### int QFileDevice::handle() const

----------

返回文件的句柄。

该返回值是一个小的正整数，适用于C标准库函数`fdopen()`和`fcntl()`。在使用文件描述符的系统（ Unix 系统）中，该句柄也可以用于 [QSocketNotifier](https://doc.qt.io/qt-5/qsocketnotifier.html)。

文件未打开或者有错误时返回`-1`。

### bool QFileDevice::isSequential() const	[override virtual]

----------

重写了父类方法：[QIODevice::isSequential](https://doc.qt.io/qt-5/qiodevice.html#isSequential)() const

如果文件只能顺序操作则返回`true`，否则返回`false`。

大部分文件支持随机访问，但是一些特殊文件不支持。

您也可以在 [QIODevice::isSequential](https://doc.qt.io/qt-5/qiodevice.html#isSequential)() 中找到相关信息。

### [uchar](https://doc.qt.io/qt-5/qtglobal.html#uchar-typedef) *QFileDevice::map(qint64 *offset*, qint64 *size*, [QFileDevice::MemoryMapFlags](https://doc.qt.io/qt-5/qfiledevice.html#MemoryMapFlags-enum) *flags* = NoOptions)

------

将文件从`offset`位置开始的`size`个字节映射到内存中。文件在打开后才能成功映射，映射完成后文件则不需要保持打开状态。当 [QFile](https://doc.qt.io/qt-5/qfile.html) 被销毁或者该对象打开新的文件时，所有未断开的映射都将自动断开。

映射的打开模式与文件打开的模式（读/写）保持一致，除非使用 [MapPrivateOption](https://doc.qt.io/qt-5/qfiledevice.html#MemoryMapFlags-enum) 选项，这种情形下对映射的内存总是可写。

通过`flags`传入映射选项。

返回映射内存的地址指针，报错时返回`nullptr`。

您也可以在 [unmap](https://doc.qt.io/qt-5/qfiledevice.html#unmap)() 中找到相关信息。

### [QFileDevice::Permissions](https://doc.qt.io/qt-5/qfiledevice.html#Permission-enum) QFileDevice::permissions() const	[virtual]

------

返回文件完整的 [QFile::Permission](https://doc.qt.io/qt-5/qfiledevice.html#Permission-enum) `或`运算组合。

您也可以在 [setPermissions](https://doc.qt.io/qt-5/qfiledevice.html#setPermissions)() 中找到相关信息。

### [qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) QFileDevice::pos() const	[override virtual]

------

重写了父类方法：[QIODevice::pos](https://doc.qt.io/qt-5/qiodevice.html#pos)() const

### [qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) QFileDevice::readData(char **data*, [qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) *len*)	[override virtual protected]

-----

重写了父类方法：[QIODevice::readData](https://doc.qt.io/qt-5/qiodevice.html#readData)(char *data, qint64 maxSize)*

### *[qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) QFileDevice::readLineData(char **data*, [qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) *maxlen*)	[override virtual protected]

--------

重写了父类方法：[QIODevice::readLineData](https://doc.qt.io/qt-5/qiodevice.html#readLineData)(char *data, qint64 maxSize)

### bool QFileDevice::resize([qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) *sz*)	[virtual]

--------

设置文件大小为`sz`个字节。成功返回`true`，失败返回`false`。如果`sz`大于当前文件大小，新增的字节将被置`0`。如果`sz`小于文件大小，文件则简单地截断。

注意：文件不存在时该函数会失败。

您也可以在 [size](https://doc.qt.io/qt-5/qfiledevice.html#size)() 中找到相关信息。

### bool QFileDevice::seek([qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) *pos*)	[override virtual] 

--------

重写了父类方法：[QIODevice::seek](https://doc.qt.io/qt-5/qiodevice.html#seek)(qint64 pos)

对于随机访问设备，该函数将当前文件位置设置为`pos`，成功则返回`true`，失败返回`false`。对于顺序访问设备，默认行为是不做操作并返回`false`。

寻找位置超出文件末尾：如果位置超出文件末尾，`seek()`不会立即扩展文件。如果在此位置执行写入，则文件将被扩展。在之前文件末尾和新写入地数据之间地内容是未定义的，并且因平台和文件系统而异。

### bool QFileDevice::setFileTime(const [QDateTime](https://doc.qt.io/qt-5/qdatetime.html) &*newDate*, [QFileDevice::FileTime](https://doc.qt.io/qt-5/qfiledevice.html#FileTime-enum) *fileTime*)

--------

依据`fileTime`选项值设置给定的*newDate*，成功返回`true`，否则返回`false`。

注：使用该函数时文件必须被打开。

该函数在 Qt 5.10 引入。

您也可以在 [fileTime](https://doc.qt.io/qt-5/qfiledevice.html#fileTime)() 和  [FileTime](https://doc.qt.io/qt-5/qfiledevice.html#FileTime-enum) 找到相关信息。

### bool QFileDevice::setPermissions([QFileDevice::Permissions](https://doc.qt.io/qt-5/qfiledevice.html#Permission-enum) *permissions*)	[virtual]

--------

为文件设置`permission`指定的权限，成功返回`true`，如果无法修改权限则返回`false`。

注意：此函数不会操纵ACLs，这可能会限制其有效性。

您也可以在 [permissions](https://doc.qt.io/qt-5/qfiledevice.html#permissions)() 中找到相关信息。

### [qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) QFileDevice::size() const	[override virtual]

--------

重写了父类方法：[QIODevice::size](https://doc.qt.io/qt-5/qiodevice.html#size)() const

返回文件大小。

对于 Unix 上的常规空文件（如，/proc 下的文件），该函数返回`0`；这类文件是当你调用`read()`时按需要生成的。

### bool QFileDevice::unmap([uchar](https://doc.qt.io/qt-5/qtglobal.html#uchar-typedef) **address*)

--------

断开地址`address`处的映射.

成功返回`true`，否则返回`false`。

您也可以在 [map](https://doc.qt.io/qt-5/qfiledevice.html#map)() 中找到相关信息。

### void QFileDevice::unsetError()

-------

将文件错误设置为 [QFileDevice::NoError](https://doc.qt.io/qt-5/qfiledevice.html#FileError-enum)。

另外您也可以在 [error](https://doc.qt.io/qt-5/qfiledevice.html#error)() 中找到相关信息。

### [qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) QFileDevice::writeData(const char **data*, [qint64](https://doc.qt.io/qt-5/qtglobal.html#qint64-typedef) *len*)	[override virtual protected]

--------

重写了父类方法：[QIODevice::writeData](https://doc.qt.io/qt-5/qiodevice.html#writeData)(const char *data, qint64 maxSize)

