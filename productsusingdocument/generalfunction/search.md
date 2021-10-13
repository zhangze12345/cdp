# 搜索

## 搜索功能界面概览

![搜索功能界面](../../.gitbook/assets/界面.gif)

## 搜索的作用

在用户洞察平台中，搜索功能为全局的通用功能，在所有功能页面的右上角，都设有搜索按钮，点击搜索按钮后将会弹出搜索条件配置框，目前搜索功能支持**用户ID**以及**全部用户属性**。

通过搜索功能，使用者可以快速的定位到某个用户，或者筛选出一批用户。

## 搜索的使用方法

使用搜索时，根据搜索条件的不同，使用方法也有所不同：

### 以用户ID进行搜索

点击搜索按钮，在搜索条件配置框的左侧选择用户ID，在右侧输入框内输入对应的内容，点击搜索按钮即可开始搜索并展示出结果。

对用户ID进行搜索时支持模糊搜索，例如存在三个用户，其用户ID分别为A123，B123，C123，此时如果通过**123**进行搜索时，点击搜索按钮，这三个用户都会展示在搜索结果中。

### 以布尔类型的用户属性进行搜索

在搜索条件配置框左侧选择某个布尔类型的用户属性时，配置框右侧的输入框将转化为下拉选项框，分别有四个选项：

{% hint style="info" %}
为真：对应属性值为True的用户。

为假：对应属性值为False的用户。

有值：对应属性值中有值的用户。

没值：对应属性值中无值的用户。
{% endhint %}

{% hint style="danger" %}
属性值如果为NULL，不属于没值
{% endhint %}

例如搜索**会员用户**，可以搜索**是否为会员-为真**，如果需要搜索**非会员**，则可以搜索**是否为会员-为假**。

### 以日期时间类型的用户属性进行搜索

在搜索条件配置框左侧选择某个日期时间类型的用户属性时，配置框右侧的输入框将转化为下图所示的组合筛选器：

![以日期时间类型的用户属性进行搜索](../../.gitbook/assets/以日期时间类型的用户属性进行搜索.gif)

组合筛选器中所有可选组合如下：

| 选择序列 | 可选组合内容                        |
| ---- | ----------------------------- |
| 1    | 相对当前时间点-过去-【输入值】-之前           |
| 2    | 相对当前时间点-过去-【输入值】-之内           |
| 3    | 相对当前时间点-未来-【输入值】-之前           |
| 4    | 相对当前时间点-未来-【输入值】-之内           |
| 5    | 相对当前时间区间-过去-【输入值】-天至-【输入值】-之内 |
| 6    | 相对当前时间区间-未来-【输入值】-天至-【输入值】-之内 |
| 7    | 绝对时间-等于-【选择日期】                |
| 8    | 绝对时间-不等于-【选择日期】               |
| 9    | 绝对时间-大于-【选择日期】                |
| 10   | 绝对时间-大于等于-【选择日期】              |
| 11   | 绝对时间-小于-【选择日期】                |
| 12   | 绝对时间-小于等于-【选择日期】              |
| 13   | 绝对时间-区间-【选择日期】-至-【选择日期】       |
| 14   | 有值                            |
| 15   | 没值                            |

例如搜索出**会员服务在未来一周内即将到期的用户**，可以搜索**会员到期日-相对当前时间点-未来-7-之内**。

### 以数值类型的用户属性进行搜索

在搜索条件配置框左侧选择某个日期时间类型的用户属性时，配置框右侧的输入框将转化为下图所示的数值筛选器：

![以数值类型的用户属性进行搜索](../../.gitbook/assets/以数值类型的用户属性进行搜索.gif)

数值筛选器中所有可选组合如下：

| 选择序列 | 可选组合内容          |
| ---- | --------------- |
| 1    | 等于-【输入值】        |
| 2    | 不等于-【输入值】       |
| 3    | 大于-【输入值】        |
| 4    | 小于-【输入值】        |
| 5    | 有值              |
| 6    | 没值              |
| 7    | 区间-【输入值】-至【输入值】 |

### 以字符串类型的用户属性进行搜索

与以用户ID进行搜索时的规则相同。