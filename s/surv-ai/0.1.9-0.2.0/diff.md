# Comparing `tmp/surv_ai-0.1.9.tar.gz` & `tmp/surv_ai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surv_ai-0.1.9.tar", max compression
+gzip compressed data, was "surv_ai-0.2.0.tar", max compression
```

## Comparing `surv_ai-0.1.9.tar` & `surv_ai-0.2.0.tar`

### file list

```diff
@@ -1,32 +1,35 @@
--rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.1.9/LICENSE
--rw-r--r--   0        0        0    21457 2023-05-24 16:07:15.155665 surv_ai-0.1.9/README.md
--rw-r--r--   0        0        0     1449 2023-05-24 22:03:59.026252 surv_ai-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     1301 2023-05-22 19:00:12.464186 surv_ai-0.1.9/surv_ai/__init__.py
--rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.1.9/surv_ai/core/__init__.py
--rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.1.9/surv_ai/core/agent.py
--rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.1.9/surv_ai/core/agents/__init__.py
--rw-r--r--   0        0        0     1608 2023-05-22 15:04:42.549505 surv_ai-0.1.9/surv_ai/core/agents/binary.py
--rw-r--r--   0        0        0     6959 2023-05-24 22:03:59.026585 surv_ai-0.1.9/surv_ai/core/agents/reasoning.py
--rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.1.9/surv_ai/core/interfaces.py
--rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.1.9/surv_ai/core/model.py
--rw-r--r--   0        0        0     4800 2023-05-24 17:10:39.143388 surv_ai-0.1.9/surv_ai/core/survey.py
--rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.1.9/surv_ai/lib/__init__.py
--rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.1.9/surv_ai/lib/conversation/__init__.py
--rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.1.9/surv_ai/lib/conversation/conversation.py
--rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.1.9/surv_ai/lib/conversation/interfaces.py
--rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.1.9/surv_ai/lib/knowledge_store/__init__.py
--rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.1.9/surv_ai/lib/knowledge_store/interfaces.py
--rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.1.9/surv_ai/lib/knowledge_store/local.py
--rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.1.9/surv_ai/lib/llm/__init__.py
--rw-r--r--   0        0        0     3926 2023-05-24 19:57:13.306950 surv_ai-0.1.9/surv_ai/lib/llm/anthropic.py
--rw-r--r--   0        0        0     4427 2023-05-24 22:03:59.026889 surv_ai-0.1.9/surv_ai/lib/llm/gpt.py
--rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.1.9/surv_ai/lib/llm/interfaces.py
--rw-r--r--   0        0        0     2005 2023-05-24 03:24:35.670699 surv_ai-0.1.9/surv_ai/lib/log.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.1.9/surv_ai/lib/tools/__init__.py
--rw-r--r--   0        0        0      732 2023-05-24 15:30:01.272295 surv_ai-0.1.9/surv_ai/lib/tools/interfaces.py
--rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.1.9/surv_ai/lib/tools/query/__init__.py
--rw-r--r--   0        0        0     7697 2023-05-24 22:03:59.027208 surv_ai-0.1.9/surv_ai/lib/tools/query/google_custom_search.py
--rw-r--r--   0        0        0      219 2023-05-19 05:42:04.105413 surv_ai-0.1.9/surv_ai/lib/tools/query/interfaces.py
--rw-r--r--   0        0        0     6326 2023-05-24 16:07:49.258939 surv_ai-0.1.9/surv_ai/lib/tools/query/wikipedia.py
--rw-r--r--   0        0        0     3229 2023-05-24 16:07:49.215788 surv_ai-0.1.9/surv_ai/lib/tools/tool_belt.py
--rw-r--r--   0        0        0    22809 1970-01-01 00:00:00.000000 surv_ai-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     1056 2023-05-19 03:25:36.438871 surv_ai-0.2.0/LICENSE
+-rw-r--r--   0        0        0    23413 2023-06-13 03:18:53.919084 surv_ai-0.2.0/README.md
+-rw-r--r--   0        0        0     1541 2023-06-13 03:18:53.922934 surv_ai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1495 2023-06-13 03:18:53.923358 surv_ai-0.2.0/surv_ai/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 02:57:50.211881 surv_ai-0.2.0/surv_ai/core/__init__.py
+-rw-r--r--   0        0        0     1667 2023-05-22 16:09:44.534005 surv_ai-0.2.0/surv_ai/core/agent.py
+-rw-r--r--   0        0        0        0 2023-05-09 03:57:54.724106 surv_ai-0.2.0/surv_ai/core/agents/__init__.py
+-rw-r--r--   0        0        0     1596 2023-06-02 12:27:31.332246 surv_ai-0.2.0/surv_ai/core/agents/binary.py
+-rw-r--r--   0        0        0     6840 2023-06-02 12:27:31.332538 surv_ai-0.2.0/surv_ai/core/agents/reasoning.py
+-rw-r--r--   0        0        0     1762 2023-06-13 03:18:53.924240 surv_ai-0.2.0/surv_ai/core/agents/web_page_summary.py
+-rw-r--r--   0        0        0     1857 2023-05-22 19:00:12.464474 surv_ai-0.2.0/surv_ai/core/interfaces.py
+-rw-r--r--   0        0        0     1279 2023-05-22 16:09:44.531688 surv_ai-0.2.0/surv_ai/core/model.py
+-rw-r--r--   0        0        0     6363 2023-06-13 03:18:53.924732 surv_ai-0.2.0/surv_ai/core/survey.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:43:12.303158 surv_ai-0.2.0/surv_ai/lib/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-22 03:24:33.757534 surv_ai-0.2.0/surv_ai/lib/conversation/__init__.py
+-rw-r--r--   0        0        0     1065 2023-05-22 15:04:42.565319 surv_ai-0.2.0/surv_ai/lib/conversation/conversation.py
+-rw-r--r--   0        0        0      409 2023-05-21 02:50:40.891526 surv_ai-0.2.0/surv_ai/lib/conversation/interfaces.py
+-rw-r--r--   0        0        0       53 2023-05-08 03:25:52.022148 surv_ai-0.2.0/surv_ai/lib/knowledge_store/__init__.py
+-rw-r--r--   0        0        0      693 2023-05-22 15:04:42.556450 surv_ai-0.2.0/surv_ai/lib/knowledge_store/interfaces.py
+-rw-r--r--   0        0        0     1486 2023-05-22 15:04:42.581390 surv_ai-0.2.0/surv_ai/lib/knowledge_store/local.py
+-rw-r--r--   0        0        0        0 2023-04-16 19:53:58.086455 surv_ai-0.2.0/surv_ai/lib/llm/__init__.py
+-rw-r--r--   0        0        0     3926 2023-05-24 19:57:13.306950 surv_ai-0.2.0/surv_ai/lib/llm/anthropic.py
+-rw-r--r--   0        0        0     4427 2023-05-24 22:03:59.026889 surv_ai-0.2.0/surv_ai/lib/llm/gpt.py
+-rw-r--r--   0        0        0      432 2023-05-22 15:04:42.564655 surv_ai-0.2.0/surv_ai/lib/llm/interfaces.py
+-rw-r--r--   0        0        0     2005 2023-05-24 03:24:35.670699 surv_ai-0.2.0/surv_ai/lib/log.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:14.406022 surv_ai-0.2.0/surv_ai/lib/tools/__init__.py
+-rw-r--r--   0        0        0      853 2023-06-13 03:18:53.925346 surv_ai-0.2.0/surv_ai/lib/tools/interfaces.py
+-rw-r--r--   0        0        0        0 2023-04-16 23:16:30.843990 surv_ai-0.2.0/surv_ai/lib/tools/query/__init__.py
+-rw-r--r--   0        0        0     1077 2023-06-13 03:18:53.925731 surv_ai-0.2.0/surv_ai/lib/tools/query/dataframe.py
+-rw-r--r--   0        0        0     3743 2023-06-13 03:18:53.926108 surv_ai-0.2.0/surv_ai/lib/tools/query/google_custom_search.py
+-rw-r--r--   0        0        0     1484 2023-06-13 03:18:53.926406 surv_ai-0.2.0/surv_ai/lib/tools/query/twitter.py
+-rw-r--r--   0        0        0     3274 2023-06-13 03:18:53.926781 surv_ai-0.2.0/surv_ai/lib/tools/query/wikipedia.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:18:53.926860 surv_ai-0.2.0/surv_ai/lib/tools/tool.py
+-rw-r--r--   0        0        0     2972 2023-06-13 03:18:53.928012 surv_ai-0.2.0/surv_ai/lib/tools/tool_belt.py
+-rw-r--r--   0        0        0    24800 1970-01-01 00:00:00.000000 surv_ai-0.2.0/PKG-INFO
```

### Comparing `surv_ai-0.1.9/LICENSE` & `surv_ai-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/README.md` & `surv_ai-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -214,33 +214,34 @@
 
 def build_parameter(date_range: tuple[str, str]):
     tool_belt = ToolBelt(
         tools=[
             GoogleCustomSearchTool(
                 google_api_key=os.environ["GOOGLE_API_KEY"],
                 google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                n_pages=20,
+                n_pages=30,
                 start_date=date_range[0],
-                end_date=date_range[1]
+                end_date=date_range[1],
+                max_concurrency=20,
             ),
         ],
     )
     base_knowledge = [
         Knowledge(
             text=f"It is currently {date_range[0]}. The included articles were published between {date_range[0]} and {date_range[1]}",
             source="Additional context",
         ),
     ]
     return SurveyParameter(
         independent_variable=date_range[1],
         kwargs={
             "client": client,
             "n_agents": 100,
-            "max_knowledge_per_agent":20,
-            "max_concurrency": 10,
+            "max_knowledge_per_agent":5,
+            "max_concurrency": 20,
             "tool_belt": tool_belt,
             "base_knowledge": base_knowledge,
         },
     )
 
 date_ranges = [
     ('2022-05-01', '2022-06-01'),
@@ -252,26 +253,36 @@
 ]
 
 model = Model(
     Survey,
     parameters=[build_parameter(date_range) for date_range in date_ranges],
 )
 
-results = await model.build(
+democrat_results = await model.build(
     "Democrats are favored to maintain control of the Senate in the 2022 November Midterm elections.",
 )
 ```
 
+We can also plot the inverted statement and observe opposite trend lines:
+
+```
+republican_results = await model.build(
+    "Republicans are favored to maintain control of the Senate in the 2022 November Midterm elections.",
+)
+```
+
 When compared with a leading model in political opinion polling, our model is presented as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
 
 *In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. [FiveThirtyEight data can be found here.](https://projects.fivethirtyeight.com/2022-election-forecast/senate/)*
 
-Pretty cool! Another example could involve plotting sentiments about the economy and using fluctuations in the yield curve as a benchmark for accuracy.
+Pretty cool! Note that the outputs don't represent complementary probabilities due to nuances in how the models reason, and biases of the models and data sources, but we can observe trend lines that do mirror each other quite well.
+
+Another example could involve plotting sentiments about the economy and using fluctuations in the S&P 500 as a benchmark for accuracy.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -300,15 +311,15 @@
         ),
     ]
     return SurveyParameter(
         independent_variable=date_range[1],
         kwargs={
             "client": client,
             "n_agents": 100,
-            "max_knowledge_per_agent":20,
+            "max_knowledge_per_agent":5,
             "max_concurrency": 10,
             "tool_belt": tool_belt,
             "base_knowledge": base_knowledge,
         },
     )
 
 date_ranges = [
@@ -329,17 +340,17 @@
 results = await model.build(
     "The United States economy looks like it is heading for a recession.",
 )
 ```
 
 This gives us the following graph:
 
-![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/yield_spread.png)
+![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/S&P.png)
 
-*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. Please note that it is the complement of multi-agent model that is plotted. [Yield spread data can be found here.](https://www.longtermtrends.net/us-treasury-yield-curve/)*
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. Please note that it is the complement of multi-agent model that is plotted. [S&P data can be found here.](https://www.google.com/finance/quote/.INX:INDEXSP?sa=X&ved=2ahUKEwi2hJWyg6D_AhXiGFkFHdqHCIYQ3ecFegQIIRAf)*
 
 ### Measuring bias in a data corpus
 
 A promising application of this technique is observing bias within a text corpus. For instance, we could create a model that uses different news sites as its independent variable to explore how the agents' conclusions might vary based on the data source utilized.
 
 ```
 from surv_ai import (
@@ -446,15 +457,15 @@
         ),
     ]
     return SurveyParameter(
         independent_variable=client.__class__.__name__,
         kwargs={
             "client": client,
             "n_agents": 100,
-            "max_knowledge_per_agent":20,
+            "max_knowledge_per_agent":3,
             "max_concurrency": 3,
             "tool_belt": tool_belt,
             "base_knowledge": base_knowledge,
         },
     )
 
 model = Model(
@@ -462,21 +473,76 @@
     parameters=[build_parameter(client) for client in clients],
 )
 results = await model.build(
     "OpenAI has been irresponsible in their handling of AI technology."
 )
 ```
 
-When we compare this statement between Anthropic and OpenAI's models, the resulting scatter plot appears as follows:
+When we compare the results between Anthropic and OpenAI's models, the scatter plot appears as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/openai.png)
 
 *In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com for articles published in the first half of 2023.*
 
 
+### Measuring sentiment on Twitter
+
+In addition to querying news sources we can also query social media websites for sentiment. There are many uses for this, but one simple and fun one would be to try and see if we can predict who will win the Academy Award for best picture.
+
+```
+from surv_ai import (
+    GPTClient,
+    ToolBelt,
+    TwitterTool,
+    Knowledge,
+    Survey,
+)
+client = GPTClient(os.environ["OPEN_AI_API_KEY"])
+
+films = [
+    "Everything Everywhere All At Once",
+    "All Quiet On the Western Front",
+    "The Banshees of Inisherin",
+    "The Fablemans",
+    "Tár",
+    "Top Gun: Maverick",
+    "Triangle of Sadness",
+    "Women Talking",
+]
+
+survey = Survey(
+    client,
+    n_agents=200,
+    tool_belt=ToolBelt(
+        tools=[
+            TwitterTool(
+                start_date="2023-01-01",
+                end_date="2023-03-11",
+                n_tweets=1000,
+            )
+        ]
+    ),
+    max_knowledge_per_agent=10,
+    base_knowledge=[
+        Knowledge(text="It is currently March 11th, 2023 and the Oscar's are tomorrow.", source="Additional context")
+    ]
+)
+
+results = {}
+for film in films:
+    results[film] = await survey.conduct(f"{film} is likely to win the Academy Award for Best Picture.")
+```
+
+Placing our results on a scatter plot, we get the correct result!
+
+![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/best_picture.png)
+*In this example, the agents were allowed to read Tweets up between January 1st 2023, and March 11th 2023 (the day before the Oscar's).*
+
+Sentiment on Twitter will not always be perfectly predictive of who will win an Academy Award, but it is an interesting way to try and predict outcomes.
+
 ## 🧠 Tips 
 
 Ultimately, a `Survey` is powered by a Large Language Model (LLM), which means that the survey hypothesis might require tuning, much like the general need to tune prompts. Here are some insights on crafting hypotheses.
 
 In these systems, any ambiguity in the original hypothesis can lead to unexpected results. This often happens because the agents interpret the statement too literally, thus rejecting the precise phrasing of the statement.
 
 Another useful tactic involves seeding base knowledge to the agents, which provides extra context to the problem. To revisit a previous example:
@@ -569,17 +635,17 @@
 
 Additionally, thanks go to the multitude of researchers and engineers out there who are contributing to unlocking the power of these models!
 
 ## 📈 Next steps 
 
 A few directions I plan to explore with this project include:
 
-1. I'm considering transitioning the core Large Language Model (LLM) interaction code to take advantage of Microsoft's Guidance framework.
-2. I aim to further refine the agent code to improve decision-making across a wide variety of problems. I'm particularly interested in exploring Tree of Thought Prompting to see the outcomes it generates.
-3. I plan to incorporate clients with more instruction-tuned and reinforcement-learned LLMs.
-4. One feature that would be exciting would be the ability to easily fit a machine learning model against a multi-agent model. This could allow projection with the multi-agent models.
-5. More documentation and use guides!
-
+1. Use the AmbiFC fact-checking data set to benchmark the approach of this framework and compare all future changes against this benchmark: https://paperswithcode.com/paper/evidence-based-verification-for-real-world
+2. More documentation and use guides!
+3. Kicking off a development blog.
+4. More integrations with various helpful tools.
+5. More examples and use cases.
+6. Experimentation to further optimize performance.
 
 ## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
```

### Comparing `surv_ai-0.1.9/pyproject.toml` & `surv_ai-0.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "surv_ai"
-version = "0.1.9"
+version = "0.2.0"
 description = "A framework for multi-agent modeling using large language models"
 authors = ["Daniel Balsam <daniel.balsam@survai.org>"]
 license = "MIT"
 readme = "README.md"
 keywords=[
     "ai",
     "artificial intelligence",
@@ -46,21 +46,23 @@
 python = "^3.9"
 pydantic = "^1.10.7"
 python-dotenv = "^1.0.0"
 beautifulsoup4 = "^4.12.2"
 colorama = "^0.4.6"
 exceptiongroup = "^1.1.1"
 requests = "^2.31.0"
+snscrape = {git = "https://github.com/JustAnotherArchivist/snscrape.git"}
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.22.0"
 isort = "^5.12.0"
 flake8 = "^6.0.0"
 black = "^23.3.0"
 matplotlib = "^3.7.1"
 pytest = "^7.3.1"
 mock = "^5.0.2"
 pytest-asyncio = "^0.21.0"
+pandas = "^2.0.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `surv_ai-0.1.9/surv_ai/__init__.py` & `surv_ai-0.2.0/surv_ai/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from .core.agent import BaseAgent  # noqa
 from .core.agents.binary import BinaryAgent  # noqa
 from .core.agents.reasoning import ReasoningAgent  # noqa
+from .core.agents.web_page_summary import WebPageSummaryAgent  # noqa
 from .core.interfaces import DataPoint  # noqa
 from .core.interfaces import (  # noqa
     AgentInterface,
     ModelInterface,
     SurveyInterface,
     SurveyParameter,
     SurveyResponse,
@@ -17,11 +18,13 @@
 from .lib.knowledge_store.interfaces import KnowledgeStoreInterface  # noqa
 from .lib.knowledge_store.local import LocalKnowledgeStore  # noqa
 from .lib.llm.anthropic import AnthropicClient  # noqa
 from .lib.llm.gpt import GPTClient  # noqa
 from .lib.llm.interfaces import LargeLanguageModelClientInterface  # noqa
 from .lib.llm.interfaces import Prompt, PromptMessage  # noqa
 from .lib.log import AgentLogLevel, logger  # noqa
+from .lib.tools.interfaces import ToolInterface, ToolResult  # noqa
+from .lib.tools.query.dataframe import DataframeTool  # noqa
 from .lib.tools.query.google_custom_search import GoogleCustomSearchTool  # noqa
-from .lib.tools.query.interfaces import ToolInterface  # noqa
+from .lib.tools.query.twitter import TwitterTool  # noqa
 from .lib.tools.query.wikipedia import WikipediaTool  # noqa
 from .lib.tools.tool_belt import ToolBelt  # noqa
```

### Comparing `surv_ai-0.1.9/surv_ai/core/agent.py` & `surv_ai-0.2.0/surv_ai/core/agent.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/core/agents/binary.py` & `surv_ai-0.2.0/surv_ai/core/agents/binary.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 
 from ..agent import BaseAgent
 
 
 class BinaryAgent(BaseAgent):
     def _get_initial_prompt_text(self, assertion: str):
         return f"""        
-        Your job is to determine if the user believes a statement is true or false.
+        Your job is to determine if the user believes a hypothesis is more likely to be true or false.
 
-        Here is the original assertion:
+        Here is the original hypothesis:
         
         "{assertion}"
 
-        The next message will be the statement for the user.
+        The next message will be what the user thinks.
 
         Your only options are "True," or "False".
 
         Please always respond with a single word.
         """
 
     async def _build_completion_prompt(self, conversation: ConversationInterface) -> str:
@@ -27,21 +27,18 @@
         )[0]
 
         self.messages = [
             PromptMessage(
                 role="system",
                 content=self._get_initial_prompt_text(assertion),
             ),
-            PromptMessage(
-                role="user",
-                content=conversation.as_string(),
-            ),
+            PromptMessage(role="user", content=conversation.as_string(), name="User thinks"),
             PromptMessage(
                 role="assistant",
-                content="I believe the user thinks this statement is: ",
+                content="I believe the user thinks this hypothesis is: ",
             ),
         ]
 
         return Prompt(messages=self.messages)
 
     async def prompt(self, statement: str, *args, **kwargs) -> str:
         prompt = await self._build_completion_prompt(statement, *args, **kwargs)
```

### Comparing `surv_ai-0.1.9/surv_ai/core/agents/reasoning.py` & `surv_ai-0.2.0/surv_ai/core/agents/reasoning.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,44 +5,40 @@
 from ..agent import BaseAgent
 from ..interfaces import AgentInterface
 
 
 class ReasoningAgent(BaseAgent, AgentInterface):
     def _get_completion_prompt_text(self, prompt: str):
         return f"""     
-        You are a citizen who must vote on whether this statement is more likely to be true or false:
+        You are a decisive agent who is concerned with whether this statement is more likely to be true or false:
 
         {prompt}
            
         You must decide whether you think the statement is more likely to be true or false.
 
-        You must cast your vote and participate in the civic process.
-
         The next two messages will be arguments in favor and against the above statement.
 
         You must decide which argument you are more persuaded by. You may not be undecided.
         """
 
     def _get_argument_prompt_text(self, prompt: str):
         return f"""     
-        You are a citizen who must vote on whether this statement is more likely to be true or false:
+        You are a decisive agent who is concerned with whether this statement is more likely to be true or false:
 
         {prompt}
            
         You must decide whether you think the statement is more likely to be true or false.
 
-        You must cast your vote and participate in the civic process.
-
         The next set of messages will be a series of articles that you can use to help you make your decision.
 
         In your response please include as many citations from your research as possible.
 
         Include both the publication title and the article title in your citations.
 
-        You must make the best decision possible with the information you have. 
+        You must make the best decision possible with the information you have.
         """
 
     def _get_plan_prompt_text(self, prompt: str):
         return f"""     
         You are a decisive agent who is concerned with whether this statement is more likely to be true or false:
 
         {prompt}
```

### Comparing `surv_ai-0.1.9/surv_ai/core/interfaces.py` & `surv_ai-0.2.0/surv_ai/core/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/core/model.py` & `surv_ai-0.2.0/surv_ai/core/model.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/lib/conversation/conversation.py` & `surv_ai-0.2.0/surv_ai/lib/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/lib/knowledge_store/interfaces.py` & `surv_ai-0.2.0/surv_ai/lib/knowledge_store/interfaces.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/lib/knowledge_store/local.py` & `surv_ai-0.2.0/surv_ai/lib/knowledge_store/local.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/lib/llm/anthropic.py` & `surv_ai-0.2.0/surv_ai/lib/llm/anthropic.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/lib/llm/gpt.py` & `surv_ai-0.2.0/surv_ai/lib/llm/gpt.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/lib/log.py` & `surv_ai-0.2.0/surv_ai/lib/log.py`

 * *Files identical despite different names*

### Comparing `surv_ai-0.1.9/surv_ai/lib/tools/tool_belt.py` & `surv_ai-0.2.0/surv_ai/lib/tools/tool_belt.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,28 +5,27 @@
 from surv_ai.lib.llm.interfaces import (
     LargeLanguageModelClientInterface,
     Prompt,
     PromptMessage,
 )
 from surv_ai.lib.log import logger
 
-from .interfaces import NoMemoriesFoundException, ToolBeltInterface, ToolInterface
+from .interfaces import (
+    NoMemoriesFoundException,
+    ToolBeltInterface,
+    ToolInterface,
+    ToolResult,
+)
 
 
 class ToolBelt(ToolBeltInterface):
     def __init__(
         self,
-        llm_client: Optional[LargeLanguageModelClientInterface] = None,
         tools: Optional[list[ToolInterface]] = None,
     ):
-        if llm_client:
-            logger.log_warning(
-                "Deprecation warning: LargeLanguageModelClient no longer should be passed into ToolBelt on init."
-            )
-
         self.tools = tools or []
 
     @staticmethod
     def tools_as_list(tools: list[ToolInterface]) -> str:
         return "\n".join(f"{i + 1}. {t.instruction}" for i, t in enumerate(tools)) if tools else ""
 
     def _get_tool_belt_prompt(self, original_prompt: str, base_knowledge: list[Knowledge]) -> str:
@@ -67,30 +66,28 @@
 
     async def inspect(
         self,
         client: LargeLanguageModelClientInterface,
         original_prompt: str,
         base_knowledge: list[Knowledge],
         attempt=1,
-    ):
+    ) -> list[ToolResult]:
         prompt = self._get_tool_belt_prompt(original_prompt, base_knowledge)
 
         response = (await client.get_completions([prompt], **{"temperature": 0.7}))[0].strip()
 
+        results: list[ToolResult] = []
         for tool in self.tools:
             match = re.match(tool.command, response)
 
             if match:
-                knowledge = []
                 for args in match.groups():
                     logger.log_context(f"...Using tool: {response}...")
 
-                    knowledge += await tool.use(client, original_prompt, args)
+                    results += await tool.use(args)
 
-                    if not knowledge and attempt < 3:
-                        knowledge = await self.inspect(client, original_prompt, base_knowledge, attempt=attempt + 1)
-                    elif not knowledge:
+                    if not results and attempt < 3:
+                        results = await self.inspect(client, original_prompt, base_knowledge, attempt=attempt + 1)
+                    elif not results:
                         raise NoMemoriesFoundException()
 
-                return knowledge
-
-        return []
+        return results
```

### Comparing `surv_ai-0.1.9/PKG-INFO` & `surv_ai-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 Metadata-Version: 2.1
 Name: surv-ai
-Version: 0.1.9
+Version: 0.2.0
 Summary: A framework for multi-agent modeling using large language models
 Home-page: https://github.com/DanielBalsam/surv_ai
 License: MIT
 Keywords: ai,artificial intelligence,data science,statistics,models,llm,agents,survai,surv_ai,survey,multi-agent,large language model,artificial intelligence,machine learning,natural language processing,nlp,sentiment analysis
 Author: Daniel Balsam
 Author-email: daniel.balsam@survai.org
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
 Requires-Dist: colorama (>=0.4.6,<0.5.0)
 Requires-Dist: exceptiongroup (>=1.1.1,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
+Requires-Dist: snscrape @ git+https://github.com/JustAnotherArchivist/snscrape.git
 Project-URL: Documentation, https://github.com/DanielBalsam/surv_ai/blob/main/README.md
 Project-URL: Repository, https://github.com/DanielBalsam/surv_ai
 Description-Content-Type: text/markdown
 
 # 🕵 Multi-agent modeling with large language models 
 <!-- [![PyPi](https://img.shields.io/badge/Official%20Website-agpt.co-blue?style=flat&logo=world&logoColor=white)](https://agpt.co) -->
 [![PyPi](https://shields.io/pypi/v/surv-ai)](https://pypi.org/project/surv-ai/)
@@ -242,33 +242,34 @@
 
 def build_parameter(date_range: tuple[str, str]):
     tool_belt = ToolBelt(
         tools=[
             GoogleCustomSearchTool(
                 google_api_key=os.environ["GOOGLE_API_KEY"],
                 google_search_engine_id=os.environ["GOOGLE_SEARCH_ENGINE_ID"],
-                n_pages=20,
+                n_pages=30,
                 start_date=date_range[0],
-                end_date=date_range[1]
+                end_date=date_range[1],
+                max_concurrency=20,
             ),
         ],
     )
     base_knowledge = [
         Knowledge(
             text=f"It is currently {date_range[0]}. The included articles were published between {date_range[0]} and {date_range[1]}",
             source="Additional context",
         ),
     ]
     return SurveyParameter(
         independent_variable=date_range[1],
         kwargs={
             "client": client,
             "n_agents": 100,
-            "max_knowledge_per_agent":20,
-            "max_concurrency": 10,
+            "max_knowledge_per_agent":5,
+            "max_concurrency": 20,
             "tool_belt": tool_belt,
             "base_knowledge": base_knowledge,
         },
     )
 
 date_ranges = [
     ('2022-05-01', '2022-06-01'),
@@ -280,26 +281,36 @@
 ]
 
 model = Model(
     Survey,
     parameters=[build_parameter(date_range) for date_range in date_ranges],
 )
 
-results = await model.build(
+democrat_results = await model.build(
     "Democrats are favored to maintain control of the Senate in the 2022 November Midterm elections.",
 )
 ```
 
+We can also plot the inverted statement and observe opposite trend lines:
+
+```
+republican_results = await model.build(
+    "Republicans are favored to maintain control of the Senate in the 2022 November Midterm elections.",
+)
+```
+
 When compared with a leading model in political opinion polling, our model is presented as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/midterms_2022.png)
 
 *In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. [FiveThirtyEight data can be found here.](https://projects.fivethirtyeight.com/2022-election-forecast/senate/)*
 
-Pretty cool! Another example could involve plotting sentiments about the economy and using fluctuations in the yield curve as a benchmark for accuracy.
+Pretty cool! Note that the outputs don't represent complementary probabilities due to nuances in how the models reason, and biases of the models and data sources, but we can observe trend lines that do mirror each other quite well.
+
+Another example could involve plotting sentiments about the economy and using fluctuations in the S&P 500 as a benchmark for accuracy.
 
 ```
 from surv_ai import (
     GPTClient,
     Model,
     ToolBelt,
     GoogleCustomSearchTool,
@@ -328,15 +339,15 @@
         ),
     ]
     return SurveyParameter(
         independent_variable=date_range[1],
         kwargs={
             "client": client,
             "n_agents": 100,
-            "max_knowledge_per_agent":20,
+            "max_knowledge_per_agent":5,
             "max_concurrency": 10,
             "tool_belt": tool_belt,
             "base_knowledge": base_knowledge,
         },
     )
 
 date_ranges = [
@@ -357,17 +368,17 @@
 results = await model.build(
     "The United States economy looks like it is heading for a recession.",
 )
 ```
 
 This gives us the following graph:
 
-![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/yield_spread.png)
+![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/S&P.png)
 
-*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. Please note that it is the complement of multi-agent model that is plotted. [Yield spread data can be found here.](https://www.longtermtrends.net/us-treasury-yield-curve/)*
+*In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com. Please note that it is the complement of multi-agent model that is plotted. [S&P data can be found here.](https://www.google.com/finance/quote/.INX:INDEXSP?sa=X&ved=2ahUKEwi2hJWyg6D_AhXiGFkFHdqHCIYQ3ecFegQIIRAf)*
 
 ### Measuring bias in a data corpus
 
 A promising application of this technique is observing bias within a text corpus. For instance, we could create a model that uses different news sites as its independent variable to explore how the agents' conclusions might vary based on the data source utilized.
 
 ```
 from surv_ai import (
@@ -474,15 +485,15 @@
         ),
     ]
     return SurveyParameter(
         independent_variable=client.__class__.__name__,
         kwargs={
             "client": client,
             "n_agents": 100,
-            "max_knowledge_per_agent":20,
+            "max_knowledge_per_agent":3,
             "max_concurrency": 3,
             "tool_belt": tool_belt,
             "base_knowledge": base_knowledge,
         },
     )
 
 model = Model(
@@ -490,21 +501,76 @@
     parameters=[build_parameter(client) for client in clients],
 )
 results = await model.build(
     "OpenAI has been irresponsible in their handling of AI technology."
 )
 ```
 
-When we compare this statement between Anthropic and OpenAI's models, the resulting scatter plot appears as follows:
+When we compare the results between Anthropic and OpenAI's models, the scatter plot appears as follows:
 
 ![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/openai.png)
 
 *In this example, the agents crawled websites such as nytimes.com, wsj.com, abcnews.com, cnn.com, bloomberg.com, foxnews.com, economist.com, washingtonpost.com, and nbcnews.com for articles published in the first half of 2023.*
 
 
+### Measuring sentiment on Twitter
+
+In addition to querying news sources we can also query social media websites for sentiment. There are many uses for this, but one simple and fun one would be to try and see if we can predict who will win the Academy Award for best picture.
+
+```
+from surv_ai import (
+    GPTClient,
+    ToolBelt,
+    TwitterTool,
+    Knowledge,
+    Survey,
+)
+client = GPTClient(os.environ["OPEN_AI_API_KEY"])
+
+films = [
+    "Everything Everywhere All At Once",
+    "All Quiet On the Western Front",
+    "The Banshees of Inisherin",
+    "The Fablemans",
+    "Tár",
+    "Top Gun: Maverick",
+    "Triangle of Sadness",
+    "Women Talking",
+]
+
+survey = Survey(
+    client,
+    n_agents=200,
+    tool_belt=ToolBelt(
+        tools=[
+            TwitterTool(
+                start_date="2023-01-01",
+                end_date="2023-03-11",
+                n_tweets=1000,
+            )
+        ]
+    ),
+    max_knowledge_per_agent=10,
+    base_knowledge=[
+        Knowledge(text="It is currently March 11th, 2023 and the Oscar's are tomorrow.", source="Additional context")
+    ]
+)
+
+results = {}
+for film in films:
+    results[film] = await survey.conduct(f"{film} is likely to win the Academy Award for Best Picture.")
+```
+
+Placing our results on a scatter plot, we get the correct result!
+
+![](https://raw.githubusercontent.com/DanielBalsam/surv_ai/main/examples/best_picture.png)
+*In this example, the agents were allowed to read Tweets up between January 1st 2023, and March 11th 2023 (the day before the Oscar's).*
+
+Sentiment on Twitter will not always be perfectly predictive of who will win an Academy Award, but it is an interesting way to try and predict outcomes.
+
 ## 🧠 Tips 
 
 Ultimately, a `Survey` is powered by a Large Language Model (LLM), which means that the survey hypothesis might require tuning, much like the general need to tune prompts. Here are some insights on crafting hypotheses.
 
 In these systems, any ambiguity in the original hypothesis can lead to unexpected results. This often happens because the agents interpret the statement too literally, thus rejecting the precise phrasing of the statement.
 
 Another useful tactic involves seeding base knowledge to the agents, which provides extra context to the problem. To revisit a previous example:
@@ -597,18 +663,18 @@
 
 Additionally, thanks go to the multitude of researchers and engineers out there who are contributing to unlocking the power of these models!
 
 ## 📈 Next steps 
 
 A few directions I plan to explore with this project include:
 
-1. I'm considering transitioning the core Large Language Model (LLM) interaction code to take advantage of Microsoft's Guidance framework.
-2. I aim to further refine the agent code to improve decision-making across a wide variety of problems. I'm particularly interested in exploring Tree of Thought Prompting to see the outcomes it generates.
-3. I plan to incorporate clients with more instruction-tuned and reinforcement-learned LLMs.
-4. One feature that would be exciting would be the ability to easily fit a machine learning model against a multi-agent model. This could allow projection with the multi-agent models.
-5. More documentation and use guides!
-
+1. Use the AmbiFC fact-checking data set to benchmark the approach of this framework and compare all future changes against this benchmark: https://paperswithcode.com/paper/evidence-based-verification-for-real-world
+2. More documentation and use guides!
+3. Kicking off a development blog.
+4. More integrations with various helpful tools.
+5. More examples and use cases.
+6. Experimentation to further optimize performance.
 
 ## 🤝 Contribute 
 
 If you'd like to contribute then please reach out!
```

