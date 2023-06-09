# Comparing `tmp/spark-llm-0.1.1.tar.gz` & `tmp/spark_llm-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark-llm-0.1.1.tar", last modified: Thu Jun  8 18:09:10 2023, max compression
+gzip compressed data, was "spark_llm-0.1.2.tar", max compression
```

## Comparing `spark-llm-0.1.1.tar` & `spark_llm-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,7 @@
-drwxr-xr-x   0 gengliang.wang   (502) staff       (20)        0 2023-06-08 18:09:10.567642 spark-llm-0.1.1/
--rw-r--r--   0 gengliang.wang   (502) staff       (20)    11357 2023-06-07 23:43:47.000000 spark-llm-0.1.1/LICENSE
--rw-r--r--   0 gengliang.wang   (502) staff       (20)     2473 2023-06-08 18:09:10.567464 spark-llm-0.1.1/PKG-INFO
--rw-r--r--   0 gengliang.wang   (502) staff       (20)     1757 2023-06-08 17:50:13.000000 spark-llm-0.1.1/README.md
--rw-r--r--   0 gengliang.wang   (502) staff       (20)       38 2023-06-08 18:09:10.567705 spark-llm-0.1.1/setup.cfg
--rw-r--r--   0 gengliang.wang   (502) staff       (20)     1138 2023-06-08 17:50:13.000000 spark-llm-0.1.1/setup.py
-drwxr-xr-x   0 gengliang.wang   (502) staff       (20)        0 2023-06-08 18:09:10.565670 spark-llm-0.1.1/spark_llm/
--rw-r--r--   0 gengliang.wang   (502) staff       (20)      137 2023-06-08 04:15:29.000000 spark-llm-0.1.1/spark_llm/__init__.py
--rw-r--r--   0 gengliang.wang   (502) staff       (20)     4959 2023-06-08 03:00:00.000000 spark-llm-0.1.1/spark_llm/prompt.py
--rw-r--r--   0 gengliang.wang   (502) staff       (20)     7416 2023-06-08 05:29:48.000000 spark-llm-0.1.1/spark_llm/spark_llm_assistant.py
-drwxr-xr-x   0 gengliang.wang   (502) staff       (20)        0 2023-06-08 18:09:10.567139 spark-llm-0.1.1/spark_llm.egg-info/
--rw-r--r--   0 gengliang.wang   (502) staff       (20)     2473 2023-06-08 18:09:10.000000 spark-llm-0.1.1/spark_llm.egg-info/PKG-INFO
--rw-r--r--   0 gengliang.wang   (502) staff       (20)      265 2023-06-08 18:09:10.000000 spark-llm-0.1.1/spark_llm.egg-info/SOURCES.txt
--rw-r--r--   0 gengliang.wang   (502) staff       (20)        1 2023-06-08 18:09:10.000000 spark-llm-0.1.1/spark_llm.egg-info/dependency_links.txt
--rw-r--r--   0 gengliang.wang   (502) staff       (20)       51 2023-06-08 18:09:10.000000 spark-llm-0.1.1/spark_llm.egg-info/requires.txt
--rw-r--r--   0 gengliang.wang   (502) staff       (20)       10 2023-06-08 18:09:10.000000 spark-llm-0.1.1/spark_llm.egg-info/top_level.txt
+-rw-r--r--   0        0        0    11357 2023-06-07 23:43:47.653712 spark_llm-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1925 2023-06-08 22:10:10.249098 spark_llm-0.1.2/README.md
+-rw-r--r--   0        0        0      903 2023-06-09 04:34:28.145833 spark_llm-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      131 2023-06-08 22:37:32.156425 spark_llm-0.1.2/spark_llm/__init__.py
+-rw-r--r--   0        0        0     5272 2023-06-08 22:37:32.162648 spark_llm-0.1.2/spark_llm/prompt.py
+-rw-r--r--   0        0        0     8829 2023-06-08 22:37:32.194595 spark_llm-0.1.2/spark_llm/spark_llm_assistant.py
+-rw-r--r--   0        0        0     3071 1970-01-01 00:00:00.000000 spark_llm-0.1.2/PKG-INFO
```

### Comparing `spark-llm-0.1.1/LICENSE` & `spark_llm-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spark-llm-0.1.1/README.md` & `spark_llm-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -5,43 +5,51 @@
 ## Installation
 
 ```bash
 pip install spark-llm
 ```
 
 ## Usage
-To create an instance of SparkLLMAssistant:
+### Initialization
 ```python
 from langchain.chat_models import ChatOpenAI
 from spark_llm import SparkLLMAssistant
 
 llm = ChatOpenAI(model_name='gpt-4') # using gpt-4 can achieve better results
 assistant=SparkLLMAssistant(llm=llm)
 ```
 
-To create a Dataframe with web search and LLM:
+### Data Ingestion
 ```python
 auto_df=assistant.create_df("2022 USA national auto sales by brand")
 auto_df.show(n=5)
 ```
-| rank | brand     | sales   | Percentage_Change |
-|------|-----------|---------|-------------------|
-| 1    | Toyota    | 1849751 | -9                |
-| 2    | Ford      | 1767439 | -2                |
-| 3    | Chevrolet | 1502389 | 6                 |
-| 4    | Honda     | 881201  | -33               |
-| 5    | Hyundai   | 724265  | -2                |
+| rank | brand     | us_sales_2022 | sales_change_vs_2021 |
+|------|-----------|---------------|----------------------|
+| 1    | Toyota    | 1849751       | -9                   |
+| 2    | Ford      | 1767439       | -2                   |
+| 3    | Chevrolet | 1502389       | 6                    |
+| 4    | Honda     | 881201        | -33                  |
+| 5    | Hyundai   | 724265        | -2                   |
 
-To explain a Spark Dataframe in simple words
+### DataFrame Transformation
+```python
+auto_top_growth_df=assistant.transform_df(auto_df, "top brand with the highest growth")
+auto_top_growth_df.show()
+```
+| brand    | us_sales_2022 | sales_change_vs_2021 |
+|----------|---------------|----------------------|
+| Cadillac | 134726        | 14                   |
+
+### DataFrame Explaination
 ```python
-auto_top_growth_df = auto_df.orderBy(auto_df.percentage_change.desc()).limit(1)
 assistant.explain_df(auto_top_growth_df)
 ```
 
-> In summary, this dataframe is retrieving the single record with the highest percentage change in sales from the `auto_sales_2022` view, which contains information about the rank, brand, sales, and percentage change in sales for various car brands in the year 2022.
+> In summary, this dataframe is retrieving the brand with the highest sales change in 2022 compared to 2021. It presents the results sorted by sales change in descending order and only returns the top result.
 
 Refer to [example.ipynb](https://github.com/gengliangwang/spark-llm/blob/main/examples/example.ipynb) for more detailed usage examples.
 
 
 ## Contributing
 Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
```

### Comparing `spark-llm-0.1.1/spark_llm/prompt.py` & `spark_llm-0.1.2/spark_llm/prompt.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 The answer MUST contain the url link only
 """
 
 SEARCH_PROMPT = PromptTemplate(
     input_variables=["query", "search_results", "columns"], template=SEARCH_TEMPLATE
 )
 
-
 SQL_TEMPLATE = """Given the following question:
 ```
 {query}
 ```
 I got the following answer from a web page:
 ```
 {web_content}
@@ -33,14 +32,27 @@
 The answer MUST contain query only.
 """
 
 SQL_PROMPT = PromptTemplate(
     input_variables=["query", "web_content", "columns"], template=SQL_TEMPLATE
 )
 
+TRANSFORM_TEMPLATE = """
+Given a Spark temp view `{view_name}` with the following columns:
+```
+{columns}
+```
+Write a Spark SQL query to retrieve: {desc}
+The answer MUST contain query only.
+"""
+
+TRANSFORM_PROMPT = PromptTemplate(
+    input_variables=["view_name", "columns", "desc"], template=TRANSFORM_TEMPLATE
+)
+
 EXPLAIN_PREFIX = """You are an Apache Spark SQL expert, who can summary what a dataframe retrieves. Given an analyzed 
 query plan of a dataframe, you will 
 1. convert the dataframe to SQL query. Note that an explain output contains plan 
 nodes separated by "\n". Each plan node has its own expressions and expression ids. 
 2. summary what the sql query retrieves. 
 """
```

### Comparing `spark-llm-0.1.1/spark_llm/spark_llm_assistant.py` & `spark_llm-0.1.2/spark_llm/spark_llm_assistant.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,20 @@
 import tiktoken
 from bs4 import BeautifulSoup
 from langchain import LLMChain, GoogleSearchAPIWrapper
 from langchain.base_language import BaseLanguageModel
 from pyspark.sql import SparkSession, DataFrame
 from tiktoken import Encoding
 
-from spark_llm.prompt import SEARCH_PROMPT, SQL_PROMPT, EXPLAIN_DF_PROMPT
+from spark_llm.prompt import (
+    SEARCH_PROMPT,
+    SQL_PROMPT,
+    EXPLAIN_DF_PROMPT,
+    TRANSFORM_PROMPT,
+)
 
 
 class SparkLLMAssistant:
     _HTTP_HEADER = {
         "User-Agent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36"
         " (KHTML, like Gecko) Chrome/91.0.4472.124 Safari/537.36",
         "Accept": "text/html,application/xhtml+xml,application/xml;q=0.9,*/*;q=0.8",
@@ -45,14 +50,15 @@
         self._llm = llm
         self._web_search_tool = web_search_tool or self._default_web_search_tool
         self._encoding = encoding or tiktoken.get_encoding("cl100k_base")
         self._max_tokens_of_web_content = max_tokens_of_web_content
         self._search_llm_chain = LLMChain(llm=self._llm, prompt=SEARCH_PROMPT)
         self._sql_llm_chain = LLMChain(llm=self._llm, prompt=SQL_PROMPT)
         self._explain_chain = LLMChain(llm=llm, prompt=EXPLAIN_DF_PROMPT)
+        self._transform_chain = LLMChain(llm=llm, prompt=TRANSFORM_PROMPT)
         self._verbose = verbose
 
     @staticmethod
     def _extract_view_name(query: str) -> str:
         """
         Extract the view name from the provided SQL query.
 
@@ -169,15 +175,42 @@
 
         soup = BeautifulSoup(response.text, "html.parser")
         # If the input is a URL link, use the title of web page as the dataset's description.
         if is_url:
             desc = soup.title.string
         return self._create_dataframe_with_llm(soup.get_text(), desc, columns)
 
+    def transform_df(self, df: DataFrame, desc: str) -> DataFrame:
+        """
+        This method applies a transformation to a provided Spark DataFrame, the specifics of which are determined by the 'desc' parameter.
+
+        :param df: The Spark DataFrame that is to be transformed.
+        :param desc: A natural language string that outlines the specific transformation to be applied on the DataFrame.
+
+        :return: Returns a new Spark DataFrame that is the result of applying the specified transformation on the input DataFrame.
+        """
+        temp_view_name = "temp_view_for_transform"
+        df.createOrReplaceTempView(temp_view_name)
+        schema_str = "\n".join([f"{name}: {dtype}" for name, dtype in df.dtypes])
+        sql_query = self._transform_chain.run(
+            view_name=temp_view_name, columns=schema_str, desc=desc
+        )
+        self.log(f"SQL query for the transform:\n{sql_query}")
+        return self._spark.sql(sql_query)
+
     def explain_df(self, df: DataFrame) -> str:
-        explain_result=self._explain_chain.run(df._jdf.queryExecution().analyzed().toString())
+        """
+        This method generates a natural language explanation of the SQL plan of the input Spark DataFrame.
+
+        :param df: The Spark DataFrame to be explained.
+
+        :return: A string explanation of the DataFrame's SQL plan, detailing what the DataFrame is intended to retrieve.
+        """
+        explain_result = self._explain_chain.run(
+            df._jdf.queryExecution().analyzed().toString()
+        )
         # If there is code block in the explain result, ignore it.
-        if '```' in explain_result:
+        if "```" in explain_result:
             summary = explain_result.split("```")[-1]
             return summary.strip()
         else:
             return explain_result
```

