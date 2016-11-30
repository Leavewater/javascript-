#Array

##concat()

- 用于连接两个或多个数组。
- 语法 array1.concat(array2,array3,...,arrayX)
  - array2, array3, ..., arrayX	必需。该参数可以是具体的值，也可以是数组对象。可以是任意多个。
- 返回值：Array 对象	返回一个新的数组。该数组是通过把所有 arrayX 参数添加到 arrayObject 中生成的。
  如果要进行 concat() 操作的参数是数组，那么添加的是数组中的元素，而不是数组。


##indexOf()

- 用法和string类似

##lastIndexOf()

- 用法和string类似

##pop()

- 用于删除并返回数组的最后一个元素。
- 语法：array.pop()
- 返回：所有类型*	The removed array item
- ！！！此方法改变数组的长度

##push()

- 向数组的末尾添加一个或多个元素，并返回新的长度。
- 语法 array.push(item1, item2, ..., itemX)
  - item1, item2, ..., itemX	必需。要添加到数组的元素。
- 返回值：Number	数组新长度
- ！！！此方法改变数组的长度。

##reverse()

- 用于颠倒数组中元素的顺序。
- 语法 array.reverse()
- ！！！这种方法会改变原始数组

##shift()

- 用于把数组的第一个元素从其中删除，并返回第一个元素的值。
- 语法：array.shift()
- 返回值：任何类型
- ！！！此方法改变数组的长度

##slice()

- 和数组方法类似

##sort()

- 用于对数组的元素进行排序。
- 默认排序顺序为按字母升序。

##splice()

- 用于插入、删除或替换数组的元素。
- 语法 array.splice(index,howmany,item1,.....,itemX)
  - index	必需。规定从何处添加/删除元素。该参数是开始插入和（或）删除的数组元素的下标，必须是数字。
  - howmany	必需。规定应该删除多少元素。必须是数字，但可以是 "0"。如果未规定此参数，则删除从 index 开始到原数组结尾的所有元素。
  - item1, ..., itemX	可选。要添加到数组的新元素
- 返回值：Array	如果从 arrayObject 中删除了元素，则返回的是含有被删除的元素的数组。
- ！！！这种方法会改变原始数组

##join()

- 用于把数组中的所有元素转换一个字符串。
- 语法 array.join(separator)
  - separator	可选。指定要使用的分隔符。如果省略该参数，则使用逗号作为分隔符。
- 返回值：String	返回一个字符串。该字符串是通过把 arrayObject 的每个元素转换为字符串，然后把这些字符串连接起来，在两个元素之间插入 separator 字符串而生成的。

##toString()

- 把数组转换为字符串，并返回结果。
- 数组中的元素之间用逗号分隔。
- 语法 array.toString()
- 返回值：String	数组的所有值用逗号隔开

##unshift()

- 向数组的开头添加一个或更多元素，并返回新的长度。
- 语法 array.unshift(item1,item2, ..., itemX)
  - item1,item2, ..., itemX	可选。向数组起始位置添加一个或者多个元素。
- ！！！该方法将改变数组的数目。
- IE8及更早IE版本不支持。


# String

##chartAt()

- 用于返回指定位置的字符
- 语法：string.charAt(index)
  - index，必需。表示字符串中某个位置的数字，即字符在字符串中的位置。
- 返回值：string，返回在指定位置的字符。

##concat()

- 用于连接两个或多个字符串
- 语法：string.concat(string1, string2, ..., stringX)
  - string1,string2...必需。将被连接为一个字符串的一个或多个字符串对象。
- 返回：string，两个或多个字符串连接后生成的新字符串。

##indexOf()

- 返回某个指定的字符串值在字符串中首次出现的位置
- 语法：string.indexOf(searchvalue,start)
  - searchvalue，必需。规定需检索的字符串值。
  - start，可选的整数参数。规定在字符串中开始检索的位置。它的合法取值是 0 到 string Object.length - 1。
    如省略该参数，则将从字符串的首字符开始检索。
- 返回值：number,查找指定字符串第一次出现的位置，如果没找到匹配的字符串则返回 -1。

##lastIndexOf()

- 返回一个指定的字符串值最后出现的位置，在一个字符串中的指定位置从后向前搜索。
- 语法：string.lastIndexOf(searchvalue,start)
  - searchvalue	必需。规定需检索的字符串值。
  - start	可选的整数参数。规定在字符串中开始检索的位置。它的合法取值是 0 到 stringObject.length - 1。
  如省略该参数，则将从字符串的最后一个字符处开始检索。
- 返回值：Number，查找的字符串最后出现的位置，如果没有找到匹配字符串则返回 -1。

##match()

- 在字符串内检索指定的值，或找到一个或多个正则表达式的匹配。
- 语法：string.match(regexp)
  - regexp	必需。规定要匹配的模式的 RegExp 对象。
    如果该参数不是 RegExp 对象，则需要首先把它传递给 RegExp 构造函数，将其转换为 RegExp 对象。
- 返回值：Array	存放匹配结果的数组。该数组的内容依赖于 regexp 是否具有全局标志 g。 
  如果没找到匹配结果返回 null 。

##replace()

- 用于在字符串中用一些字符替换另一些字符，或替换一个与正则表达式匹配的子串
- 语法：string.replace(searchvalue,newvalue)
  - searchvalue	必须。规定子字符串或要替换的模式的 RegExp 对象。
    请注意，如果该值是一个字符串，则将它作为要检索的直接量文本模式，而不是首先被转换为 RegExp 对象。
  - newvalue	必需。一个字符串值。规定了替换文本或生成替换文本的函数。
- 返回值：String	一个新的字符串，是用 replacement 替换了 regexp 的第一次匹配或所有匹配之后得到的。

##search()

- 用于检索字符串中指定的子字符串，或检索与正则表达式相匹配的子字符串。
- 语法: string.search(searchvalue)
  - searchvalue	必须。查找的字符串或者正则表达式
- 返回值Number,与指定查找的字符串或者正则表达式相匹配的 String 对象起始位置。

##slice()

- 提取字符串的某个部分，并以新的字符串返回被提取的部分，如果是负数，则该参数规定的是从字符串的尾部开始算起的位置。也就是说，-1 指字符串的最后一个字符，-2 指倒数第二个字符，以此类推。
- 语法string.slice(start,end)
  - start	必须. 要抽取的片断的起始下标。第一个字符位置为 0
  - end	可选。 紧接着要抽取的片段的结尾的下标。若未指定此参数，则要提取的子串包括 start 到原字符串结尾的字符串。
  如果该参数是负数，那么它规定的是从字符串的尾部开始算起的位置。
- 返回值：String，提取的字符串的一部分。

##substring()

- 用于提取字符串中介于两个指定下标之间的字符。
- 返回的子串包括 开始 处的字符，但不包括 结束 处的字符。
- 语法：string.substring(from, to)
  - from	必需。一个非负的整数，规定要提取的子串的第一个字符在 string Object 中的位置。
  - to	可选。一个非负的整数，比要提取的子串的最后一个字符在 string Object 中的位置多 1。
       如果省略该参数，那么返回的子串会一直到字符串的结尾。
- 返回值：String，提取的字符串的一部分。

##substring和slice区别

- slice参数可负，slice(-2)从倒数0到-2位置
- slice(-5,-2): 从倒数第5到倒数第2
- substring参数如为负则实际为0

##splict()

- 用于把一个字符串分割成字符串数组
- 语法 string.split(separator,limit)
  - separator	可选。字符串或正则表达式，从该参数指定的地方分割 string Object。
  - limit	可选。该参数可指定返回的数组的最大长度。如果设置了该参数，返回的子串不会多于这个参数指定的数组。
    如果没有设置该参数，整个字符串都会被分割，不考虑它的长度。
- 返回值：Array	一个字符串数组。该数组是通过在 separator 指定的边界处将字符串 string Object 
  分割成子串创建的。返回的数组中的字串不包括 separator 自身。

##substr()

- 在字符串中抽取从 开始 下标开始的指定数目的字符。
- 语法：string.substr(start,length)
  - start	必需。要抽取的子串的起始下标。必须是数值。如果是负数，那么该参数声明从字符串的尾部开始算起的位置。
    也就是说，-1 指字符串中最后一个字符，-2 指倒数第二个字符，以此类推。
  - length	可选。子串中的字符数。必须是数值。如果省略了该参数，那么返回从 stringObject 的开始位置到结尾的字串。
- 返回值：string, 一个包含文本提取部分的新字符串

##trim()

- 去除字符串两边的空白
- 语法：string.trim()
