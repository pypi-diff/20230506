# Comparing `tmp/promptwatch-0.0.4.tar.gz` & `tmp/promptwatch-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.0.4.tar", last modified: Wed May  3 12:44:13 2023, max compression
+gzip compressed data, was "promptwatch-0.0.5.tar", last modified: Sat May  6 08:09:00 2023, max compression
```

## Comparing `promptwatch-0.0.4.tar` & `promptwatch-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.764048 promptwatch-0.0.4/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-03 12:44:13.763905 promptwatch-0.0.4/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.0.4/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.4/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-03 12:44:13.764086 promptwatch-0.0.4/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 21:26:09.000000 promptwatch-0.0.4/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.761187 promptwatch-0.0.4/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.762681 promptwatch-0.0.4/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-03 12:43:27.000000 promptwatch-0.0.4/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    11830 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.4/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1912 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.763678 promptwatch-0.0.4/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-03 12:40:47.000000 promptwatch-0.0.4/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    31533 2023-05-03 12:39:13.000000 promptwatch-0.0.4/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13397 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/promptwatch_context.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.0.4/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-03 12:44:13.763388 promptwatch-0.0.4/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.4/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-03 12:44:13.000000 promptwatch-0.0.4/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 08:09:00.961507 promptwatch-0.0.5/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-06 08:09:00.961351 promptwatch-0.0.5/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3750 2023-05-02 21:26:09.000000 promptwatch-0.0.5/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.0.5/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-05-06 08:09:00.961551 promptwatch-0.0.5/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1169 2023-05-02 21:26:09.000000 promptwatch-0.0.5/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 08:09:00.956297 promptwatch-0.0.5/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 08:09:00.958606 promptwatch-0.0.5/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      282 2023-05-06 08:08:32.000000 promptwatch-0.0.5/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    11830 2023-05-02 21:26:09.000000 promptwatch-0.0.5/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3706 2023-05-02 21:26:09.000000 promptwatch-0.0.5/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5469 2023-04-22 10:16:33.000000 promptwatch-0.0.5/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1912 2023-05-02 21:26:09.000000 promptwatch-0.0.5/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 08:09:00.960645 promptwatch-0.0.5/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      107 2023-05-03 12:40:47.000000 promptwatch-0.0.5/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    33555 2023-05-06 07:31:24.000000 promptwatch-0.0.5/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13419 2023-05-03 21:32:50.000000 promptwatch-0.0.5/src/promptwatch/promptwatch_context.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1081 2023-05-02 21:26:09.000000 promptwatch-0.0.5/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-05-06 08:09:00.960220 promptwatch-0.0.5/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4123 2023-05-06 08:09:00.000000 promptwatch-0.0.5/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      555 2023-05-06 08:09:00.000000 promptwatch-0.0.5/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-05-06 08:09:00.000000 promptwatch-0.0.5/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.0.5/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       28 2023-05-06 08:09:00.000000 promptwatch-0.0.5/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-05-06 08:09:00.000000 promptwatch-0.0.5/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.0.4/PKG-INFO` & `promptwatch-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.4
+Version: 0.0.5
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.4/README.md` & `promptwatch-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.4/setup.py` & `promptwatch-0.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.4/src/promptwatch/caching.py` & `promptwatch-0.0.5/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.4/src/promptwatch/client.py` & `promptwatch-0.0.5/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.4/src/promptwatch/data_model.py` & `promptwatch-0.0.5/src/promptwatch/data_model.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.4/src/promptwatch/decorators.py` & `promptwatch-0.0.5/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.4/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.0.5/src/promptwatch/langchain/langchain_support.py`

 * *Files 7% similar despite different names*

```diff
@@ -166,18 +166,30 @@
 
             if not prompt_template:
                 # lets create anonymous prompt template description
                 prompt_template = create_prompt_template_description(self.current_llm_chain.prompt)
 
             
             prompt_input_values = self.prompt_watch.current_activity.inputs
+            
+            # process history/chat messages placeholder (chat prompt)
+            
+
             if prompt_template and prompt_template.prompt_input_params and prompt_input_values:
-                prompt_input_values = {k:v for k,v in prompt_input_values.items() if k in prompt_template.prompt_input_params and isinstance(v,str)}
+                prompt_input_values = {k:v for k,v in prompt_input_values.items() if k in prompt_template.prompt_input_params and (isinstance(v,str) )}
             else:
                 prompt_input_values={k:v for k,v in prompt_input_values.items() if isinstance(v,str)}
+
+            if  prompt_template and isinstance(prompt_template.prompt_template,list):
+                non_text_input = {k:v for k,v in  self.prompt_watch.current_activity.inputs.items() if not isinstance(v,str)}
+                for k, v in non_text_input.items():
+                    if v and isinstance(v,list) and isinstance(v[0],BaseMessage):
+                        prompt_input_values[k] = convert_chat_messages(v)
+                        
+
         else:
             info_message="Could not retrieve all the additional information needed to for reproducible prompt execution. Consider registering the prompt template."
 
         if len(prompts)==1:
             
             self.prompt_watch._open_activity(LlmPrompt(
                 prompt= prompts[0], #why we have here more than one prompt?
@@ -225,17 +237,19 @@
 
         for thought, generated_responses in zip(thoughts, response.generations):
             thought.generated = "\n---\n".join([resp.text for resp in generated_responses])
             thought.metadata["generation_info"] = [resp.generation_info for resp in generated_responses] if len(generated_responses)>1 else generated_responses[0].generation_info
 
         if response.llm_output is not None:
             self.prompt_watch.current_activity.metadata["llm_output"]=response.llm_output
-            if "token_usage" in response.llm_output:
-                token_usage = response.llm_output["token_usage"]
-                if "total_tokens" in token_usage:
+            token_usage= response.llm_output.get("token_usage")
+            if token_usage and isinstance(token_usage,dict):
+                total_tokens = token_usage.get("total_tokens")
+                
+                if total_tokens:
                     self.prompt_watch.current_activity.metadata["total_tokens"] = self.prompt_watch.current_activity.metadata.get("total_tokens",0)+ token_usage["total_tokens"]
         self.prompt_watch._close_current_activity()
 
         
 
     
     def on_llm_error(
@@ -622,20 +636,37 @@
             if not cached_res:
 
                 llmresult:ChatResult = self.inner_llm._generate(prompts, stop) 
                 if callback:
                     callback(cached_res, llmresult.generations[0][0].text)
                 return llmresult
             else:
-                generation = Generation(text=cached_res.result, generation_info={"cached":True, **cached_res.metadata})
-                return LLMResult(generations=[[generation]])
+                generation = Generation(text=cached_res.result, generation_info={"cached":True, **cached_res.metadata,  "cache_namespace_key":cached_res.cache_namespace_key})
+                return LLMResult(generations=[[generation]], llm_output={"cached":True})
             
         else:
             return self.inner_llm._generate(prompts, stop) 
         
+    async def _agenerate(self, 
+                         prompts: List[str], stop: Optional[List[str]] = None
+        ) -> LLMResult:
+        if prompts and len(prompts)==1:
+            cached_res,callback=self._get_from_cache(prompts[0], stop=stop)
+            
+            if not cached_res:
+
+                chat_result:ChatResult = await self.inner_llm._agenerate(prompts, stop) 
+                if callback:
+                    callback(cached_res, chat_result.generations[0].text)
+                return chat_result
+            else:
+                generation = Generation(text=cached_res.result, generation_info={"cached":True, **cached_res.metadata,  "cache_namespace_key":cached_res.cache_namespace_key})
+                return LLMResult(generations=[[generation]], llm_output={"cached":True})
+        else:
+            return self.inner_llm._generate(prompts, stop) 
 
 
 class CachedChatLLM(BaseChatModel):
     
     inner_llm:Any
     cache_namespace_key:Optional[str]
     cache_embeddings:Optional[Embeddings]
@@ -688,29 +719,24 @@
         return (await self._agenerate(messages, stop=stop)).generations[0].message
         
     async def _agenerate(
        self, messages: List[BaseMessage], stop: Optional[List[str]] = None,**kwargs
     ):
         cached_res,callback=self._get_from_cache(messages, stop=stop)
         
-        
         if not cached_res:
 
-
             chat_result:ChatResult = await self.inner_llm._agenerate(messages, stop, **kwargs) 
             if callback:
                 callback(cached_res, chat_result.generations[0].text)
             return chat_result
         else:
             generated_msg = AIMessage(content=cached_res.result)
-            generation = ChatGeneration(message=generated_msg, generation_info={"cached":True, **cached_res.metadata})
-        
-       
-        
-        return ChatResult(generations=[generation])
+            generation = ChatGeneration(message=generated_msg, generation_info={"cached":True, **cached_res.metadata, "cache_namespace_key":cached_res.cache_namespace_key})
+            return ChatResult(generations=[generation],llm_output={"cached":True})
 
         
     def _generate(
         self, messages: List[BaseMessage], stop: Optional[List[str]] = None,**kwargs
     ) -> ChatResult:
         cached_res,callback=self._get_from_cache(messages, stop=stop)
         
@@ -720,11 +746,16 @@
 
             chat_result:ChatResult = self.inner_llm._generate(messages, stop,**kwargs) 
             if callback:
                 callback(cached_res, chat_result.generations[0].text)
             return chat_result
         else:
             generated_msg = AIMessage(content=cached_res.result)
-            generation = ChatGeneration(message=generated_msg, generation_info={"cached":True, **cached_res.metadata})
- 
-        return ChatResult(generations=[generation])
-    
+            generation = ChatGeneration(message=generated_msg, generation_info={"cached":True, **cached_res.metadata, "cache_namespace_key":cached_res.cache_namespace_key})
+            return ChatResult(generations=[generation],llm_output={"cached":True})
+    
+    def _combine_llm_outputs(self, llm_outputs: List[Optional[dict]]) -> dict:
+        """Combine llm outputs."""
+        if llm_outputs and len(llm_outputs)==1 and llm_outputs[0].get("cached"):
+            return llm_outputs[0]
+        else:
+            return self.inner_llm._combine_llm_outputs(llm_outputs)
```

### Comparing `promptwatch-0.0.4/src/promptwatch/promptwatch_context.py` & `promptwatch-0.0.5/src/promptwatch/promptwatch_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
 
         
 
     def _open_activity(self, activity:ActivityBase):
             
         if not self.current_session.session_name and isinstance(activity,ChainSequence) and activity.inputs:
             # if current session doesn't have a name, use first non empty input of first chain
-            self.current_session.session_name = next((v for k,v in activity.inputs.items() if v), None)
+            self.current_session.session_name = next((v for k,v in activity.inputs.items() if v and isinstance(v,str)), None)
 
         if not self.current_session.start_time:
             self.start_session()
         self.current_session.steps_count+=1
         activity.order=self.current_session.steps_count
 
         if self.current_activity:
```

### Comparing `promptwatch-0.0.4/src/promptwatch/utils.py` & `promptwatch-0.0.5/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.0.4/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.0.5/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.0.4
+Version: 0.0.5
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.0.4/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.0.5/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

