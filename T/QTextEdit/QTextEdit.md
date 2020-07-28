
# **QTextEdit Class**

----------

## **QTextEdit 类是用于显示纯文本和富文本的控件。**

|  属性  | 方法|
|------:|:------|
|头文件:|`    include <QTextEdit>`|
|qmake参数:|QT += widgets|
|继承:    |QAbstractScrollArea|
|派生:|[QTextBrowser](https://doc.qt.io/qt-5/qtextbrowser.html)|

----------

## **简述**

----------
### **公共类型**

|  类型  | 值 |
|------:|:------|
|struct|[ExtraSelection](https://doc.qt.io/qt-5/qtextedit-extraselection.html)|
|flags|[AutoFormatting](https://doc.qt.io/qt-5/qtextedit.html#AutoFormattingFlag-enum)|
|enum|**[AutoFormattingFlag](https://doc.qt.io/qt-5/qtextedit.html#AutoFormattingFlag-enum)** { AutoNone, AutoBulletList, AutoAll }|
|enum|**[LineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum)** { NoWrap, WidgetWidth, FixedPixelWidth, FixedColumnWidth }|

----------


### **属性**
|  名称  | 类型|
|------:|:------|
| **[acceptRichText](https://doc.qt.io/qt-5/qtextedit.html#acceptRichText-prop)** | bool |
|**[autoFormatting](https://doc.qt.io/qt-5/qtextedit.html#autoFormatting-prop)** |AutoFormatting|
|**[cursorWidth](https://doc.qt.io/qt-5/qtextedit.html#cursorWidth-prop)** |int|
|**[document](https://doc.qt.io/qt-5/qtextedit.html#document-prop)** |QTextDocument*|
|**[documentTitle](https://doc.qt.io/qt-5/qtextedit.html#documentTitle-prop)** |QString|
|**[html](https://doc.qt.io/qt-5/qtextedit.html#html-prop)** |QString|
|**[lineWrapColumnOrWidth](https://doc.qt.io/qt-5/qtextedit.html#lineWrapColumnOrWidth-prop)** |int|
|**[lineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#lineWrapMode-prop)** |LineWrapMode|
|**[markdown](https://doc.qt.io/qt-5/qtextedit.html#markdown-prop)** |QString|
|**[overwriteMode](https://doc.qt.io/qt-5/qtextedit.html#overwriteMode-prop)** |bool|
|**[placeholderText](https://doc.qt.io/qt-5/qtextedit.html#placeholderText-prop)** |QString|
|**[plainText](https://doc.qt.io/qt-5/qtextedit.html#plainText-prop)** |QString|
|**[readOnly](https://doc.qt.io/qt-5/qtextedit.html#readOnly-prop)** |bool|
|**[tabChangesFocus](https://doc.qt.io/qt-5/qtextedit.html#tabChangesFocus-prop)** |bool|
|**[tabStopDistance](https://doc.qt.io/qt-5/qtextedit.html#tabStopDistance-prop)** |qreal|
|**[textInteractionFlags](https://doc.qt.io/qt-5/qtextedit.html#textInteractionFlags-prop)** |Qt::TextInteractionFlags|
|**[undoRedoEnabled](https://doc.qt.io/qt-5/qtextedit.html#undoRedoEnabled-prop)** |bool|
|**[wordWrapMode](https://doc.qt.io/qt-5/qtextedit.html#wordWrapMode-prop)** |QTextOption::WrapMode|
| ||

----------

### **公共成员函数**

|  类型  | 函数名|
|------:|:------|
|    |**[QTextEdit](https://doc.qt.io/qt-5/qtextedit.html#QTextEdit-1)**(const QString &*text*, QWidget **parent* = nullptr)|
| |**[QTextEdit](https://doc.qt.io/qt-5/qtextedit.html#QTextEdit)**(QWidget **parent* = nullptr)|
|virtual |**[QTextEdit](https://doc.qt.io/qt-5/qtextedit.html#QTextEdit)**(QWidget **parent* = nullptr)|
|bool |**[acceptRichText](https://doc.qt.io/qt-5/qtextedit.html#acceptRichText-prop)**() const|
|Qt::Alignment |**[alignment](https://doc.qt.io/qt-5/qtextedit.html#alignment)**() const|
|QString |**[anchorAt](https://doc.qt.io/qt-5/qtextedit.html#anchorAt)**(const QPoint &*pos*) const|
|QTextEdit::AutoFormatting |**[autoFormatting](https://doc.qt.io/qt-5/qtextedit.html#autoFormatting-prop)**() const|
|bool |**[canPaste](https://doc.qt.io/qt-5/qtextedit.html#canPaste)**() const|
|QMenu * |**[createStandardContextMenu](https://doc.qt.io/qt-5/qtextedit.html#createStandardContextMenu)**()|
|QMenu * |**[createStandardContextMenu](https://doc.qt.io/qt-5/qtextedit.html#createStandardContextMenu-1)**(const QPoint &*position*)|
|QTextCharFormat |**[currentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormat)**() const|
|QFont |**[currentFont](https://doc.qt.io/qt-5/qtextedit.html#currentFont)**() const|
|QTextCursor |**[cursorForPosition](https://doc.qt.io/qt-5/qtextedit.html#cursorForPosition)**(const QPoint &*pos*) const|
|QRect |**[cursorRect](https://doc.qt.io/qt-5/qtextedit.html#cursorRect)**(const QTextCursor &*cursor*) const|
|QRect |**[cursorRect](https://doc.qt.io/qt-5/qtextedit.html#cursorRect-1)**() const|
|int |**[cursorWidth](https://doc.qt.io/qt-5/qtextedit.html#cursorWidth-prop)**() const|
|QTextDocument * |**[document](https://doc.qt.io/qt-5/qtextedit.html#document-prop)**() const|
|QString |**[documentTitle](https://doc.qt.io/qt-5/qtextedit.html#documentTitle-prop)**() const|
|void |**[ensureCursorVisible](https://doc.qt.io/qt-5/qtextedit.html#ensureCursorVisible)**()|
|QList<QTextEdit::ExtraSelection> |**[extraSelections](https://doc.qt.io/qt-5/qtextedit.html#extraSelections)**() const|
|bool |**[find](https://doc.qt.io/qt-5/qtextedit.html#find)**(const QString &*exp*, QTextDocument::FindFlags *options* = QTextDocument::FindFlags())|
|bool |**[find](https://doc.qt.io/qt-5/qtextedit.html#find-1)**(const QRegExp &*exp*, QTextDocument::FindFlags *options* = QTextDocument::FindFlags())|
|bool |**[find](https://doc.qt.io/qt-5/qtextedit.html#find-2)**(const QRegularExpression &*exp*, QTextDocument::FindFlags *options* = QTextDocument::FindFlags())|
|QString |**[fontFamily](https://doc.qt.io/qt-5/qtextedit.html#fontFamily)**() const|
|bool |**[fontItalic](https://doc.qt.io/qt-5/qtextedit.html#fontItalic)**() const|
|qreal |**[fontPointSize](https://doc.qt.io/qt-5/qtextedit.html#fontPointSize)**() const|
|bool |**[fontUnderline](https://doc.qt.io/qt-5/qtextedit.html#fontUnderline)**() const|
|int |**[fontWeight](https://doc.qt.io/qt-5/qtextedit.html#fontWeight)**() const|
|bool |**[isReadOnly](https://doc.qt.io/qt-5/qtextedit.html#readOnly-prop)**() const|
|bool |**[isUndoRedoEnabled](https://doc.qt.io/qt-5/qtextedit.html#undoRedoEnabled-prop)**() const|
|int |**[lineWrapColumnOrWidth](https://doc.qt.io/qt-5/qtextedit.html#lineWrapColumnOrWidth-prop)**() const|
|QTextEdit::LineWrapMode |**[lineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#lineWrapMode-prop)**() const|
|virtual QVariant |**[lineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#lineWrapMode-prop)**() const|
|void |**[mergeCurrentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#mergeCurrentCharFormat)**(const QTextCharFormat &*modifier*)|
|void |**[moveCursor](https://doc.qt.io/qt-5/qtextedit.html#moveCursor)**(QTextCursor::MoveOperation *operation*, QTextCursor::MoveMode *mode* = QTextCursor::MoveAnchor)|
|bool |**[overwriteMode](https://doc.qt.io/qt-5/qtextedit.html#overwriteMode-prop)**() const|
|QString |**[placeholderText](https://doc.qt.io/qt-5/qtextedit.html#placeholderText-prop)**() const|
|void |**[print](https://doc.qt.io/qt-5/qtextedit.html#print)**(QPagedPaintDevice **printer*) const|
|void |**[setAcceptRichText](https://doc.qt.io/qt-5/qtextedit.html#acceptRichText-prop)**(bool *accept*)|
|void |**[setAutoFormatting](https://doc.qt.io/qt-5/qtextedit.html#autoFormatting-prop)**(QTextEdit::AutoFormatting *features*)|
|void |**[setCurrentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#setCurrentCharFormat)**(const QTextCharFormat &*format*)|
|void |**[setCursorWidth](https://doc.qt.io/qt-5/qtextedit.html#cursorWidth-prop)**(int *width*)|
|void |**[setDocument](https://doc.qt.io/qt-5/qtextedit.html#document-prop)**(QTextDocument **document*)|
|void |**[setDocumentTitle](https://doc.qt.io/qt-5/qtextedit.html#documentTitle-prop)**(const QString &*title*)|
|void |**[setExtraSelections](https://doc.qt.io/qt-5/qtextedit.html#setExtraSelections)**(const QList<QTextEdit::ExtraSelection> &*selections*)|
|void |**[setLineWrapColumnOrWidth](https://doc.qt.io/qt-5/qtextedit.html#lineWrapColumnOrWidth-prop)**(int *w*)|
|void |**[setLineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#lineWrapMode-prop)**(QTextEdit::LineWrapMode *mode*)|
|void |**[setOverwriteMode](https://doc.qt.io/qt-5/qtextedit.html#overwriteMode-prop)**(bool *overwrite*)|
|void |**[setPlaceholderText](https://doc.qt.io/qt-5/qtextedit.html#placeholderText-prop)**(const QString &*placeholderText*)|
|void |**[setReadOnly](https://doc.qt.io/qt-5/qtextedit.html#readOnly-prop)**(bool *ro*)|
|void |**[setTabChangesFocus](https://doc.qt.io/qt-5/qtextedit.html#tabChangesFocus-prop)**(bool *b*)|
|void |**[setTabStopDistance](https://doc.qt.io/qt-5/qtextedit.html#tabStopDistance-prop)**(qreal *distance*)|
|void |**[setTextCursor](https://doc.qt.io/qt-5/qtextedit.html#setTextCursor)**(const QTextCursor &*cursor*)|
|void |**[setTextInteractionFlags](https://doc.qt.io/qt-5/qtextedit.html#textInteractionFlags-prop)**(Qt::TextInteractionFlags *flags*)|
|void |**[setUndoRedoEnabled](https://doc.qt.io/qt-5/qtextedit.html#undoRedoEnabled-prop)**(bool *enable*)|
|void |**[setWordWrapMode](https://doc.qt.io/qt-5/qtextedit.html#wordWrapMode-prop)**(QTextOption::WrapMode *policy*)|
|bool |**[tabChangesFocus](https://doc.qt.io/qt-5/qtextedit.html#tabChangesFocus-prop)**() const|
|qreal |**[tabStopDistance](https://doc.qt.io/qt-5/qtextedit.html#tabStopDistance-prop)**() const|
|QColor |**[textBackgroundColor](https://doc.qt.io/qt-5/qtextedit.html#textBackgroundColor)**() const|
|QColor |**[textColor](https://doc.qt.io/qt-5/qtextedit.html#textColor)**() const|
|Qt::TextInteractionFlags |**[textInteractionFlags](https://doc.qt.io/qt-5/qtextedit.html#textInteractionFlags-prop)**() const|
|QString |**[toHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)**() const|
|QString |**[toMarkdown](https://doc.qt.io/qt-5/qtextedit.html#markdown-prop)**(QTextDocument::MarkdownFeatures *features* = QTextDocument::MarkdownDialectGitHub) const|
|QString |**[toPlainText](https://doc.qt.io/qt-5/qtextedit.html#toPlainText)**() const|
|QTextOption::WrapMode |**[wordWrapMode](https://doc.qt.io/qt-5/qtextedit.html#wordWrapMode-prop)**() const|

----------

### **重写父类的公共函数**

|             类型 | 函数名                                                       |
| ---------------: | ------------------------------------------------------------ |
| virtual QVariant | **[inputMethodQuery](https://doc.qt.io/qt-5/qtextedit.html#inputMethodQuery)**(Qt::InputMethodQuery *property*) const override |

--------

### **槽**

|  类型  | 函数名|
|------:|:------|
|void| **[append](https://doc.qt.io/qt-5/qtextedit.html#append)**(const QString &*text*) |
|void| **[clear](https://doc.qt.io/qt-5/qtextedit.html#clear)**() |
|void| **[copy](https://doc.qt.io/qt-5/qtextedit.html#copy)**() |
|void| **[cut](https://doc.qt.io/qt-5/qtextedit.html#cut)**() |
|void| **[insertHtml](https://doc.qt.io/qt-5/qtextedit.html#insertHtml)**(const QString &*text*) |
|void| **[insertPlainText](https://doc.qt.io/qt-5/qtextedit.html#insertPlainText)**(const QString &*text*) |
|void| **[paste](https://doc.qt.io/qt-5/qtextedit.html#paste)**() |
|void| **[redo](https://doc.qt.io/qt-5/qtextedit.html#redo)**() |
|void| **[scrollToAnchor](https://doc.qt.io/qt-5/qtextedit.html#scrollToAnchor)**(const QString &*name*) |
|void| **[selectAll](https://doc.qt.io/qt-5/qtextedit.html#selectAll)**() |
|void| **[setAlignment](https://doc.qt.io/qt-5/qtextedit.html#setAlignment)**(Qt::Alignment *a*) |
|void| **[setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)**(const QFont &*f*) |
|void| **[setFontFamily](https://doc.qt.io/qt-5/qtextedit.html#setFontFamily)**(const QString &*fontFamily*) |
|void| **[setFontItalic](https://doc.qt.io/qt-5/qtextedit.html#setFontItalic)**(bool *italic*) |
|void| **[setFontPointSize](https://doc.qt.io/qt-5/qtextedit.html#setFontPointSize)**(qreal *s*) |
|void| **[setFontUnderline](https://doc.qt.io/qt-5/qtextedit.html#setFontUnderline)**(bool *underline*) |
|void| **[setFontWeight](https://doc.qt.io/qt-5/qtextedit.html#setFontWeight)**(int *weight*) |
|void| **[setHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)**(const QString &*text*) |
|void| **[setMarkdown](https://doc.qt.io/qt-5/qtextedit.html#markdown-prop)**(const QString &*markdown*) |
|void| **[setPlainText](https://doc.qt.io/qt-5/qtextedit.html#setPlainText)**(const QString &*text*) |
|void| **[setText](https://doc.qt.io/qt-5/qtextedit.html#setText)**(const QString &*text*) |
|void| **[setTextBackgroundColor](https://doc.qt.io/qt-5/qtextedit.html#setTextBackgroundColor)**(const QColor &*c*) |
|void| **[setTextColor](https://doc.qt.io/qt-5/qtextedit.html#setTextColor)**(const QColor &*c*) |
|void| **[undo](https://doc.qt.io/qt-5/qtextedit.html#undo)**() |
|void| **[zoomIn](https://doc.qt.io/qt-5/qtextedit.html#zoomIn)**(int *range* = 1) |
|void| **[zoomOut](https://doc.qt.io/qt-5/qtextedit.html#zoomOut)**(int *range* = 1) |
||  |

----------

### **信号**

| 类型 | 函数名                                                       |
| ---: | ------------------------------------------------------------ |
| void | **[copyAvailable](https://doc.qt.io/qt-5/qtextedit.html#copyAvailable)**(bool *yes*) |
| void | **[currentCharFormatChanged](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormatChanged)**(const QTextCharFormat &*f*) |
| void | **[cursorPositionChanged](https://doc.qt.io/qt-5/qtextedit.html#cursorPositionChanged)**() |
| void | **[redoAvailable](https://doc.qt.io/qt-5/qtextedit.html#redoAvailable)**(bool *available*) |
| void | **[selectionChanged](https://doc.qt.io/qt-5/qtextedit.html#selectionChanged)**() |
| void | **[textChanged](https://doc.qt.io/qt-5/qtextedit.html#textChanged)**() |
| void | **[undoAvailable](https://doc.qt.io/qt-5/qtextedit.html#undoAvailable)**(bool *available*) |

--------

### **保护成员函数**

|                类型 | 函数名                                                       |
| ------------------: | ------------------------------------------------------------ |
|        virtual bool | **[canInsertFromMimeData](https://doc.qt.io/qt-5/qtextedit.html#canInsertFromMimeData)**(const QMimeData **source*) const |
| virtual QMimeData * | **[createMimeDataFromSelection](https://doc.qt.io/qt-5/qtextedit.html#createMimeDataFromSelection)**() const |
|        virtual void | **[insertFromMimeData](https://doc.qt.io/qt-5/qtextedit.html#insertFromMimeData)**(const QMimeData **source*) |

----

### **重写父类的保护方法**

|         类型 | 函数名                                                       |
| -----------: | ------------------------------------------------------------ |
| virtual void | **[changeEvent](https://doc.qt.io/qt-5/qtextedit.html#changeEvent)**(QEvent **e*) override |
| virtual void | **[contextMenuEvent](https://doc.qt.io/qt-5/qtextedit.html#contextMenuEvent)**(QContextMenuEvent **event*) override |
| virtual void | **[dragEnterEvent](https://doc.qt.io/qt-5/qtextedit.html#dragEnterEvent)**(QDragEnterEvent **e*) override |
| virtual void | **[dragLeaveEvent](https://doc.qt.io/qt-5/qtextedit.html#dragLeaveEvent)**(QDragLeaveEvent **e*) override |
| virtual void | **[dragMoveEvent](https://doc.qt.io/qt-5/qtextedit.html#dragMoveEvent)**(QDragMoveEvent **e*) override |
| virtual void | **[dropEvent](https://doc.qt.io/qt-5/qtextedit.html#dropEvent)**(QDropEvent **e*) override |
| virtual void | **[focusInEvent](https://doc.qt.io/qt-5/qtextedit.html#focusInEvent)**(QFocusEvent **e*) override |
| virtual void | **[focusNextPrevChild](https://doc.qt.io/qt-5/qtextedit.html#focusNextPrevChild)**(bool *next*) override |
| virtual void | **[focusOutEvent](https://doc.qt.io/qt-5/qtextedit.html#focusOutEvent)**(QFocusEvent **e*) override |
| virtual void | **[inputMethodEvent](https://doc.qt.io/qt-5/qtextedit.html#inputMethodEvent)**(QInputMethodEvent **e*) override |
| virtual void | **[keyPressEvent](https://doc.qt.io/qt-5/qtextedit.html#keyPressEvent)**(QKeyEvent **e*) override |
| virtual void | **[keyReleaseEvent](https://doc.qt.io/qt-5/qtextedit.html#keyReleaseEvent)**(QKeyEvent **e*) override |
| virtual void | **[mouseDoubleClickEvent](https://doc.qt.io/qt-5/qtextedit.html#mouseDoubleClickEvent)**(QMouseEvent **e*) override |
| virtual void | **[mouseMoveEvent](https://doc.qt.io/qt-5/qtextedit.html#mouseMoveEvent)**(QMouseEvent **e*) override |
| virtual void | **[mousePressEvent](https://doc.qt.io/qt-5/qtextedit.html#mousePressEvent)**(QMouseEvent **e*) override |
| virtual void | **[mouseReleaseEvent](https://doc.qt.io/qt-5/qtextedit.html#mouseReleaseEvent)**(QMouseEvent **e*) override |
| virtual void | **[paintEvent](https://doc.qt.io/qt-5/qtextedit.html#paintEvent)**(QPaintEvent **event*) override |
| virtual void | **[resizeEvent](https://doc.qt.io/qt-5/qtextedit.html#resizeEvent)**(QResizeEvent **e*) override |
| virtual void | **[scrollContentsBy](https://doc.qt.io/qt-5/qtextedit.html#scrollContentsBy)**(int *dx*, int *dy*) override |
| virtual void | **[showEvent](https://doc.qt.io/qt-5/qtextedit.html#showEvent)**(*QShowEvent **) override |
| virtual void | **[wheelEvent](https://doc.qt.io/qt-5/qtextedit.html#wheelEvent)**(QWheelEvent **e*) override |

## **详细说明**

----------

#### 概念介绍

QTextEdit 是一种高级的所见即所得的视图/编辑器控件，支持 HTML 风格标签，或者 Markdown 格式。为处理大的文档以及快速响应用户输入而专门做了优化。

QTextEdit 适用于段落和字符，段落是以单词为单位来适应控件宽度而格式化的字符串。默认情况下，读取纯文本时，一个新的换行表示一个段落。文档由零个以上段落组成。段落中的单词按照段落的对齐方式对齐，以硬换行符分隔。每一个字符都有自己的属性，比如字体和颜色。

QTextEdit 可以显示图片，列表和表格。如果文件太大无法在编辑窗口内全部展示，则会显示窗口滚动条。编辑器加载显示纯文本和富文本文件。富文本可以使用 HTML 4 标记的子集描述。有关详细信息，请参阅受支持的 [Supported HTML Subset](https://doc.qt.io/qt-5/richtext-html-subset.html) 页面。

如果只需要显示很小的一段富文本，可以使用 [QLabel](https://doc.qt.io/qt-5/qlabel.html) 。

Qt 中的富文本支持旨在提供一种快速、便携、高效的方法，为应用程序添加合理的在线帮助设施，并为富文本编辑器提供基础。如果您发现 它对 HTML 支持不能满足您的需求，您可以考虑使用 Qt WebKit ，它提供了功能齐全的 Web 浏览器控件。

QTextEdit 默认光标形状是 Qt::IBeamCursor 。可以通过函数 [viewport](https://doc.qt.io/qt-5/qabstractscrollarea.html#viewport)() 的光标属性进行修改。

#### 使用 QTextEdit 作为显示控件

QTextEdit 可以显示 HTML 的大型子集，包括表格和图片。

可以通过 [setHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)() 设置或将已有删除并将文本传入 [setHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)() 后替换回来。如果对旧版 HTML 调用 [setHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)() ，然后再调用 [toHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)() ，返回的文本的标签可能会改变，但是渲染是相同的。调用 [clear](https://doc.qt.io/qt-5/qtextedit.html#clear)() 删除所有文本。

通用可以通过 [setMarkdown](https://doc.qt.io/qt-5/qtextedit.html#markdown-prop)() 设置或替换文本，同样要注意：调用 [toMarkdown](https://doc.qt.io/qt-5/qtextedit.html#markdown-prop)() 时，返回的文本可能有变化，但是会尽可能保持原义。Markdown 包含内嵌 HTML 时会被解析，与 [setHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)() 有同样的限制。但是 [toMarkdown](https://doc.qt.io/qt-5/qtextedit.html#markdown-prop)() 只输出“纯” Markdown 语法文本，不包含内嵌的 HTML。

可以通过 QTextCursor 类插入文本，或者用更方便的函数 [insertHtml](https://doc.qt.io/qt-5/qtextedit.html#insertHtml)() 、[insertPlainText](https://doc.qt.io/qt-5/qtextedit.html#insertPlainText)() 、 [append](https://doc.qt.io/qt-5/qtextedit.html#append)() 或 [paste](https://doc.qt.io/qt-5/qtextedit.html#paste)() 。 [QTextCursor](https://doc.qt.io/qt-5/qtextcursor.html) 也能向文档中插入表格或列表等复杂的对象，同样它也可以用于创建文本选中并对选中文本进行设置。

默认情况下，编辑器在单词间空格处换行以适应控件的宽度。 [setLineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#lineWrapMode-prop)() 用来设置您想要的换行模式，指定 NoWrap 则不换行。调用 [setLineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#lineWrapMode-prop)() 时指定 [FixedPixelWidth](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum) 模式则是固定像素换行，指定 FixedColumnWidth 则是固定字符列数（例如80列）换行，并通过调用 [setLineWrapColumnOrWidth](https://doc.qt.io/qt-5/qtextedit.html#lineWrapColumnOrWidth-prop)()决定究竟是像素还是字符列来换行。如果使用 [WidgetWidth](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum) 指定根据控件宽度换行，您可以指定在空格上或者通过调用 [setWordWrapMode](https://doc.qt.io/qt-5/qtextedit.html#wordWrapMode-prop)() 指定任意位置进行换行。

[find](https://doc.qt.io/qt-5/qtextedit.html#find)() 函数可以用于在文本中查找和选中给定的字符串。

如果您想要在 QTextEdit 中限制段落总数，例如在日志查看器中经常用到。那么你可以使用 [QTextDocument](https://doc.qt.io/qt-5/qtextdocument.html) 的 maximumBlockCount 属性来实现。

----------

### **只读模式-键绑定**

当 QTextEdit 用于只读时，快捷键的绑定仅限于浏览，文本只能被鼠标选中。

|         按键          |       动作       |
| :-------------------: | :--------------: |
|          Up           |   向上移动一行   |
|         Down          |   向下移动一行   |
|         Left          |   左移一个字符   |
|         Right         |   右移一个字符   |
|        PageUp         | 向上翻页（视窗） |
|       PargeDown       | 向下翻页（视窗） |
|         Home          | 移动到文本最前端 |
|          End          | 移动到文本最末端 |
| Alt+Wheel（鼠标滚轮） |   水平滚动页面   |
|      Ctrl+Wheel       |     缩放文本     |
|        Ctrl+A         |   选中所有文本   |

文本编辑器也许能够提供一些元信息。例如， [documentTitle](https://doc.qt.io/qt-5/qtextedit.html#documentTitle-prop)() 函数将返回 HTML \<title> 标签内的文本。

注：缩放 HTML 文本时，只有当字体设置不是固定尺寸时才有效。

#### 使用 QTextEdit 作为编辑器

QTextEdit 作为显示控件时的所有操作在该场景下同样适用。

当前字符属性可通过 [setFontItalic](https://doc.qt.io/qt-5/qtextedit.html#setFontItalic)() 、 [setFontWeight](https://doc.qt.io/qt-5/qtextedit.html#setFontWeight)() 、 [setFontUnderline](https://doc.qt.io/qt-5/qtextedit.html#setFontUnderline)() 、 [setFontFamily](https://doc.qt.io/qt-5/qtextedit.html#setFontFamily)() 、 [setFontPointSize](https://doc.qt.io/qt-5/qtextedit.html#setFontPointSize)() 、 [setTextColor](https://doc.qt.io/qt-5/qtextedit.html#setTextColor)() 和 [setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)()等函数来设置。通过 [setAlignment](https://doc.qt.io/qt-5/qtextedit.html#setAlignment)() 设置段落对齐。

QTextCursor 类可以处理文本选择，通过该类可以创建选择，恢复文本内容或者删除选择。可以使用 textCursor() 函数检索与用户可见光标对应的对象。如果要在 QTextEdit 中设置选择文本，只需在 QTextCursor 对象上创建一个选择，然后使用  setTextCursor() 使光标成为可见光标。所选内容可以通过 [copy](https://doc.qt.io/qt-5/qtextedit.html#copy)() 和 [cut](https://doc.qt.io/qt-5/qtextedit.html#cut)() 复制或剪切到剪切板。选中全部文本可使用 [selectAll](https://doc.qt.io/qt-5/qtextedit.html#selectAll)()。

当光标移动以时内部的格式属性会改变，[currentCharFormatChanged](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormatChanged)() 信号会被发送以反映新的光标位置属性。

任何时候文本一旦更改（由于 [setText](https://doc.qt.io/qt-5/qtextedit.html#setText)() 或者编辑器本身触发）都会发送 [textChanged](https://doc.qt.io/qt-5/qtextedit.html#textChanged)()  信号。

QTextEdit 保存了 QTextDocument 对象，可以使用 [document](https://doc.qt.io/qt-5/qtextedit.html#document-prop)() 方法检索该对象。还可以使用 [setDocument](https://doc.qt.io/qt-5/qtextedit.html#document-prop)()设置自己的文档对象。

[QTextDocument](https://doc.qt.io/qt-5/qtextdocument.html) 提供了 [isModified()](https://doc.qt.io/qt-5/qtextdocument.html#modified-prop) 函数，当文档在第一次被加载或者最后一次以 false 为参数调用 setModified 后文本产生了修改，则该函数返回 true 。同时[QTextDocument](https://doc.qt.io/qt-5/qtextdocument.html) 也提供了撤销和重做的功能。

#### 拖放

--------

QTextEdit 同时还支持自定义拖放行为。默认情况下，当用户将这些 [MIME](https://baike.baidu.com/item/MIME/2900607) 类型的数据放到文档中时，QTextEdit 将插入纯文本、 HTML 和富文本。重写类方法 [canInsertFromMimeData](https://doc.qt.io/qt-5/qtextedit.html#canInsertFromMimeData)() 和  [insertFromMimeData](https://doc.qt.io/qt-5/qtextedit.html#insertFromMimeData)()  可以支持一些其他的 [MIME](https://baike.baidu.com/item/MIME/2900607) 类型数据。

例如，为 QTextEdit 实现拖放图片的功能，你可以按照以下方式实现：

```c++
bool TextEdit::canInsertFromMimeData( const QMimeData *source ) const
{
    if (source->hasImage())
        return true;
    else
        return QTextEdit::canInsertFromMimeData(source);
}
```

通过返回 true 我们添加了图片 [MIME](https://baike.baidu.com/item/MIME/2900607) 类型的数据的支持，其他类型则使用默认方法。

```c++
void TextEdit::insertFromMimeData( const QMimeData *source )
{
    if (source->hasImage())
    {
        QImage image = qvariant_cast<QImage>(source->imageData());
        QTextCursor cursor = this->textCursor();
        QTextDocument *document = this->document();
        document->addResource(QTextDocument::ImageResource, QUrl("image"), image);
        cursor.insertImage("image");
    }
}
```

我们从 MIME 源持有的  [QVariant](https://doc.qt.io/qt-5/qvariant.html) 解包图像，作为资源插入到文档。

### **Editing Key Bindings**

--------

在编辑时的按键绑定。

|     按键     |                      动作                      |
| :----------: | :--------------------------------------------: |
|  Backspace   |                删除光标左侧字符                |
|    Delete    |                删除光标右侧字符                |
|    Ctrl+C    |               复制（选中的文本）               |
| Ctrl+Insert  |               复制（选中的文本）               |
|    Ctrl+K    |                   删除到行尾                   |
|    Ctrl+V    |                      粘贴                      |
| Shift+Insert |                      粘贴                      |
|    Ctrl+X    |                      剪切                      |
| Shift+Delete |                      剪切                      |
|    Ctrl+Z    |                      撤销                      |
|    Ctrl+Y    |                      重做                      |
|     Left     |              光标向左移动一个字符              |
|  Ctrl+Left   | 光标向左移动一个单词（译者注：以空格区分单词） |
|    Right     |              光标向右移动一个字符              |
|  Ctrl+Right  |              光标向右移动一个单词              |
|      Up      |                光标向上移动一行                |
|     Down     |                光标向下移动一行                |
|    PageUp    |                光标向上移动一页                |
|   PageDown   |                光标向下移动一页                |
|     Home     |                 光标移动到行首                 |
|  Ctrl+Home   |               光标移动到文本之首               |
|     End      |                 光标移动到行尾                 |
|   Ctrl+End   |               光标移动到文本之尾               |
|  Alt+Wheel   |                  横向滚动翻页                  |
|              |                                                |

要选择（标记）文本，按住 Shift 键同时按一个移动击键，例如，Shift+Right 将选择右侧的字符，Shift+Ctrl=Right 将选择右侧的单词，等等。

您也可以在[QTextDocument](https://doc.qt.io/qt-5/qtextdocument.html) 、 [QTextCursor](https://doc.qt.io/qt-5/qtextcursor.html)、 [Application Example](https://doc.qt.io/qt-5/qtwidgets-mainwindows-application-example.html) 、 [Syntax Highlighter Example](https://doc.qt.io/qt-5/qtwidgets-richtext-syntaxhighlighter-example.html) 、 [Rich Text Processing](https://doc.qt.io/qt-5/richtext.html)中找到相关信息。

### **类型成员**

--------

#### enum QTextEdit::AutoFormattingFlag / flags QTextEdit::AutoFormatting

| 常量                      | 值         | 描述                                                         |
| :------------------------ | :--------- | ------------------------------------------------------------ |
| QTextEdit::AutoNone       | 0          | 不做任何自动格式化。                                         |
| QTextEdit::AutoBulletList | 0x00000001 | 自动创建项目符号列表（在列的最左侧输入‘*’或者在已有符号列表后输入回车）。 |
| QTextEdit::AutoAll        | 0xffffffff | 应用所有自动格式化，目前只支持项目符号列表。                 |

自动格式化类型由 [QFlags](https://doc.qt.io/qt-5/qflags.html) \<AutoFormattingFlag> 定义，存储上面各值的或运算结果值。

#### enum QTextEdit::LineWrapMode

| 常量                        | 值   |
| --------------------------- | ---- |
| QTextEdit::NoWrap           | 0    |
| QTextEdit::WidgetWidth      | 1    |
| QTextEdit::FixedPixelWidth  | 2    |
| QTextEdit::FixedColumnWidth | 3    |

## **成员变量**

**acceptRichText : bool**

--------

该属性值表示是否接受用户输入富文本。

如果该属性值为 false ，则表示只接受纯文本输入。例如从剪切板或通过拖放。

该属性值默认是 true 。在 Qt 4.1 中引入。

**访问函数**

| 类型 | 函数名                               |
| ---: | ------------------------------------ |
| bool | **acceptRichText**() const           |
| void | **setAcceptRichText**(bool *accept*) |



**autoFormatting : [AutoFormatting](https://doc.qt.io/qt-5/qtextedit.html#AutoFormattingFlag-enum)**

--------

该属性值表示是否开启自动格式化功能。

该属性值可以是 [AutoFormattingFlag](https://doc.qt.io/qt-5/qtextedit.html#AutoFormattingFlag-enum) 枚举的任何值之间的或结合。默认值是 [AutoNone](https://doc.qt.io/qt-5/qtextedit.html#AutoFormattingFlag-enum) ，选择 [AutoAll](https://doc.qt.io/qt-5/qtextedit.html#AutoFormattingFlag-enum) 是开启所有自动格式化功能。目前只支持项目符号列表，以后的版本可能会加入其他格式化功能。

访问函数：

|                      类型 | 函数名                                                      |
| ------------------------: | ----------------------------------------------------------- |
| QTextEdit::AutoFormatting | **autoFormatting**() const                                  |
|                      void | **setAutoFormatting**(QTextEdit::AutoFormatting *features*) |



**cursorWidth : int**

--------

该属性值指定了光标的像素宽度，默认是1。

该属性在 Qt 4.2 引入。

**访问函数**

|                      类型 | 函数名                          |
| ------------------------: | ------------------------------- |
| QTextEdit::AutoFormatting | **cursorWidth**() const         |
|                      void | **setCursorWidth**(int *width*) |



**document : [QTextDocument](https://doc.qt.io/qt-5/qtextdocument.html)***

--------

该属性值为文本编辑器内部的文档对象。

注：编辑器不会拥有该文档的所有权，除非它是文档的父对象。提供文档的父对象仍然是该对象的所有者。如果之前分配的文档是编辑器的子对象，则会将其删除。

|            类型 | 函数名                                     |
| --------------: | ------------------------------------------ |
| QTextDocument * | **document**() const                       |
|            void | **setDocument**(QTextDocument **document*) |



**documentTitle : [QString](https://doc.qt.io/qt-5/qstring.html)**

--------

该属性值保存了从文本中解析出的文档标题。

默认情况，当新建空的文档时，该属性值为空字符串。

**访问函数**

|    类型 | 函数名                                       |
| ------: | -------------------------------------------- |
| QString | **documentTitle**() const                    |
|    void | **setDocumentTitle**(const QString &*title*) |



**html : QString**

--------

该属性值为编辑器中的文本提供了 HTML 接口。

toHTML() 以 HTML 格式返回文本内容。

setHTML() 会修改编辑器中的文本。所有之前被删除的文本以及撤销/重做历史都会被清空。输入的文本都被解析为 HTML 格式的富文本。[currentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormat)() 也会被重置，除非光标已经处在文档最前端。

注：当包含 HTML 的 QString 被创建且被传给 setHTML() 时，由调用者保证文本能够正确解码。

默认新建空文档时，该属性值包含了 HTML 4.0 的相关描述文本，不含正文。

**访问函数**

|    类型 | 函数名                             |
| ------: | ---------------------------------- |
| QString | **toHtml**() const                 |
|    void | **setHtml**(const QString &*text*) |

**通知信号**

| 类型 | 函数名                                                       |
| ---: | ------------------------------------------------------------ |
| void | **[textChanged](https://doc.qt.io/qt-5/qtextedit.html#textChanged)**() |

您也可以在 [Supported HTML Subset](https://doc.qt.io/qt-5/richtext-html-subset.html) 和  [plainText](https://doc.qt.io/qt-5/qtextedit.html#plainText-prop) 中找到相关信息。



**lineWrapColumnOrWidth : int**

--------

该属性值保存了文本的换行位置（根据不同换行模式可以是像素或者字符列数）。

如果换行模式是 [FixedPixelWidth](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum) ，该属性值为文本换行位置到编辑器左侧边缘的像素数。如果换行模式是  [FixedColumnWidth](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum) ，该属性值为文本换行位置到编辑器左侧边缘的字符列数。

默认值是0。

**访问函数**

| 类型 | 函数名                                |
| ---: | ------------------------------------- |
|  int | **lineWrapColumnOrWidth**() const     |
| void | **setLineWrapColumnOrWidth**(int *w*) |

您也可以在 [lineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#lineWrapMode-prop) 中找到相关信息。



**lineWrapMode : [LineWrapMode](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum)**

--------

该属性值保存了换行模式。

默认模式 [WidgetWidth](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum) 会使文本在编辑器最右侧按照单词进行换行。当空格符处出现换行时，会保持单词的完整性，不会造成单词拆分。如果你希望在单词中出现换行，可以通过 [setWordWrapMode](https://doc.qt.io/qt-5/qtextedit.html#wordWrapMode-prop)() 进行设置。如果你设置的换行模式是  [FixedPixelWidth](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum) 或 [FixedColumnWidth](https://doc.qt.io/qt-5/qtextedit.html#LineWrapMode-enum)，你还应该调用[setLineWrapColumnOrWidth](https://doc.qt.io/qt-5/qtextedit.html#lineWrapColumnOrWidth-prop)() 设置你想要的行宽。

**访问函数**

|                    类型 | 函数名                                              |
| ----------------------: | --------------------------------------------------- |
| QTextEdit::LineWrapMode | **lineWrapMode**() const                            |
|                    void | **setLineWrapMode**(QTextEdit::LineWrapMode *mode*) |

您还可以从 [lineWrapColumnOrWidth](https://doc.qt.io/qt-5/qtextedit.html#lineWrapColumnOrWidth-prop) 找到相关信息。



**markdown : [QString](https://doc.qt.io/qt-5/qstring.html)**

----

该属性值为编辑器中的文本提供了 Markdown 接口。

toMarkdown() 返回“纯” Markdown 格式文本，不含任何内嵌的 HTML 格式。一些 [QTextDocument](https://doc.qt.io/qt-5/qtextdocument.html) 支持的功能（例如颜色和字体）都不会在“纯” Markdown 下显示，而是被忽略掉。

setMarkdown() 会修改编辑器中的文本。所有之前被删除的文本以及撤销/重做历史都会被清空。输入的文本都会被解析为 Markdown 格式的富文本。

Markdwon 中包含 HTML 块时解析的方式与 [setHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop) 一样，然而，HTML 块中内嵌的 Markdown 时则不被支持。

一些解析的功能可以通过 feature 参数开启或关闭。

| 常量                      | 描述                                 |
| ------------------------- | ------------------------------------ |
| MarkdownNoHTML            | 丢弃 Markdown 中的所有 HTML 标签     |
| MarkdownDialectCommonMark | 解析仅支持被 CommonMark 标准化的功能 |
| MarkdownDialectGitHub     | 解析支持 GitHub 方言（默认值）       |

该属性在 Qt 5.14 引入。

**访问函数**

|    类型 | 函数名                                                       |
| ------: | ------------------------------------------------------------ |
| QString | **toMarkdown**(QTextDocument::MarkdownFeatures *features* = QTextDocument::MarkdownDialectGitHub) const |
|    void | **setMarkdown**(const QString &*markdown*)                   |

**通知信号**

| 类型 | 函数                                                         |
| ---- | ------------------------------------------------------------ |
| void | **[textChanged](https://doc.qt.io/qt-5/qtextedit.html#textChanged)**() |

您也可以在 [plainText](https://doc.qt.io/qt-5/qtextedit.html#plainText-prop) 、 [html](https://doc.qt.io/qt-5/qtextedit.html#html-prop) 、 [QTextDocument::toMarkdown](https://doc.qt.io/qt-5/qtextdocument.html#toMarkdown)() 和 [QTextDocument::setMarkdown](https://doc.qt.io/qt-5/qtextdocument.html#setMarkdown)() 中找到相关信息。



**overwriteMode : bool**

----

该属性值表示用户输入时是否覆盖已有文本。

像许多文本编辑器一样，在用户输入时编辑器控件可以配置是插入已有文本还是覆盖已有文本。

该属性值为 true 时，已有文本会被逐个字符地替换掉。属性值为 false 时，新文本会在光标处插入。

默认值是 false（文本不会被覆盖）。

该属性在 Qt 4.1 引入。

访问函数：

| 类型 | 函数名                                 |
| ---: | -------------------------------------- |
| bool | **overwriteMode**() const              |
| void | **setOverwriteMode**(bool *overwrite*) |



**placeholderText : [QString](https://doc.qt.io/qt-5/qstring.html)**

----

该属性保存编辑器占位符。

当 document() 为空时设置该属性值使编辑器得占位符标志为灰色。

默认情况，该属性包含一个空字符串。

该属性在 Qt 5.2 引入。

访问函数：

|    类型 | 函数名                                                   |
| ------: | -------------------------------------------------------- |
| QString | **placeholderText**() const                              |
|    void | **setPlaceholderText**(const QString &*placeholderText*) |

你也可以在 [document](https://doc.qt.io/qt-5/qtextedit.html#document-prop)() 中找到相关信息。



**plainText : [QString](https://doc.qt.io/qt-5/qstring.html)**

----

该属性用于获取和设置编辑器中的纯文本。

当属性被设置时，先前的内容以及撤销/重做历史将被清空。 [currentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormat)() 也会被重置，除非光标已经处在文档最前端。

如果文本编辑器中有其他类型的内容，当调用 [toPlainText](https://doc.qt.io/qt-5/qtextedit.html#toPlainText)() 时则不会用纯文本替换他。唯一例外是 &nbsp 字符，会替换为标准空白符。

默认当编辑器无内容时，该属性包含一个空字符串。

该属性在 Qt 4.3 中引入。

访问函数：

|    类型 | 函数名                                                       |
| ------: | ------------------------------------------------------------ |
| QString | **[toPlainText](https://doc.qt.io/qt-5/qtextedit.html#toPlainText)**() const |
|    void | **[setPlainText](https://doc.qt.io/qt-5/qtextedit.html#setPlainText)**(const QString &*text*) |

您也可以在 [html](https://doc.qt.io/qt-5/qtextedit.html#html-prop) 中找到相关信息。



**readOnly : bool**

----

该属性值表示文本编辑器只读属性。

在只读模式下用户只能浏览和选择文本，而不能修改它。

默认值是 false 。

访问函数：

| 类型 | 函数名                     |
| ---: | -------------------------- |
| bool | **isReadOnly**() const     |
| void | **setReadOnly**(bool *ro*) |



**tabChangesFocus : bool**

----

该属性表示 Tab 键是改变焦点还是作为输入。

在某些情况下，文本编辑不应允许用户使用 Tab 键输入制表符或更改缩进，因为这将会打断焦点链。默认值为 false 。

访问函数：

| 类型 | 函数名                           |
| ---: | -------------------------------- |
| bool | **tabChangesFocus**() const      |
| void | **setTabChangesFocus**(bool *b*) |



**tabStopDistance : [qreal](https://doc.qt.io/qt-5/qtglobal.html#qreal-typedef)**

----

该属性值为制表位距离的像素数。

默认值为 80 像素。

该属性在 Qt 5.10 引入。

访问函数：

|  类型 | 函数名                                   |
| ----: | ---------------------------------------- |
| qreal | **tabStopDistance**() const              |
|  void | **setTabStopDistance**(qreal *distance*) |



**textInteractionFlags : [Qt::TextInteractionFlags](https://doc.qt.io/qt-5/qt.html#TextInteractionFlag-enum)**

----

指定控件如何与用户输入进行交互。

默认值取决于 [QTextEdit](https://doc.qt.io/qt-5/qtextedit.html) 是只读还是可编辑。以及控件是不是 [QTextBrowser](https://doc.qt.io/qt-5/qtextbrowser.html) 。

该属性在 Qt 4.2 引入。

访问函数：

|                     类型 | 函数名                                                       |
| -----------------------: | ------------------------------------------------------------ |
| Qt::TextInteractionFlags | **textInteractionFlags**() const                             |
|                     void | **setTextInteractionFlags**(Qt::TextInteractionFlags *flags*) |



**undoRedoEnabled : bool**

----

该属性值表示是否开启撤销和重做功能。

只有此属性为 true ，并且存在可以撤消（或重做）的操作时，用户才能撤消或重做。

访问函数：

| 类型 | 函数名                                |
| ---: | ------------------------------------- |
| bool | **isUndoRedoEnabled**() const         |
| void | **setUndoRedoEnabled**(bool *enable*) |



**wordWrapMode : [QTextOption::WrapMode](https://doc.qt.io/qt-5/qtextoption.html#WrapMode-enum)**

----

该属性值为 QTextEdit 在用单词换行文本时使用的模式

默认值被设置为 [QTextOption::WrapAtWordBoundaryOrAnywhere](https://doc.qt.io/qt-5/qtextoption.html#WrapMode-enum) 。

访问函数：

|                  类型 | 函数名                                              |
| --------------------: | --------------------------------------------------- |
| QTextOption::WrapMode | **wordWrapMode**() const                            |
|                  void | **setWordWrapMode**(QTextOption::WrapMode *policy*) |

您也可以在 [QTextOption::WrapMode](https://doc.qt.io/qt-5/qtextoption.html#WrapMode-enum) 中找到相关信息。

## **成员函数**

----------

**QTextEdit::QTextEdit(const [QString](https://doc.qt.io/qt-5/qstring.html) &*text*, [QWidget](https://doc.qt.io/qt-5/qwidget.html#QWidget) *\*parent* = nullptr)**

通过父对象 *parent* 构造 QTextEdit 。该类用于显示文本，文本被解释为 html 。

----------

 **QTextEdit::QTextEdit([QWidget](https://doc.qt.io/qt-5/qwidget.html#QWidget) *\*parent* = nullptr)**

通过父对象 *parent* 构造一个空的 QTextEdit 。

----

**void QTextEdit::append(const [QString](https://doc.qt.io/qt-5/qstring.html) &*text*)**	[slot]

在文本末尾追加新的文本段落。

注：附加的新段落将具有与当前段落相同的字符格式和块格式，由光标的位置决定。

您也可以在 [currentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormat)() 和 [QTextCursor::blockFormat](https://doc.qt.io/qt-5/qtextcursor.html#blockFormat)() 中找到相关信息。

----

**void QTextEdit::clear()**	[slot]

删除文本编辑器中所有文本。

注：

- 撤销/重做历史也会被清楚。
- [currentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormat)() 也会被重置，除非光标已经处在文档最前端。

----

**void QTextEdit::copyAvailable(bool *yes*)**	[signal]

在文本编辑中选择或取消选择文本时，将发出此信号。

选择文本时将发出该信号时将 *yes* 被置为 true 。如果未选择任何文本或取消选择所选文本，则发出此信号时将 *yes* 设置为 false 。

如果 *yes* 为 true 时可以使用 [copy](https://doc.qt.io/qt-5/qtextedit.html#copy)() 将选择内容复制到剪切板。如果 *yes* 为 false 则不做任何事情。

您已可以在 [selectionChanged](https://doc.qt.io/qt-5/qtextedit.html#selectionChanged)() 中找到相关信息。

----

**void QTextEdit::currentCharFormatChanged(const [QTextCharFormat](https://doc.qt.io/qt-5/qtextcharformat.html) &*f*)**	[signal]

如果当前字符格式改变时(例如，由光标位置的变化引起)发送该信号。

新的格式是 *f* 。

您也可以在 [setCurrentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#setCurrentCharFormat)() 中找到相关信息。

----

**void QTextEdit::cursorPositionChanged()**	[signal]

当光标位置产生变化时则发送该信号。

----

**void QTextEdit::cut()** [slot]

剪切内容到剪切板。

您也可以在 [copy](https://doc.qt.io/qt-5/qtextedit.html#copy)() 和 [paste](https://doc.qt.io/qt-5/qtextedit.html#paste)() 中找到相关信息。

----

**void QTextEdit::insertHtml(const [QString](https://doc.qt.io/qt-5/qstring.html) &*text*)**	[slot]

该函数为槽函数，假定在当前光标下插入的文本为 html 格式。

相当于：

```c++
edit->textCursor().insertHtml(fragment);
```

注：当将此功能与样式表一起使用时，样式表将仅适用于文档中的当前块。要在整个文档中应用样式表，请使用 [QTextDocument::setDefaultStyleSheet](https://doc.qt.io/qt-5/qtextdocument.html#defaultStyleSheet-prop)() 。

----

**void QTextEdit::insertPlainText(const [QString](https://doc.qt.io/qt-5/qstring.html) &*text*)**	[slot]

在当前光标位置插入文本的槽函数。

相当于：

```c++
edit->textCursor().insertText(text);
```

----

**void QTextEdit::paste()**	[slot]

在当前光标位置粘贴剪切板中的内容。

要更改此函数的行为，即修改 QTextEdit 可以粘贴的是什么以及如何粘贴，重新实现虚函数 [canInsertFromMimeData](https://doc.qt.io/qt-5/qtextedit.html#canInsertFromMimeData)() 和 [insertFromMimeData](https://doc.qt.io/qt-5/qtextedit.html#insertFromMimeData)() 。

您也可以在 [cut](https://doc.qt.io/qt-5/qtextedit.html#cut)() 和 [copy](https://doc.qt.io/qt-5/qtextedit.html#copy)()中找到相关信息。

----

**void QTextEdit::redo()**	[slot]

重做上一次操作。

如果没有需要重做的操作，如果没有要重做的操作，即撤消/重做历史记录中没有重做步骤，则不执行任何操作。

该函数在 Qt 4.2 中引入。

您也可以在 [undo](https://doc.qt.io/qt-5/qtextedit.html#undo)() 中找到相关信息。

----

**void QTextEdit::redoAvailable(bool *available*)**	[signal]

当重做操作可用或不可用时发送该信号。

----

**void QTextEdit::scrollToAnchor(const [QString](https://doc.qt.io/qt-5/qstring.html) &*name*)**	[slot]

滚动文本编辑器以使名称为 *name* 的锚点可见。如果 *name* 为空，或者锚点已可见，或者找不到该锚点，则该函数不做操作。

----

**void QTextEdit::selectAll()**	[slot]

选中所有文本。

您也可以在  [copy](https://doc.qt.io/qt-5/qtextedit.html#copy)() 、 [cut](https://doc.qt.io/qt-5/qtextedit.html#cut)() 和 [textCursor](https://doc.qt.io/qt-5/qtextedit.html#textCursor)() 中找到相关信息。

----

**void QTextEdit::selectionChanged()**	[signal]

当文本选择产生变化时发送该信号。

您也可以在 [copyAvailable](https://doc.qt.io/qt-5/qtextedit.html#copyAvailable)() 中找到相关信息。

----

----

**void QTextEdit::setAlignment([Qt::Alignment](https://doc.qt.io/qt-5/qt.html#AlignmentFlag-enum) *a*)**	[slot]

通过 a 指定当前段落对齐方式。分别有 [Qt::AlignLeft](https://doc.qt.io/qt-5/qt.html#AlignmentFlag-enum) 、 [Qt::AlignRight](https://doc.qt.io/qt-5/qt.html#AlignmentFlag-enum) 、 [Qt::AlignJustify](https://doc.qt.io/qt-5/qt.html#AlignmentFlag-enum) 和 [Qt::AlignCenter](https://doc.qt.io/qt-5/qt.html#AlignmentFlag-enum) (水平居中)。

您也可以在 [alignment](https://doc.qt.io/qt-5/qtextedit.html#alignment)() 中找到相关信息。

----

----

**void QTextEdit::setCurrentFont(const [QFont](https://doc.qt.io/qt-5/qfont.html) &*f*)**	[slot]

设置当前字体格式为 *f* 。

您也可以在 [currentFont](https://doc.qt.io/qt-5/qtextedit.html#currentFont)()、 [setFontPointSize](https://doc.qt.io/qt-5/qtextedit.html#setFontPointSize)() 和 [setFontFamily](https://doc.qt.io/qt-5/qtextedit.html#setFontFamily)() 中找到相关信息。

--------

**void QTextEdit::setFontFamily(const [QString](https://doc.qt.io/qt-5/qstring.html) &*fontFamily*)**	[slot]

设置当前字体系列。

您也可以在 [fontFamily](https://doc.qt.io/qt-5/qtextedit.html#fontFamily)() 和 [setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)() 中找到相关信息。

---

**void QTextEdit::setFontItalic(bool *italic*)**	[slot]

当 *italic* 为 true 时，设置当前字体为斜体。否则字体为非斜体。

您也可以在 [fontItalic](https://doc.qt.io/qt-5/qtextedit.html#fontItalic)() 中找到相关信息。

----

**void QTextEdit::setFontPointSize([qreal](https://doc.qt.io/qt-5/qtglobal.html#qreal-typedef) *s*)**	[slot]

将当前字体格式的点大小设置为 *s* 。

请注意，如果 *s* 为零或负，则此函数的行为未定义。

您也可以在 [fontPointSize](https://doc.qt.io/qt-5/qtextedit.html#fontPointSize)()、 [setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)() 和 [setFontFamily](https://doc.qt.io/qt-5/qtextedit.html#setFontFamily)() 中找到相关信息。

----

**void QTextEdit::setFontUnderline(bool *underline*)**	[slot]

如果 *underline* 为 true ，则为当前字体设置下划线，否则不设置。

您也可以在 [fontUnderline](https://doc.qt.io/qt-5/qtextedit.html#fontUnderline)() 中找到相关信息。

----

**void QTextEdit::setFontWeight(int *weight*)**	[slot]

设置当前字体大小为 weight ，可用值范围由 [QFont::Weight](https://doc.qt.io/qt-5/qfont.html#Weight-enum) 枚举值给定。

您也可也在 [fontWeight](https://doc.qt.io/qt-5/qtextedit.html#fontWeight)() 、 [setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)() 和 [setFontFamily](https://doc.qt.io/qt-5/qtextedit.html#setFontFamily)() 中找到相关信息。

----

**void QTextEdit::setPlainText(const [QString](https://doc.qt.io/qt-5/qstring.html) &*text*)**	[slot]

将编辑器文本设置为 *text* ，之前的文本被删除。

注意：

- text 被解析为纯文本。
- 撤销/重做历史被清空。
- [currentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormat)() 也会被重置，除非光标已经处在文档最前端。

您也可以在 [toPlainText](https://doc.qt.io/qt-5/qtextedit.html#toPlainText)() 中找到相关信息。

----

**void QTextEdit::setText(const [QString](https://doc.qt.io/qt-5/qstring.html) &*text*)**	[slot]

设置编辑器的文本。文本可以是纯文本，也可以是 HTML 格式，编辑器会尝试猜测文本的正确格式。

请直接使用 [setHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)() 或 [setPlainText](https://doc.qt.io/qt-5/qtextedit.html#setPlainText)() 函数，避免让编辑器猜测文本格式。

该函数在 Qt 4.2 中引入。

您也可以在 [toPlainText](https://doc.qt.io/qt-5/qtextedit.html#toPlainText)() 和 [toHtml](https://doc.qt.io/qt-5/qtextedit.html#html-prop)() 中找到相关信息。

----

**void QTextEdit::setTextBackgroundColor(const [QColor](https://doc.qt.io/qt-5/qcolor.html) &*c*)**	[slot]

设置文本背景色为 *c* 。

该函数在 Qt 4.4 中引入。

您也可以在 [textBackgroundColor](https://doc.qt.io/qt-5/qtextedit.html#textBackgroundColor)() 中找到相关信息。

----

**void QTextEdit::setTextColor(const [QColor](https://doc.qt.io/qt-5/qcolor.html) &*c*)**	[slot]

设置文本颜色为 *c* 。

您也可以在 [textColor](https://doc.qt.io/qt-5/qtextedit.html#textColor)() 中找到相关信息。

----

**void QTextEdit::textChanged()**	[slot]

当文档内容更改时发送该信号。例如，文本插入，删除或格式变化时。

注：该函数时属性 [html](https://doc.qt.io/qt-5/qtextedit.html#html-prop) 和 [markdown](https://doc.qt.io/qt-5/qtextedit.html#markdown-prop) 的通知信号。

----

**void QTextEdit::undo()**	[slot]

撤销最后一次操作。

如果没有要撤销的操作，即撤消/重做历史记录中没有撤销的步骤，则不执行任何操作。

该函数在 Qt 4.2 中引入。

您也可以在 [redo](https://doc.qt.io/qt-5/qtextedit.html#redo)() 中找到相关信息。

----

**void QTextEdit::undoAvailable(bool *available*)**	[signal]

当撤销操作可用时发送该信号。

----

**void QTextEdit::zoomIn(int *range* = 1)**	[slot]

使基本字体大小放大为 *range* 个点，然后以这个新的尺寸重新计算字体大小，以此来放大文本。该操作不会改变图片尺寸。

您也可以在 [zoomOut](https://doc.qt.io/qt-5/qtextedit.html#zoomOut)() 中找到相关信息。

----

**void QTextEdit::zoomOut(int *range* = 1)**	[slot]

使基本字体大小缩小为 *range* 个点，然后以这个新的尺寸重新计算字体大小，以此来缩小文本。该操作不会改变图片尺寸。

您也可以在 [zoomIn](https://doc.qt.io/qt-5/qtextedit.html#zoomIn)() 中找到相关信息。

----

**QTextEdit::~QTextEdit()**	[virtual]

析构函数。

----

**[Qt::Alignment](https://doc.qt.io/qt-5/qt.html#AlignmentFlag-enum) QTextEdit::alignment() const**

返回当前段落对齐方式。

您也可以在 [setAlignment](https://doc.qt.io/qt-5/qtextedit.html#setAlignment)() 中找到相关信息。

----

**[QString](https://doc.qt.io/qt-5/qstring.html) QTextEdit::anchorAt(const [QPoint](https://doc.qt.io/qt-5/qpoint.html) &*pos*) const**

返回在位置 *pos* 处锚点的引用。如果该位置处没有锚点则返回空字符串。

----

**bool QTextEdit::canInsertFromMimeData(const [QMimeData](https://doc.qt.io/qt-5/qmimedata.html) *\*source*) const**	[virtual protected]

如果由 *source* 指定的 MIME 数据对象可以被解码并且能被插入到文档中则该函数返回 true 。例如，在拖动操作期间，鼠标进入此控件时，需要确定是否可以接受该拖放操作。

重新实现此函数，以便对其他 MIME 类型启用拖放支持。

----

**bool QTextEdit::canPaste() const**

当文本可以从剪切板复制到文本编辑器时返回 true 。

该函数在 Qt 4.2 中引入。

----

**void QTextEdit::changeEvent([QEvent](https://doc.qt.io/qt-5/qevent.html) \*e)**	[override virtual protected]

重写父类 QFrame 函数 [QFrame::changeEvent](https://doc.qt.io/qt-5/qframe.html#changeEvent)(QEvent *ev)。

----

----

**void QTextEdit::contextMenuEvent([QContextMenuEvent](https://doc.qt.io/qt-5/qcontextmenuevent.html) \**event*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::contextMenuEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#contextMenuEvent)(QContextMenuEvent *e) 。

显示由 [createStandardContextMenu](https://doc.qt.io/qt-5/qtextedit.html#createStandardContextMenu)() 创建的上下文菜单。

如果你不想编辑器有上下文菜单，你可以设置 [contextMenuPolicy](https://doc.qt.io/qt-5/qwidget.html#contextMenuPolicy-prop) 为 [Qt::NoContextMenu](https://doc.qt.io/qt-5/qt.html#ContextMenuPolicy-enum)。如果你想自定义上下文菜单可以重写该函数。如果要扩展标准上下文菜单，请重写此函数，调用 [createStandardContextMenu](https://doc.qt.io/qt-5/qtextedit.html#createStandardContextMenu)() 并扩展其返回的菜单。

事件通过 *event* 对象传入。

```c++
void MyTextEdit::contextMenuEvent(QContextMenuEvent *event)
{
    QMenu *menu = createStandardContextMenu();
    menu->addAction(tr("My Menu Item"));
    //...
    menu->exec(event->globalPos());
    delete menu;
}
```

----

**[QMimeData](https://doc.qt.io/qt-5/qmimedata.html) *QTextEdit::createMimeDataFromSelection() const**	[virtual protected]

此函数返回一个新的 MIME 数据对象，以表示文本编辑的当前选择的内容.当需要将选择内容封装到新的 QMimeData 对象中时，将调用该函数。例如，当进行拖放操作时，或将数据复制到剪贴板时。

如果重新实现此函数，请注意返回的 QMimeData 对象的所有权将会传递给调用方。选中的数据对象可以通过 [textCursor](https://doc.qt.io/qt-5/qtextedit.html#textCursor)() 找回。

-----

----

**[QMenu](https://doc.qt.io/qt-5/qmenu.html) *QTextEdit::createStandardContextMenu()**

该函数用于创建右键上下文菜单。由默认函数 [contextMenuEvent](https://doc.qt.io/qt-5/qtextedit.html#contextMenuEvent)() 调用。菜单的所有权会传递给调用者。

我们推荐使用 createStandardContextMenu([QPoint](https://doc.qt.io/qt-5/qpoint.html)) 来代替，这样会使操作与单击区域相关联。

----

**[QMenu](https://doc.qt.io/qt-5/qmenu.html) QTextEdit::createStandardContextMenu(const [QPoint](https://doc.qt.io/qt-5/qpoint.html) &*position*)**

该函数用于创建右键上下文菜单。它由默认函数 [contextMenuEvent](https://doc.qt.io/qt-5/qtextedit.html#contextMenuEvent)() 来调用，并且包含鼠标在文档中点击的坐标。这样可以让操作对用户的点击位置敏感。菜单的所有权会传递给调用者。

该函数在 Qt 4.4 引入。

----

**[QTextCharFormat](https://doc.qt.io/qt-5/qtextcharformat.html) QTextEdit::currentCharFormat() const**

返回插入新文本时使用的字符格式。

您也可以在 [setCurrentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#setCurrentCharFormat)() 中找到相关信息。

----

**[QFont](https://doc.qt.io/qt-5/qfont.html) QTextEdit::currentFont() const**

返回当前字体格式。

你也可以在 [setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)()、 [setFontFamily](https://doc.qt.io/qt-5/qtextedit.html#setFontFamily)() 和 [setFontPointSize](https://doc.qt.io/qt-5/qtextedit.html#setFontPointSize)() 中 找到相关信息。

----

**[QTextCursor](https://doc.qt.io/qt-5/qtextcursor.html) QTextEdit::cursorForPosition(const [QPoint](https://doc.qt.io/qt-5/qpoint.html) &*pos*) const**

返回 *pos*（视窗坐标）处的光标。

----

**[QRect](https://doc.qt.io/qt-5/qrect.html) QTextEdit::cursorRect(const [QTextCursor](https://doc.qt.io/qt-5/qtextcursor.html) &*cursor*) const**

返回包含 *cursor* 的矩形（视窗坐标）。

----

**[QRect](https://doc.qt.io/qt-5/qrect.html) QTextEdit::cursorRect() const**

返回包含文本编辑光标的矩形（视窗坐标）。

----

**void QTextEdit::dragEnterEvent([QDragEnterEvent](https://doc.qt.io/qt-5/qdragenterevent.html) *\*e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::dragEnterEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#dragEnterEvent)(QDragEnterEvent *event) 。

----

**void QTextEdit::dragLeaveEvent([QDragLeaveEvent](https://doc.qt.io/qt-5/qdragleaveevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::dragLeaveEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#dragLeaveEvent)(QDragLeaveEvent *event) 。

----

**void QTextEdit::dragMoveEvent([QDragMoveEvent](https://doc.qt.io/qt-5/qdragmoveevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::dragMoveEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#dragMoveEvent)(QDragMoveEvent *event) 。

----

**void QTextEdit::dropEvent([QDropEvent](https://doc.qt.io/qt-5/qdropevent.html) \**e*)**	[override virtual protected]

重写父类方法： [QAbstractScrollArea::dropEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#dropEvent)(QDropEvent *event) 。

----

**void QTextEdit::ensureCursorVisible()**

如有必要，通过滚动文本编辑确保光标可见。

----

**[QList](https://doc.qt.io/qt-5/qlist.html) \<[QTextEdit::ExtraSelection](https://doc.qt.io/qt-5/qtextedit-extraselection.html)> QTextEdit::extraSelections() const**

返回先前的额外选择集。

该函数在 Qt 4.2 中引入。

您也可以在 [setExtraSelections](https://doc.qt.io/qt-5/qtextedit.html#setExtraSelections)() 中找到相关信息。

----

**bool QTextEdit::find(const [QString](https://doc.qt.io/qt-5/qstring.html) &*exp*, [QTextDocument::FindFlags](https://doc.qt.io/qt-5/qtextdocument.html#FindFlag-enum) *options* = QTextDocument::FindFlags())**

通过给定选项 *options* 查找下一个 *exp* 字符串的匹配项。如果找到 *exp* 字符串则返回 true ，并使光标选中匹配项，如果未找到 则返回 false 。

----

**bool QTextEdit::find(const [QRegExp](https://doc.qt.io/qt-5/qregexp.html) &*exp*, [QTextDocument::FindFlags](https://doc.qt.io/qt-5/qtextdocument.html#FindFlag-enum) *options* = QTextDocument::FindFlags())**

该函数为重载函数。

通过给定选项 *options* 查找下一个匹配正则表达式 *exp* 的项。该重载函数会忽略 [QTextDocument::FindCaseSensitively](https://doc.qt.io/qt-5/qtextdocument.html#FindFlag-enum) 选项，希望大小写敏感时需要使用 [QRegExp::caseSensitivity](https://doc.qt.io/qt-5/qregexp.html#caseSensitivity) 代替。

如果找到匹配 *exp* 的字符串则返回 true，并使光标选中匹配项，如果未找到则返回 false。

该函数在 Qt 5.3 中引入。

----

**bool QTextEdit::find(const [QRegularExpression](https://doc.qt.io/qt-5/qregularexpression.html) &*exp*, [QTextDocument::FindFlags](https://doc.qt.io/qt-5/qtextdocument.html#FindFlag-enum) *options* = QTextDocument::FindFlags())**

该函数为重载函数。

通过给定选项 *options* 查找下一个匹配正则表达式 exp 的项。该重载函数会忽略 [QTextDocument::FindCaseSensitively](https://doc.qt.io/qt-5/qtextdocument.html#FindFlag-enum) 选项，希望大小写敏感时需要使用  [QRegularExpression](https://doc.qt.io/qt-5/qregularexpression.html#PatternOption-enum)::[CaseInsensitiveOption](https://doc.qt.io/qt-5/qregularexpression.html#PatternOption-enum)代替。

如果找到匹配 *exp* 的字符串则返回 true ，并使光标选中匹配项，如果未找到则返回 false 。

该函数在 Qt 5.13 中引入。

----

**void QTextEdit::focusInEvent([QFocusEvent](https://doc.qt.io/qt-5/qfocusevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QWidget::focusInEvent](https://doc.qt.io/qt-5/qwidget.html#focusInEvent)(QFocusEvent *event) 。

----

**bool QTextEdit::focusNextPrevChild(bool *next*)**	[override virtual protected]

重写父类函数： [QWidget::focusNextPrevChild](https://doc.qt.io/qt-5/qwidget.html#focusNextPrevChild)(bool next) 。

----

**void QTextEdit::focusOutEvent([QFocusEvent](https://doc.qt.io/qt-5/qfocusevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QWidget::focusOutEvent](https://doc.qt.io/qt-5/qwidget.html#focusOutEvent)(QFocusEvent *event) 。

----

**[QString](https://doc.qt.io/qt-5/qstring.html) QTextEdit::fontFamily() const**

返回当前字体系列。

您也可以在 [setFontFamily](https://doc.qt.io/qt-5/qtextedit.html#setFontFamily)() 、 [setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)() 和 [setFontPointSize](https://doc.qt.io/qt-5/qtextedit.html#setFontPointSize)() 中找到相关信息。

----

**bool QTextEdit::fontItalic() const**

如果当前字体为斜体则返回 true ，否则返回 false 。

您也可以在 [setFontItalic](https://doc.qt.io/qt-5/qtextedit.html#setFontItalic)() 中找到相关信息。

----

**[qreal](https://doc.qt.io/qt-5/qtglobal.html#qreal-typedef) QTextEdit::fontPointSize() const**

返回当前字体的点大小。

您也可以在 [setFontFamily](https://doc.qt.io/qt-5/qtextedit.html#setFontFamily)()、 [setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)() 和 [setFontPointSize](https://doc.qt.io/qt-5/qtextedit.html#setFontPointSize)() 中找到相关信息。

----

----

**bool QTextEdit::fontUnderline() const**

如果当前字体有下划线则返回 true ，否则返回 false 。

您也可以在 [setFontUnderline](https://doc.qt.io/qt-5/qtextedit.html#setFontUnderline)() 中找到相关信息。

----

-----

**int QTextEdit::fontWeight() const**

返回当前字体的粗细。

您也可以在 [setFontWeight](https://doc.qt.io/qt-5/qtextedit.html#setFontWeight)() 、 [setCurrentFont](https://doc.qt.io/qt-5/qtextedit.html#setCurrentFont)() 、 [setFontPointSize](https://doc.qt.io/qt-5/qtextedit.html#setFontPointSize)() 和 [QFont::Weight](https://doc.qt.io/qt-5/qfont.html#Weight-enum) 中找到相关信息。

----

----

**void QTextEdit::inputMethodEvent([QInputMethodEvent](https://doc.qt.io/qt-5/qinputmethodevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QWidget::inputMethodEvent](https://doc.qt.io/qt-5/qwidget.html#inputMethodEvent)(QInputMethodEvent *event) 。

----

----

**[QVariant](https://doc.qt.io/qt-5/qvariant.html) QTextEdit::inputMethodQuery([Qt::InputMethodQuery](https://doc.qt.io/qt-5/qt.html#InputMethodQuery-enum) *property*) const**	[override virtual]

重写父类函数：  [QWidget::inputMethodQuery](https://doc.qt.io/qt-5/qwidget.html#inputMethodQuery)(Qt::InputMethodQuery query) const 。

----

----

**void QTextEdit::insertFromMimeData(const [QMimeData](https://doc.qt.io/qt-5/qmimedata.html) *\*source*)**	[virtual protected]

此函数将 *source* 指定的 MIME 数据对象的内容插入到为文本编辑器的当前光标位置中。当从剪切板粘贴文本或者编辑器接收拖放时都会调用该函数。

重新实现此函数，以便对其他 MIME 类型启用拖放支持。

----

----

**void QTextEdit::keyPressEvent([QKeyEvent](https://doc.qt.io/qt-5/qkeyevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::keyPressEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#keyPressEvent)(QKeyEvent *e) 。

----

**void QTextEdit::keyReleaseEvent([QKeyEvent](https://doc.qt.io/qt-5/qkeyevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QWidget::keyReleaseEvent](https://doc.qt.io/qt-5/qwidget.html#keyReleaseEvent)(QKeyEvent *event) 。

----

**[QVariant](https://doc.qt.io/qt-5/qvariant.html) QTextEdit::loadResource(int *type*, const [QUrl](https://doc.qt.io/qt-5/qurl.html) &*name*)**	[virtual]

由给定的 *type* 和 *name* 加载资源。

该函数是 [QTextDocument::loadResource](https://doc.qt.io/qt-5/qtextdocument.html#loadResource)() 的扩展。

注意：可以通过元对象系统和 QML 调用此函数。参考 [Q_INVOKABLE](https://doc.qt.io/qt-5/qobject.html#Q_INVOKABLE) 。

您也可以在 [QTextDocument::loadResource](https://doc.qt.io/qt-5/qtextdocument.html#loadResource)() 中找到相关信息。

----

**void QTextEdit::mergeCurrentCharFormat(const [QTextCharFormat](https://doc.qt.io/qt-5/qtextcharformat.html) &*modifier*)**

通过在编辑器光标对象调用 [QTextCursor::mergeCharFormat](https://doc.qt.io/qt-5/qtextcursor.html#mergeCharFormat) ，将 *modifier* 中指定的属性合并到当前字符格式中。

如果编辑器中有选中内容，则 *modifier* 的属性将直接应用于所选内容。

您也可以在 [QTextCursor::mergeCharFormat](https://doc.qt.io/qt-5/qtextcursor.html#mergeCharFormat)() 中找到相关信息。

----

**void QTextEdit::mouseDoubleClickEvent([QMouseEvent](https://doc.qt.io/qt-5/qmouseevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::mouseDoubleClickEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#mouseDoubleClickEvent)(QMouseEvent *e) 。

----

**void QTextEdit::mouseMoveEvent([QMouseEvent](https://doc.qt.io/qt-5/qmouseevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::mouseMoveEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#mouseMoveEvent)(QMouseEvent *e) 。

----

**void QTextEdit::mousePressEvent([QMouseEvent](https://doc.qt.io/qt-5/qmouseevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::mousePressEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#mousePressEvent)(QMouseEvent *e) 。

----

**void QTextEdit::mouseReleaseEvent([QMouseEvent](https://doc.qt.io/qt-5/qmouseevent.html) \**e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::mouseReleaseEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#mouseReleaseEvent)(QMouseEvent *e) 。

----

**void QTextEdit::moveCursor([QTextCursor::MoveOperation](https://doc.qt.io/qt-5/qtextcursor.html#MoveOperation-enum) *operation*, [QTextCursor::MoveMode](https://doc.qt.io/qt-5/qtextcursor.html#MoveMode-enum) *mode* = QTextCursor::MoveAnchor)**

通过给定的 *operation* 操作来移动光标。

如果 mode 是 [QTextCursor::KeepAnchor](https://doc.qt.io/qt-5/qtextcursor.html#MoveMode-enum)，光标选中它移动过的文本。效果相当于用户按住 Shift 键并移动光标。

该函数在 Qt 4.2 中引入。

您也可以在 [QTextCursor::movePosition](https://doc.qt.io/qt-5/qtextcursor.html#movePosition)() 中找到相关信息。

----

**void QTextEdit::paintEvent([QPaintEvent](https://doc.qt.io/qt-5/qpaintevent.html) *\*event*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::paintEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#paintEvent)(QPaintEvent *event) 。

可以在子类中重新实现该函数，以接收事件对象中传递的绘制事件。通常没有必要在 QTextEdit 的子类中重新实现此函数。

注意：不得通过该函数的重写函数修改文本文档。

----

**void QTextEdit::print([QPagedPaintDevice](https://doc.qt.io/qt-5/qpagedpaintdevice.html) *\*printer*) const**

该函数将文本传输给指定打印机打印。这相当于直接调用文档上的打印方法，只是此函数还支持 QPrinter::Selection 为打印范围。

该函数在 Qt 4.3 中引入。

您也可以在 [QTextDocument::print](https://doc.qt.io/qt-5/qtextdocument.html#print)() 找到相关信息。

----

**void QTextEdit::resizeEvent([QResizeEvent](https://doc.qt.io/qt-5/qresizeevent.html) *\*e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::resizeEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#resizeEvent)(QResizeEvent *event) 。

----

**void QTextEdit::scrollContentsBy(int *dx*, int *dy*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::scrollContentsBy](https://doc.qt.io/qt-5/qabstractscrollarea.html#scrollContentsBy)(int dx, int dy) 。

----

**void QTextEdit::setCurrentCharFormat(const [QTextCharFormat](https://doc.qt.io/qt-5/qtextcharformat.html) &*format*)**

当在文本编辑器的光标处插入新文本时调用 [QTextCursor::setCharFormat](https://doc.qt.io/qt-5/qtextcursor.html#setCharFormat)() 来设置字符格式。如果编辑器选中了文本，则会将字符格式应用于选中的文本。

您也可以在 [currentCharFormat](https://doc.qt.io/qt-5/qtextedit.html#currentCharFormat)() 中找到相关信息。

----

**void QTextEdit::setExtraSelections(const [QList](https://doc.qt.io/qt-5/qlist.html) \<[QTextEdit::ExtraSelection](https://doc.qt.io/qt-5/qtextedit-extraselection.html)> &*selections*)**

该函数允许在文档中的特定区域临时设置由 *selections* 指定的颜色。例如，在编程编辑器中，使用给定背景颜色标记整行文本以指示断点是否存在时非常有用。

该函数在 Qt 4.2 中引入。

您也可以在 [QTextEdit::ExtraSelection](https://doc.qt.io/qt-5/qtextedit-extraselection.html) 和 [extraSelections](https://doc.qt.io/qt-5/qtextedit.html#extraSelections)() 中找到相关信息。

----

**void QTextEdit::setTextCursor(const [QTextCursor](https://doc.qt.io/qt-5/qtextcursor.html) &*cursor*)**

设置可见光标。

您也可在 [textCursor](https://doc.qt.io/qt-5/qtextedit.html#textCursor)() 中找到相关信息。

----

**void QTextEdit::showEvent(*QShowEvent* \*)**	[override virtual protected]

重写父类函数： [QWidget::showEvent](https://doc.qt.io/qt-5/qwidget.html#showEvent)(QShowEvent *event) 。

----

**[QColor](https://doc.qt.io/qt-5/qcolor.html) QTextEdit::textBackgroundColor() const**

返回当前格式的文本背景颜色。

该函数在 Qt 4.4 中引入。

您也可以在 [setTextBackgroundColor](https://doc.qt.io/qt-5/qtextedit.html#setTextBackgroundColor)() 。

----

**[QColor](https://doc.qt.io/qt-5/qcolor.html) QTextEdit::textColor() const**

返回当前格式的文本颜色。

您也可以在 [setTextColor](https://doc.qt.io/qt-5/qtextedit.html#setTextColor)() 中找到相关信息。

----

**[QTextCursor](https://doc.qt.io/qt-5/qtextcursor.html) QTextEdit::textCursor() const**

返回表示当前可见光标的 QTextCursor 的副本。请注意，返回的光标上做的更改不会影响 QTextEdit 实际光标。使用 setTextCursor()  更新可见光标。

您也可以在 [setTextCursor](https://doc.qt.io/qt-5/qtextedit.html#setTextCursor)() 中找到相关信息。

----

**[QString](https://doc.qt.io/qt-5/qstring.html) QTextEdit::toPlainText() const**

将编辑器文本返回为纯文本。

注意：该函数用来获取属性字段 [plainText](https://doc.qt.io/qt-5/qtextedit.html#plainText-prop) 的值。

您也可以在 [QTextEdit::setPlainText](https://doc.qt.io/qt-5/qtextedit.html#setPlainText)() 中找到相关信息。

----

**void QTextEdit::wheelEvent([QWheelEvent](https://doc.qt.io/qt-5/qwheelevent.html) *\*e*)**	[override virtual protected]

重写父类函数： [QAbstractScrollArea::wheelEvent](https://doc.qt.io/qt-5/qabstractscrollarea.html#wheelEvent)(QWheelEvent *e) 。

----

----