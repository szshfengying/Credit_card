# Credit_card
信用评分卡模型
本文采用lending club官网公开数据中2017年Q2部分，数据内容为贷款申请人信息包括申请人的年龄、性别、婚姻状况、学历、贷款金额、申请人财产情况等（自变量）和贷款履行情况（因变量）。使用2017年数据是为了方便与其他人的结果对比。 
信用评分卡模型是基于客户过去行为和属性预测其未来是否逾期，流程主要包括处理缺失值、将原始变量进行WOE编码，通过IV值、相关系数、显著性依次筛选变量，使用SMOTE解决类别不平衡问题，通过逻辑回归算法解决二元分类问题（判定贷款申请人是否违约），再计算出每个样本的评分（为了方便业务使用，类似于芝麻信用分）。
最终结果，auc=0.953, ks=0.802, accuracy_score=0.938 。
