section 字面上理解为“块”，“部分”，section元素代表一个页面或一个内容块的部分，一般作为主题块列表，在html5网页中表现的意思跟字面理解差不多，即部分，块，模块，主要作用为对页面的内容进行分块或者对文章的内容进行分段。
# div，section和article的区别
语义从左到右逐渐增强
div无任何语义，仅作为样式化或者脚本化的标签
section适用于一段主题性的内容
article适用于完整的独立存在的一段内容
section标签是成对出现的,以<section>开始,以</section>结束
section标签通常带有一个标题和一个内容块。

一、section标签实例

<!doctype html>
<article>
    <h1>Web编程语言比较</h1>
    <p>web编程语言常用的有asp,asp.net,php,jsp...</p>
    <section>
        <h2>asp</h2>
        <p>asp全称Active Server Page</p>
    </section>
    <section>
        <h2>asp.net</h2>
        <p>asp的颠覆版本</p>
    </section>
    <section>
        <h2>php</h2>
        <p>草根动态语言，免费，强大</p>
    </section>
</article>
二、article与section的异同
section和article可以互相嵌套，也就是说他们没有上下级关系，section可以包含article，article也可以包含section。
感觉上使用都差不多，都可以有h1,h2,h3,都有一个主体，那应该怎么来区分它们的不同？其实很简单，只要从字面上理解它们就可以足够了：
1、article是文章，文章就是一段完整的独立的内容。
2、section就是块，某种意义上可以理解为div，但是比div的意思更加明确一点。

三、section和div的异同
1、section和div都可以对内容进行分块，但是section是进行有意义的分块，无意义的分块应该由div来做，例如用作设置样式的页面容器。
2、section内部必须有标题，标题也代表了section的意义所在。

四、使用<section>标签需要注意的地方
1、不要将<section>作为用来设置样式或行为的“钩子”容器，那是<div>的工作。
2、如果<article>、<aside>或<nav>更符合状况，不要使用<section>。
3、不要为没有标题的内容区块使用<section>。