# 中文数据预处理材料
包含素材：
*
	* 分词词典: 综合了百度、搜狗等词库，以及手动整理的若干人名和新近出现的热词
	* 中文停用词: 综合了"百度停用词表"，"哈工大停用词表"，"四川大学机器学习实验室停用词表"等若干停用词表，取交集并去除了不需要的标点符号和英文单词
* Tips
	* Chinese extraction
		chinese_pattern = u"([\u4e00-\u9fa5]+)"
		re_data = chi_pattern.findall(content_raw)
		content_clean  = ' '.join(re_data)