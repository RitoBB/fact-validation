# fact-validation

自动事实验证系统。
预处理:独热编码
文件检索: tf-idf 为原理的 pylucene 进行初步筛选
粗粒度句子筛选:包含用 stanfordNLP 进行 NER 提炼名词短语，对于 a of b 等句型的进行筛选。 􏰃 细粒度句子筛选:Bert 模型(Google GPU)
分类模型:使用 Bert 判断 true, false, not engough info
