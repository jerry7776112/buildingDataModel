# buildingDataModel
## 專案說明
## 專案名稱: 建立資料模型

## Basics of Data Models
### What is Data Model
**資料模型**是一種抽像模型，它組織資料元素並標準化它們之間的關係以及與現實世界實體的屬性的關係。
**資料模型**是定義資料如何輸入和與輸出的一種模型。其主要作用是為資訊系統提供資料的定義和格式。資料模型是資料庫系統的核心和基礎，現有的資料庫系統都是基於某種資料模型而建立起來的。

* **概念資料模型**：描述域的語義，即模型的範圍。 例如，它可能是組織或行業的興趣領域的模型。 它由表示領域中重要事物的實體類別以及有關實體類別對之間關聯的關係斷言組成。 概念模式指定可以使用模型表達的事實或命題的類型。 從這個意義上說，它定義了人工「語言」中允許的表達式，其範圍受模型範圍的限制。

* **邏輯資料模型**：描述由特定資料操作技術表示的語意。 其中包括表格和欄位、物件導向的類別和 XML 標記等的描述。

* **實體資料模型**：描述資料儲存的物理方式。 這與分區、CPU、表空間等有關。
### Why is Data Modeling Important
* 數據的組織
* 有了數據的組織才能確保之後數據的使用
* 會在應用程式建立、業務邏輯、分析模型之前建立

### Who Does This Type of Work
* Data Scientist(資料科學家)
* Data Engineer(資料工程師)
* Software Engineer(軟體工程師)

### Relational Model and Database
* 它是一個基於資料關係模型的數位資料庫
* 用於維護關係資料庫(Relational Databases)的軟體系統是關聯式資料庫管理系統(Relational DataBase Management System)（RDBMS）
* 將資料組織到一個或多個由列(column)和行(row)組成的表(table)中，並使用唯一的鍵((unique key)辨認。
* Databse/Schema
    * Collection of Tables
* Tables/Relations
    * A group of rows sharing the same labeled elements  
### ACID Properties
* **A**tomicity
    * EX: The entire transaction takes place at once or doesn't happen at all.(整個交易立即發生或根本不發生)
* **C**onsistency
    * EX: The database must be consistent before and after the tranction.(事件發生前後資料庫必須一致) 
* **I**solation
    * EX: Mutiple Transactions occur independently without interference.(多筆交易獨立發生，互不干擾)
* **D**urability
    * EX: The changes of a successful transaction occurs even if the system failure occurs.(即使系統發生故障，成功交易的變化也會發生)
### When not to use RDBMS(不適合使用 RDBMS 的情況)
* Large amounts of Data(大量數據)
* Need to be able to store different data types formats(需要能夠儲存不同的資料類型格式)
* Need a flexible schema(需要彈性的架構)
* Need high availability(需要高可用性)
* Need horizontal scalability(需要水平可擴展性)

## Exercise 1 - Creating Tables in PostgreSQL using Python
* 使用python連線至postgreSQL並建立資料表
* **詳情請參閱[Exercise 1 : Creating a Table with PostgreSQL](https://github.com/jerry7776112/buildingDataModel/blob/main/Exercise%201%20-%20Creating%20a%20Table%20with%20PostgreSQL.ipynb)**
![architecture](https://github.com/jerry7776112/buildingDataModel/blob/main/architecture/exercise.png "architecture")

## Project - Building Data Model and Creating Database
* 根據**[dataset](https://github.com/jerry7776112/buildingDataModel/tree/main/dataset)**設計資料模型建立三個資料表
* **詳情請參閱[Data Engineer Project1.ipynb](https://github.com/jerry7776112/buildingDataModel/blob/main/Data%20Engineer%20Project1.ipynb)**
![architecture](https://github.com/jerry7776112/buildingDataModel/blob/main/architecture/project.png "architecture")
