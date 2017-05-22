# 开发说明
## 对照

基本命名方式是
BibDisplay + 字段 + 限定
例如BibDisplayAuthorInterview指的是Interview里面的Author字段

|中文|英文|代码|
|:-:|:-:|:-:|
|书籍 |Book| `$SourceType = 'Book'` |
|书籍章节 |BookSection| `$SourceType = 'BookSection'` |
|杂志文章 |JournalArticle|  `$SourceType = 'JournalArticle'` |
|期刊文章 |ArticleInAPeriodical|  `$SourceType = 'ArticleInAPeriodical'` |
|会议记录 |ConferenceProceedings| `$SourceType = 'ConferenceProceedings'` |
|报告 |Report| `$SourceType = 'Report'` |
|录音 |SoundRecording| `$SourceType = 'SoundRecording'` |
|表演 |Performance| `$SourceType = 'Performance'` |
|艺术作品 |Art| `$SourceType = 'Art'` |
|网站文档 |DocumentFromInternetSite| `$SourceType = 'DocumentFromInternetSite'` |
|网站 |InternetSite| `$SourceType = 'InternetSite'` |
|电影 |Film| `$SourceType = 'Film'` |
|采访 |Interview| `$SourceType = 'Interview'` |
|专利 |Patent| `$SourceType = 'Patent'` |
|案例 |Case| `$SourceType = 'Case'` |
|杂项 |Misc| `$SourceType = 'Misc'` |

其他字段

|用途或Word中的名称|代码或模板名|
|:-:|:-:|
| 输出空格 | templ_prop_Space 或 `<span> </span>`|
| 输出句号 | templ_prop_Dot 或 `<span>,</span>`|
| 输出逗号 | templ_prop_ListSeparator |
| 公司作者 |cCorporateAuthors|
| 作者之间的分隔符 | templ_str_AndUnCap |
| 显示杂志文章/期刊文章的作者 | BibDisplayAuthorJArtcicle |
| 显示杂志文章/期刊文章/网站文档/网站的年月日等信息 | BibDisplayDayMonthYearWebSiteJournal |
| 显示杂志文章/期刊文章页码 | BibDisplayPagesJournal 调用 DisplayPageOrPages |
| 显示杂志/期刊卷号 | BibDisplayVolumeJournal |
| 显示杂志/期刊期号 | BibDisplayIssueJournal |
| 显示杂志/期刊名字 | BibDisplayJournalName/BibDisplayJournalNameAP |
| 显示杂志文章/期刊文章名字 | BibDisplayTitleJournal/BibDisplayTitleAP |

在一些模板中出现的`/*/b:Locals/b:Local[@LCID=$_LCID]/b:Strings/`字段是和当前语言环境有关的字符串，例如连接符“和”，“卷”等