
# 中文 Julia 笔记

> 版本：0.0.1<br>
> 作者：詹子知<br>
> 邮件：zhiqiangzhan@gmail.com <br />

`Github` 加载 `.ipynb` 的速度较慢，建议在 [Nbviewer](http://nbviewer.jupyter.org/github/jameszhan/notes-julia/tree/master/index.ipynb) 中查看该项目。


## 简介

部分内容来自网络。

默认安装了 `Ruby 2.4.1`，以及相关的第三方包 `bundler`， `iruby`。

为了更好地使用 [Jupyter NoteBook](http://nbviewer.jupyter.org/)，推荐安装 `jupyter`, 推荐使用 [Anaconda](https://www.anaconda.com/download/)。


安装好 `Ruby` 和相应的包之后，可以在命令行下输入：

```bash
git clone https://github.com/jameszhan/notes-ruby.git
cd notes-ruby
bundle update
```

启动笔记本

```bash
iruby notebook .
```

或者

```bash
jupyter notebook .
```

## 参考
- [Julia 官网][julia-official-website]
- [Julia 文档][julia-docs]
- [Julia 元编程][julia-metaprogramming]
- [Julia Style Guide][julia-style-guide]
- [Julia language: a concise tutorial][julia-gitbook]


## 生成静态文件

可以在 Notebook 中打开 `generate-static-files.ipynb` 来生成静态的 HTML 文件。

使用命令行工具生成。

```bash
gem install thor

chmod +x generate


# 默认生成 markdown 文件到 static-files 目录
./generate static

# 生成 pdf 文件到 static-files 目录
./generate static --to pdf  

# 生成 html 文件到 generated 目录
./generate static --to html --output=generated 
```

## 目录

- [01. **Julia 快速概览**](01-julia-overview)
	- [01.01.**Julia 简介**](01-julia-overview/01.01-julia-overview.ipynb)
	- [01.02.**20分钟体验 Ruby**](01-julia-overview/01.02-julia-in-20-minutes.ipynb)
	- [01.03.**从其它语言到 Ruby**](01-julia-overview/01.03-julia-from-other-languages.ipynb)
- [02. **Julia 基础**](02-julia-basics)
	- [02.01.**Julia 数据类型**](02-julia-basics/02.01-types.ipynb)
	- [02.02.**数字**](02-julia-basics/02.02-numbers.ipynb)
	- [02.03.**字符串**](02-julia-basics/02.03-strings.ipynb)
	- [02.04.**符号**](02-julia-basics/02.04-symbols.ipynb)
	- [02.05.**正则表达式**](02-julia-basics/02.05-regular-expression.ipynb)
	- [02.06.**列表**](02-julia-basics/02.06-arrays.ipynb)
	- [02.07.**Hash**](02-julia-basics/02.07-hashes.ipynb)
	- [02.08.**范围 (Range)**](02-julia-basics/02.08-ranges.ipynb)
- [03. **Julia 语法进阶**](03-julia-syntax)
	- [03.01.**Julia 赋值机制**](03-julia-syntax/03.01-assignment-statements.ipynb)
	- [03.02.**判断语句**](03-julia-syntax/03.02-conditional-statements.ipynb)
	- [03.03.**循环**](03-julia-syntax/03.03-loop-statements.ipynb)
	- [03.04.**迭代器**](03-julia-syntax/03.04-iterators.ipynb)
	- [03.05.**函数**](03-julia-syntax/03.05-functions.ipynb)
	- [03.06.**代码块**](03-julia-syntax/03.06-blocks.ipynb)
	- [03.07.**变量作用域**](03-julia-syntax/03.07-scope.ipynb)
	- [03.09.**异常**](03-julia-syntax/03.09-exceptions.ipynb)
	- [03.10.**Julia 元编程技巧**](03-julia-syntax/03.10-julia-meta-programming.ipynb)
	- [03.11.**Julia 代码风格**](03-julia-syntax/03.11-julia-style-guide.ipynb)
- [04. **Julia 面向对象编程**](04-julia-oop)
- [05. **Julia 在机器学习上的应用**](05-julia-on-ml)


[julia-official-website]: https://julialang.org/ "Julia 官网"
[julia-docs]: https://docs.julialang.org "Julia 文档"
[julia-style-guide]: https://docs.julialang.org/en/v1/manual/style-guide/index.html "Julia Style Guide"
[julia-metaprogramming]: https://docs.julialang.org/en/v1/manual/metaprogramming/ "Julia 元编程"
[julia-gitbook]: https://syl1.gitbook.io/julia-language-a-concise-tutorial/ "Julia language: a concise tutorial"