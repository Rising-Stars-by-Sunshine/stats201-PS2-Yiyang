# Machine Learning for China Life Expectancy
## Project information
- **Author**: Yiyang Zhang, Computation and Design with tracks in Digital Media, Class of 2025, Duke Kunshan University
- **Instructor**: Prof. Luyao Zhang, Duke Kunshan University
- **Disclaimer**: Submissions to the Problem Set 2 for STATS201 Introduction to Machine Learning for Social Science, 2023 Spring Term (Seven Week - First) instructed by Prof. Luyao Zhang at Duke Kunshan University.
- **Acknowledgments**: Thanks for Xintong Wu's encouragement and Shiran Yuan's suggestion on the selection of timeline.
- **Project Summary**: 
  - [Summarize the Background/Motivation]
  - [Research Questions]
  - [Application Scenario (Data Source)]
  - [Methodology]
  - [Results]
  - [Intellectual Merits and Practical impacts of your project.]

## Table of Contents
- data
- code
- spotlight



## Data
- Data Source:https://ourworldindata.org/life-expectancy
<table class="MsoNormalTable" border="0" cellspacing="0" style="border-collapse:collapse;margin-left:6.7500pt;margin-right:6.7500pt;
mso-table-layout-alt:fixed;border:none;mso-padding-alt:0.0000pt 5.4000pt 0.0000pt 5.4000pt ;"><tbody><tr style="height:31.1000pt;"><td width="104" valign="top" rowspan="3" style="width:104.0000pt;padding:0.0000pt 5.4000pt 0.0000pt 5.4000pt ;border-left:none;
mso-border-left-alt:none;border-right:none;mso-border-right-alt:none;
border-top:none;mso-border-top-alt:none;border-bottom:none;
mso-border-bottom-alt:none;"><p class="MsoNormal" style="mso-pagination:widow-orphan;"><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;">Explanation</span><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><o:p></o:p></span></p></td><td width="339" valign="top" style="width:339.7500pt;padding:0.0000pt 5.4000pt 0.0000pt 5.4000pt ;border-left:none;
mso-border-left-alt:none;border-right:none;mso-border-right-alt:none;
border-top:none;mso-border-top-alt:none;border-bottom:none;
mso-border-bottom-alt:none;"><p class="MsoNormal" style="mso-pagination:widow-orphan;"><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><a href="https://raw.githubusercontent.com/Rising-Stars-by-Sunshine/stats201-PS2-Yiyang/main/data/Queried_Data/life-expectancy.csv">life-expectancy</a></span><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><o:p></o:p></span></p></td></tr><tr style="height:31.1000pt;"><td width="339" valign="top" style="width:339.7500pt;padding:0.0000pt 5.4000pt 0.0000pt 5.4000pt ;border-left:none;
mso-border-left-alt:none;border-right:none;mso-border-right-alt:none;
border-top:none;mso-border-top-alt:none;border-bottom:none;
mso-border-bottom-alt:none;"><p class="MsoNormal" style="mso-pagination:widow-orphan;"><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><a href="https://raw.githubusercontent.com/Rising-Stars-by-Sunshine/stats201-PS2-Yiyang/main/data/Queried_Data/HL.csv">Queried Data</a></span><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><o:p></o:p></span></p></td></tr><tr style="height:31.1000pt;"><td width="339" valign="top" style="width:339.7500pt;padding:0.0000pt 5.4000pt 0.0000pt 5.4000pt ;border-left:none;
mso-border-left-alt:none;border-right:none;mso-border-right-alt:none;
border-top:none;mso-border-top-alt:none;border-bottom:none;
mso-border-bottom-alt:none;"><p class="MsoNormal" style="mso-pagination:widow-orphan;"><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><a href="https://raw.githubusercontent.com/Rising-Stars-by-Sunshine/stats201-PS2-Yiyang/main/data/Processed_Data/CHL.csv">Process<font face="Times New Roman Regular">ed</font>&nbsp;Data</a></span><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><o:p></o:p></span></p></td></tr><tr style="height:31.1000pt;"><td width="104" valign="top" rowspan="2" style="width:104.0000pt;padding:0.0000pt 5.4000pt 0.0000pt 5.4000pt ;border-left:none;
mso-border-left-alt:none;border-right:none;mso-border-right-alt:none;
border-top:none;mso-border-top-alt:none;border-bottom:none;
mso-border-bottom-alt:none;"><p class="MsoNormal" style="mso-pagination:widow-orphan;"><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;">Prediction</span><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><o:p></o:p></span></p></td><td width="339" valign="top" style="width:339.7500pt;padding:0.0000pt 5.4000pt 0.0000pt 5.4000pt ;border-left:none;
mso-border-left-alt:none;border-right:none;mso-border-right-alt:none;
border-top:none;mso-border-top-alt:none;border-bottom:none;
mso-border-bottom-alt:none;"><p class="MsoNormal" style="mso-pagination:widow-orphan;"><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><a href="https://raw.githubusercontent.com/Rising-Stars-by-Sunshine/stats201-PS2-Yiyang/main/data/Processed_Data/Regression_Train.csv">Regression&nbsp;Train</a></span><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><o:p></o:p></span></p></td></tr><tr style="height:16.7500pt;"><td width="339" valign="top" style="width:339.7500pt;padding:0.0000pt 5.4000pt 0.0000pt 5.4000pt ;border-left:none;
mso-border-left-alt:none;border-right:none;mso-border-right-alt:none;
border-top:none;mso-border-top-alt:none;border-bottom:none;
mso-border-bottom-alt:none;"><p class="MsoNormal" style="mso-pagination:widow-orphan;"><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><a href="https://raw.githubusercontent.com/Rising-Stars-by-Sunshine/stats201-PS2-Yiyang/main/data/Processed_Data/Regression_Test.csv">Regression&nbsp;Test</a></span><span style="font-family:'Times New Roman Regular';mso-fareast-font-family:宋体;font-size:10.5000pt;
mso-font-kerning:1.0000pt;"><o:p></o:p></span></p></td></tr></tbody></table>

## Code
- Query Data
- Process Data
- Analyze Data
- ...

## Spotlight
- Figures
- Posters
- Slides
- Presentations
- Review articles
- Media appearance

## References

### Data Source
- Data Source Title and URL
### Code Source
- Code Source Title and URL
### Articles
- Article Source Title and URL
### Literature
- Literature References in [Chicago Author-Date](https://www.chicagomanualofstyle.org/tools_citationguide/citation-guide-2.html) Style and [BibTex](https://scholar.google.com/) 

Levin, Dan, and Luyao Zhang. 2020. “Bridging Level-K to Nash Equilibrium.” *The Review of Economics and Statistics* 104 (6): 1329–40. https://doi.org/10.1162/rest_a_00990.

```
@article{levin2022bridging,
  title={Bridging level-k to nash equilibrium},
  author={Levin, Dan and Zhang, Luyao},
  journal={Review of Economics and Statistics},
  volume={104},
  number={6},
  pages={1329--1340},
  year={2022},
  publisher={MIT Press One Rogers Street, Cambridge, MA 02142-1209, USA journals-info~…}
}
```

