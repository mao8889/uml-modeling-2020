# 实验二：用例建模

## 一、实验目标

1.选题用例建模

2.撰写用例规约

3.编写实验报告

## 二、实验内容

1.根据选题创建用例图

2.根据用例攥写2-3个用例规约

3.完成实验报告

## 三、实验步骤

1.确认选题 - 护肤品推荐系统

2.根据选题创建用例图

  参与者 - 用户
  
  功能 -  
  
         a.录入皮肤状态 —— 用户登陆成功后在首页选择个人皮肤状态（油性、干性、混合性、中性），可多选特殊皮肤状态（痘痘肌、敏感肌）
         
         b.查询护肤方案 —— 系统根据用户提供的皮肤状态显示可选择的护肤品，用户可点击“筛选”按钮进行护肤品类型选择（面膜、化妆师、精华液等）
         
         c.查询护肤品详情 —— 查询护肤品的具体情况（含量、功效等）
         
   建立用户和功能的关系

3.根据用例图中功能攥写3个用例规约

4.提交实验报告

## 四、实验结果

1.用例图

![图1：实验二用例图](./No2_UseCaseDiagram.jpg)

图1：实验二用例图

2.用例规约

 表1：录入皮肤状态用例规约  

用例编号  | UC01 | 备注  
-|:-|-  
用例名称  | 录入皮肤状态  |   
前置条件  | 用户登录护肤品推荐系统 |
后置条件  |      |  
基本流程  | 1.用户点击“皮肤状态”按钮|*用例执行成功的步骤*    
~| 2.系统显示选择页面 |
~| 3.用户点击勾选皮肤状态信息，点击“确认录入”按钮 |   
~| 4.系统添加一条皮肤状态信息，提示“录入成功”， |   
~| 5.用户点击“关闭”按钮 |
~| 6.系统返回首页，显示皮肤状态信息 |
扩展流程  | 3.1 系统检查用户选择操作为空，提示“录入信息不能为空”  |*用例执行失败*    


 表2：查询护肤方案用例规约  

用例编号  | UC02 | 备注  
-|:-|-  
用例名称  | 查询护肤方案  |   
前置条件  | 用户已成功录入皮肤状态 |
后置条件  |      |
基本流程  | 1.用户点击“搜索”按钮  |*用例执行成功的步骤*    
~| 2.系统查询护肤方案 |   
~| 3.系统显示护肤方案页面 |   
~| 4.用户点击“筛选”按钮 |   
~| 5.系统显示护肤品类型选择页面 | 
~| 6.用户选择护肤品类型 |
~| 7.系统检查用户选择操作不为空，查询护肤方案 |
~| 8.系统显示护肤方案 |
扩展流程  | 7.1 系统检查用户选择操作为空，提示“请选择护肤品类型”   |*用例执行失败*  
~| 8.1 系统检查无匹配护肤方案，提示“无匹配护肤方案，请选择其他护肤品类型再次进行搜索”   |


 表3：查询护肤品详情用例规约  

用例编号  | UC03 | 备注  
-|:-|-  
用例名称  | 查询护肤品详情 |   
前置条件  | 用户登录护肤品推荐系统 | 
后置条件  |      | 
基本流程  | 1.用户在输入框输入护肤品名称，点击“搜索”按钮 |*用例执行成功的步骤*    
~| 2.系统查询护肤品信息 |   
~| 3.系统显示护肤品详细信息 | 
扩展流程  | 2.1 系统检查输入信息为空，提示“请输入护肤品名称”  |*用例执行失败*
~| 2.2 系统检查输入信息不为空，查询不到护肤品信息，提示“无此护肤品，请检查输入名称是否错误”  |