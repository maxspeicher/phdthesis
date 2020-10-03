# Search Interaction Optimization: A Human-Centered Design Approach

## Abstract

Over the past 25 years, search engines have become one of the most important, if not *the* entry point of the World Wide Web. This development has been primarily due to the continuously increasing amount of available documents, which are highly unstructured. Moreover, the general trend is towards classifying search results into categories and presenting them in terms of semantic information that answer users' queries without having to leave the search engine. With the growing amount of documents and technological enhancements, the needs of users as well as search engines are continuously evolving. Users want to be presented with increasingly sophisticated results and interfaces while companies have to place advertisements and make revenue to be able to offer their services for free. To address the above needs, it is more and more important to provide highly usable and optimized *search engine results pages* (SERPs). Yet, existing approaches to usability evaluation are often costly or time-consuming and mostly rely on explicit feedback. They are either not efficient or not effective while SERP interfaces are commonly optimized primarily from a company's point of view. Moreover, existing approaches to predicting search result relevance, which are mostly based on clicks, are not tailored to the evolving kinds of SERPs. For instance, they fail if queries are answered directly on a SERP and no clicks need to happen.

Applying *Human-Centered Design* principles, we propose a solution to the above in terms of a holistic approach that intends to satisfy both, searchers and developers. It provides novel means to counteract exclusively company-centric design and to make use of implicit user feedback for efficient and effective evaluation and optimization of usability and, in particular, relevance. We define personas and scenarios from which we infer unsolved problems and a set of well-defined requirements. Based on these requirements, we design and develop the **Search Interaction Optimization** toolkit. Using a bottom-up approach, we moreover define an eponymous, higher-level methodology. The Search Interaction Optimization toolkit comprises a total of six components.

We start with Iɴᴜɪᴛ :one:, which is a novel minimal usability instrument specifically aiming at meaningful correlations with implicit user feedback in terms of client-side interactions. Hence, it serves as a basis for deriving usability scores directly from user behavior. INUIT has been designed based on reviews of established usability standards and guidelines as well as interviews with nine dedicated usability experts. Its feasibility and effectiveness have been investigated in a user study. Also, a confirmatory factor analysis shows that the instrument can reasonably well describe real-world perceptions of usability.

Subsequently, we introduce *WaPPU* :two:, which is a context-aware A/B testing tool based on Iɴᴜɪᴛ. WaPPU implements the novel concept of *Usability-based Split Testing* and enables automatic usability evaluation of arbitrary SERP interfaces based on a quantitative score that is derived directly from user interactions. For this, usability models are automatically trained and applied based on machine learning techniques. In particular, the tool is not restricted to evaluating SERPs, but can be used with any web interface. 

Building on the above, we introduce *S.O.S., the SERP Optimization Suite* :three:, which comprises WaPPU as well as a *catalog of best practices* :four:. Once it has been detected that an investigated SERP's usability is suboptimal based on scores delivered by WaPPU, corresponding optimizations are automatically proposed based on the catalog of best practices. This catalog has been compiled in a three-step process involving reviews of existing SERP interfaces and contributions by 20 dedicated usability experts.

While the above focus on the general usability of SERPs, presenting the most relevant results is specifically important for search engines. Hence, our toolkit contains *TellMyRelevance! (TMR)* :five: — the first end-to-end pipeline for predicting search result relevance based on users’ interactions beyond clicks. TMR is a fully automatic approach that collects necessary information on the client, processes it on the server side and trains corresponding relevance models based on machine learning techniques. Predictions made by these models can then be fed back into the ranking process of the search engine, which improves result quality and hence also usability. *StreamMyRelevance! (SMR)* :six: takes the concept of TMR one step further by providing a streaming-based version. That is, SMR collects and processes interaction data and trains relevance models in near real-time.

Based on a user study and large-scale log analysis involving real-world search engines, we have evaluated the components of the Search Interaction Optimization toolkit as a whole — also to demonstrate the interplay of the different components. S.O.S., WaPPU and Iɴᴜɪᴛ have been engaged in the evaluation and optimization of a real-world SERP interface. Results show that our tools are able to correctly identify even subtle differences in usability. Moreover, optimizations proposed by S.O.S. significantly improved the usability of the investigated and redesigned SERP. TMR and SMR have been evaluated in a GB-scale interaction log analysis as well using data from real-world search engines. Our findings indicate that they are able to yield predictions that are better than those of competing state-of-the-art systems considering clicks only. Also, a comparison of SMR to existing solutions shows its superiority in terms of efficiency, robustness and scalability.

The thesis concludes with a discussion of the potential and limitations of the above contributions and provides an overview of potential future work.

## The SIO Toolkit

The six tools of the Search Interaction Optimization toolkit are intended to support *evaluation*, *optimization*, and *design* of search engine results pages.

Tool                                            | Evaluate           | Optimize           | Design             | Details
----------------------------------------------- | ------------------ | ------------------ | ------------------ | -------
:one: Iɴᴜɪᴛ: The Interface Usability Instrument | :heavy_check_mark: |                    |                    | https://github.com/maxspeicher/inuit-resources
:two: WaPPU: Was That Page Pleasant to Use?     | :heavy_check_mark: |                    |                    | https://github.com/maxspeicher/wappu-service
:three: S.O.S.: The SERP Optimization Suite     | :heavy_check_mark: | :heavy_check_mark: |                    | https://github.com/maxspeicher/sos
:four: Best Practices for SERPs                 |                    | :heavy_check_mark: | :heavy_check_mark: | https://github.com/maxspeicher/sos
:five: TellMyRelevance!                         |                    | :heavy_check_mark: |                    | https://github.com/maxspeicher/tellmyrelevance-resources
:six: StreamMyRelevance!                        |                    | :heavy_check_mark: |                    | https://github.com/maxspeicher/streammyrelevance-resources

to be continued ...

## Welcome to GitHub Pages

You can use the [editor on GitHub](https://github.com/maxspeicher/phdthesis/edit/gh-pages/index.md) to maintain and preview the content for your website in Markdown files.

Whenever you commit to this repository, GitHub Pages will run [Jekyll](https://jekyllrb.com/) to rebuild the pages in your site, from the content in your Markdown files.

### Markdown

Markdown is a lightweight and easy-to-use syntax for styling your writing. It includes conventions for

```markdown
Syntax highlighted code block

# Header 1
## Header 2
### Header 3

- Bulleted
- List

1. Numbered
2. List

**Bold** and _Italic_ and `Code` text

[Link](url) and ![Image](src)
```

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).

### Jekyll Themes

Your Pages site will use the layout and styles from the Jekyll theme you have selected in your [repository settings](https://github.com/maxspeicher/phdthesis/settings). The name of this theme is saved in the Jekyll `_config.yml` configuration file.

### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://github.com/contact) and we’ll help you sort it out.
