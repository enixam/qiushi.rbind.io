
---
title: "R for data science: tidyverse and beyond"
knit: "bookdown::render_book"
author: "Maxine"
date: "2020-01-17"
site: bookdown::bookdown_site
documentclass: book
github-repo: enixam/rfordatascience
bibliography: [packages.bib, references.bib]
biblio-style: "apalike"
link-citations: true
nocite: |
  @R-base
---


# 前言 {#preface .unnumbered}  

这份笔记最初源自于对 [R for Data Science](https://r4ds.had.co.nz)[@wickham2016r]的学习,其中第 \@ref(tibble) 章和第 \@ref(purrr) 章还包含了许多 [Advanced R](https://adv-r.hadley.nz/) 中相应章节的内容。  

限于篇幅， R for Data Sciecne 的内容聚焦于对 [**tidyverse**](https://www.tidyverse.org/) 核心包的讲解，难免遗漏了一些同样很实用的 tidyverse 包，如 [**rvest**](https://rvest.tidyverse.org/)、 [**DBI**](https://dbi.r-dbi.org/)等。一些 tidyverse 包在本书出版后的重大更新，如 [**tidyr 1.0.0**](https://www.tidyverse.org/blog/2019/09/tidyr-1-0-0/)，自然也没有被收录。  

另一方面，当下的 R 社区发展迅猛，一大批更为好用、高效的 R 包也在不断涌现，既有 Rstudio 旗下 tidyverse 的衍生系列(如 [**tidymodels**](https://www.tidyverse.org/blog/2018/08/tidymodels-0-0-1/)), 也有 "民间" 的贡献（如 [**data.table**](https://rdatatable.gitlab.io/data.table/)）。虽然学海无涯，作为学习者总还是希望能够多掌握一些，多明白一些。于是便希望这份笔记不限于原书，而是能记录一些其他自学 R 与数据科学实践的内容，最大的受益者自然是自己啦。

鉴于笔者没有经历过统计、计算机等专业的系统学习，似乎连“才疏学浅”这样的谦辞也成为一种过誉。无论如何，若发现了任何错误或有任何方面的意见，欢迎在 https://github.com/enixam/rfordatascience/issues 提交 issue 或者通过邮箱 565702994@qq.com 与我联系。  

第 \@ref(dplyr) ~ \@ref(purrr) 章的文字表述借鉴了中文译本。目前对原书中内容的再现和扩展（第一部分）已经基本完成(除了 **ggplot2** 相关部分)，随缘更新。    

绝大部分代码需要首先加载 tidyverse, 其中包含的 R 包默认已经被加载好 : 


```r
library(tidyverse)
```
