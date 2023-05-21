# Comparing `tmp/panml-0.0.13.tar.gz` & `tmp/panml-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "panml-0.0.13.tar", last modified: Fri May 19 11:10:30 2023, max compression
+gzip compressed data, was "panml-0.0.14.tar", last modified: Sun May 21 05:16:28 2023, max compression
```

## Comparing `panml-0.0.13.tar` & `panml-0.0.14.tar`

### file list

```diff
@@ -1,21 +1,25 @@
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-19 11:10:30.799528 panml-0.0.13/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.13/LICENSE
--rw-r--r--   0 williamzheng   (501) staff       (20)     1702 2023-05-19 11:10:30.799763 panml-0.0.13/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)     5031 2023-05-14 05:40:36.000000 panml-0.0.13/README.md
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-19 11:10:30.795682 panml-0.0.13/panml/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-02 06:31:00.000000 panml-0.0.13/panml/__init__.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-19 11:10:30.799051 panml-0.0.13/panml/base_models/
--rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 11:03:11.000000 panml-0.0.13/panml/base_models/__init__.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     8773 2023-05-19 11:03:11.000000 panml-0.0.13/panml/base_models/faiss.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    12533 2023-05-19 11:03:11.000000 panml-0.0.13/panml/base_models/huggingface.py
--rw-r--r--   0 williamzheng   (501) staff       (20)    11032 2023-05-19 11:03:11.000000 panml-0.0.13/panml/base_models/openai.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     4352 2023-05-19 11:03:11.000000 panml-0.0.13/panml/models.py
--rw-r--r--   0 williamzheng   (501) staff       (20)     3303 2023-05-19 11:03:11.000000 panml-0.0.13/panml/search.py
-drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-19 11:10:30.797565 panml-0.0.13/panml.egg-info/
--rw-r--r--   0 williamzheng   (501) staff       (20)     1702 2023-05-19 11:10:30.000000 panml-0.0.13/panml.egg-info/PKG-INFO
--rw-r--r--   0 williamzheng   (501) staff       (20)      348 2023-05-19 11:10:30.000000 panml-0.0.13/panml.egg-info/SOURCES.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-19 11:10:30.000000 panml-0.0.13/panml.egg-info/dependency_links.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)      196 2023-05-19 11:10:30.000000 panml-0.0.13/panml.egg-info/requires.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-19 11:10:30.000000 panml-0.0.13/panml.egg-info/top_level.txt
--rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-19 11:10:30.800475 panml-0.0.13/setup.cfg
--rw-r--r--   0 williamzheng   (501) staff       (20)     2701 2023-05-19 11:05:18.000000 panml-0.0.13/setup.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:16:28.854595 panml-0.0.14/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1063 2023-05-11 06:11:04.000000 panml-0.0.14/LICENSE
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1702 2023-05-21 05:16:28.854945 panml-0.0.14/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)     5031 2023-05-14 05:40:36.000000 panml-0.0.14/README.md
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:16:28.849211 panml-0.0.14/panml/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-19 12:08:24.000000 panml-0.0.14/panml/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:16:28.851391 panml-0.0.14/panml/core/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.14/panml/core/__init__.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:16:28.852148 panml-0.0.14/panml/core/clustering/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.14/panml/core/clustering/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     8786 2023-05-21 05:11:31.000000 panml-0.0.14/panml/core/clustering/faiss.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:16:28.853964 panml-0.0.14/panml/core/llm/
+-rw-r--r--   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:11:31.000000 panml-0.0.14/panml/core/llm/__init__.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    13683 2023-05-21 05:11:31.000000 panml-0.0.14/panml/core/llm/huggingface.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)    11105 2023-05-21 05:11:31.000000 panml-0.0.14/panml/core/llm/openai.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     4578 2023-05-21 05:11:31.000000 panml-0.0.14/panml/models.py
+-rw-r--r--   0 williamzheng   (501) staff       (20)     3307 2023-05-21 05:11:31.000000 panml-0.0.14/panml/search.py
+drwxr-xr-x   0 williamzheng   (501) staff       (20)        0 2023-05-21 05:16:28.850875 panml-0.0.14/panml.egg-info/
+-rw-r--r--   0 williamzheng   (501) staff       (20)     1702 2023-05-21 05:16:28.000000 panml-0.0.14/panml.egg-info/PKG-INFO
+-rw-r--r--   0 williamzheng   (501) staff       (20)      400 2023-05-21 05:16:28.000000 panml-0.0.14/panml.egg-info/SOURCES.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        1 2023-05-21 05:16:28.000000 panml-0.0.14/panml.egg-info/dependency_links.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)      215 2023-05-21 05:16:28.000000 panml-0.0.14/panml.egg-info/requires.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)        6 2023-05-21 05:16:28.000000 panml-0.0.14/panml.egg-info/top_level.txt
+-rw-r--r--   0 williamzheng   (501) staff       (20)       79 2023-05-21 05:16:28.856517 panml-0.0.14/setup.cfg
+-rw-r--r--   0 williamzheng   (501) staff       (20)     2731 2023-05-21 05:16:16.000000 panml-0.0.14/setup.py
```

### Comparing `panml-0.0.13/LICENSE` & `panml-0.0.14/LICENSE`

 * *Files identical despite different names*

### Comparing `panml-0.0.13/PKG-INFO` & `panml-0.0.14/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.13
+Version: 0.0.14
 Summary: PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.13/README.md` & `panml-0.0.14/README.md`

 * *Files identical despite different names*

### Comparing `panml-0.0.13/panml/base_models/faiss.py` & `panml-0.0.14/panml/core/clustering/faiss.py`

 * *Files 7% similar despite different names*

```diff
@@ -39,37 +39,37 @@
         if model_emb_source == 'huggingface':
             return self.model_emb.encode(corpus)
         elif model_emb_source == 'openai':
             df_corpus = pd.DataFrame({'corpus': corpus})
             return np.array(df_corpus['corpus'].apply(lambda x: self._get_openai_embedding(x, model=self.model)).tolist())
 
     # Store the corpus as vectors
-    def store(self, corpus: list[str], save_name: str='stored', 
+    def store(self, corpus: list[str], model_name: str='stored', 
               mode: str='flat', nlist: int=None, m: int=None, bits: int=None) -> None:
         '''
         This creates the vector index stored for vector search. 
 
         Args:
         corpus: list of texts containing the document contents forming the corpus to be searched
-        save_name: custom name affix of the vectors and corpus assigned to the saved files (file type extension should not to be included)
+        model_name: custom model name affix of the vectors and corpus assigned to the saved files (file type extension should not to be included)
         mode: parameter of FAISS vector search (flat, ivfflat, ivfpq) can improve speed, at the potentially the trade-off with accuracy
         nlist: parameter of mode: 'flat', specifies the number of partitions in the vectors space
         m: parameter of the mode: 'ivfpq', specifies the number of centroid IDs in compressed vectors
         bits: parameter of mode: 'ivfpq', specifies the number of bits in each centroid
 
         Returns:
         None. Vectors store is setup, and if specified, the vectors and corpus are saved to files
         '''   
         # Catch input exceptions
         if not isinstance(corpus, list):
             raise TypeError('Input corpus needs to be of type: list')
         if len(corpus) < 1:
             raise ValueError('Input text corpus is empty')
-        if save_name is not None:
-            if not isinstance(save_name, str):
+        if model_name is not None:
+            if not isinstance(model_name, str):
                 raise TypeError('Input save name needs to be of type: str')
         if not isinstance(mode, str):
             raise TypeError('Input mode needs to be of type: str')
         if mode not in ['flat', 'ivfflat', 'ivfpq']:
             raise ValueError('Supported mode options are: flat, ivfflat, ivfpq')
         if nlist is not None:
             if not isinstance(nlist, int):
@@ -114,17 +114,17 @@
                 self.vectors.train(emb)
                 self.vectors.add(emb)
                 self.vectors.make_direct_map()
             else:
                 raise ValueError('IVFPQ vector search not set due to missing m and bits inputs')
 
         # Saving the vector store
-        if save_name:
-            faiss.write_index(self.vectors, f"{save_name}_vectors.faiss") # vectors file
-            with open(f"{save_name}_corpus.pkl", "wb") as f: # corpus file
+        if model_name:
+            faiss.write_index(self.vectors, f"{model_name}_vectors.faiss") # vectors file
+            with open(f"{model_name}_corpus.pkl", "wb") as f: # corpus file
                 pickle.dump(self.corpus, f)
         
     # Load vectors and corpus
     def load(self, vectors_dir: str, corpus_dir: str) -> None:
         '''
         This loads the stored vectors (FAISS index) and the corresonding corpus (list object) for use in docs search
```

### Comparing `panml-0.0.13/panml/base_models/huggingface.py` & `panml-0.0.14/panml/core/llm/huggingface.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,37 +7,39 @@
 
 # HuggingFace model class
 class HuggingFaceModelPack:
     '''
     HuggingFace Hub model pack class
     '''
     # Initialize class variables
-    def __init__(self, model: str, input_block_size: int, padding_length: int, tokenizer_batch: bool, source: str) -> None:
-        if source == 'huggingface':
-            if 'flan' in model:
-                self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(model)
-            else:
-                self.model_hf = AutoModelForCausalLM.from_pretrained(model)
-        elif source == 'local':
-            if 'flan' in model:
-                self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(model, local_files_only=True)
-            else:
-                self.model_hf = AutoModelForCausalLM.from_pretrained(model, local_files_only=True)
-        if self.model_hf.config.tokenizer_class:
-            self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
-        else:
-            self.tokenizer = AutoTokenizer.from_pretrained(model, mirror='https://huggingface.co')
+    def __init__(self, model: str, input_block_size: int, padding_length: int, tokenizer_batch: bool, source: str, model_args: dict) -> None:
+        self.model_name = model
         self.padding_length = padding_length
         self.input_block_size = input_block_size
         self.tokenizer_batch = tokenizer_batch
         self.train_default_args = ['title', 'num_train_epochs', 'optimizer', 'mlm', 
                                    'per_device_train_batch_size', 'per_device_eval_batch_size',
                                    'warmup_steps', 'weight_decay', 'logging_steps', 
                                    'output_dir', 'logging_dir', 'save_model']
         
+        if source == 'huggingface':
+            if 'flan' in self.model_name:
+                self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args)
+            else:
+                self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args)
+        elif source == 'local':
+            if 'flan' in self.model_name:
+                self.model_hf = AutoModelForSeq2SeqLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
+            else:
+                self.model_hf = AutoModelForCausalLM.from_pretrained(self.model_name, **model_args, local_files_only=True)
+        if self.model_hf.config.tokenizer_class:
+            self.tokenizer = AutoTokenizer.from_pretrained(self.model_hf.config.tokenizer_class.lower().replace('tokenizer', ''), mirror='https://huggingface.co')
+        else:
+            self.tokenizer = AutoTokenizer.from_pretrained(self.model_name, mirror='https://huggingface.co')
+        
         if self.tokenizer.pad_token is None:
             self.tokenizer.pad_token = self.model_hf.config.eos_token_id
     
     # Embed text
     def embedding(self, text: str) -> torch.Tensor:
         '''
         Gets the embedding of the text using open source collections of models from HuggingFace Hub
@@ -140,49 +142,58 @@
             tokenized_dataset = hf_dataset.map(self._tokenize_function, batched=batched, num_proc=num_proc)
         else:
             tokenized_dataset = hf_dataset.map(self._tokenize_function)
 
         return tokenized_dataset
     
     # Model training
-    def fit(self, x: list[str], y: list[str], train_args: dict[str, Union[str, int, float]]={}, 
-            instruct: bool=False, num_proc=4) -> None:
+    def fit(self, x: Union[list[str], pd.Series], y: Union[list[str], pd.Series], train_args: dict[str, Union[str, int, float]]={}, 
+            instruct: bool=False, num_proc: int=4) -> None:
         '''
         Fine tuning of a language model from HuggingFace Hub
 
         Args:
         x: list of example text for training/fine tuning the language model
         y: list of example text as targets for training/fine tuning the language model. 
         Note: For autogressive based training, this parameter is set to be same as x. For instruct based training, this parameter is part of the target examples for supervised fine tuning.
         train_args: parameters to be fed into HuggingFace Hub's training_args dict, as required for training
         num_proc: parameter from HuggingFace Hub, specifies max number of processes when generating cache. Already cached shards are loaded sequentially
 
         Returns: 
         None. Trained model is saved in the .result/ folder with name "model_" prepended to the specified title
         '''
         # Catch input exceptions
+        if isinstance(x, pd.Series): # convert to list from pandas series if available
+            x = x.tolist()
         if not isinstance(x, list):
             raise TypeError('Input data array, x, needs to be of type: list')
+        if isinstance(y, pd.Series): # convert to list from pandas series if available
+            y = y.tolist()
         if not isinstance(y, list):
             raise TypeError('Input data array, y, needs to be of type: list')
         if not isinstance(train_args, dict):
             raise TypeError('Input train args needs to be of type: dict')
+        if not isinstance(num_proc, int):
+            raise TypeError('Input num proc needs to be of type: int')
+        else:
+            if num_proc < 1:
+                raise ValueError('Input num proc cannot be less than 1')
             
         # Convert to tokens format from pandas dataframes
         tokenized_data = self.tokenize_text(x, batched=self.tokenizer_batch, num_proc=num_proc)
         tokenized_target = self.tokenize_text(y, batched=self.tokenizer_batch, num_proc=num_proc)
         
         # Check for missing input arguments
         if set(list(train_args.keys())) != set(self.train_default_args):
             raise ValueError(f'Train args are not in the required format - missing: {", ".join(list(set(self.train_default_args) - set(list(train_args.keys()))))}')
         
         if instruct:
             print('Setting up training in sequence to sequence format...')
             tokenized_data = tokenized_data.add_column('labels', tokenized_target['input_ids']) # Create target sequence labels
-            data_collator = DataCollatorForSeq2Seq(tokenizer=self.tokenizer, model=self.model) # Organise data for training
+            data_collator = DataCollatorForSeq2Seq(tokenizer=self.tokenizer) # Organise data for training
             
             # Setup training in sequence to sequence format
             training_args = TrainingArguments(
                 optim=train_args['optimizer'], # model optimisation function
                 num_train_epochs=train_args['num_train_epochs'], # total number of training epochs
                 per_device_train_batch_size=train_args['per_device_train_batch_size'],  # batch size per device during training
                 per_device_eval_batch_size=train_args['per_device_eval_batch_size'],   # batch size for evaluation
@@ -225,8 +236,23 @@
                 eval_dataset=tokenized_data.remove_columns(['text']),
                 data_collator=data_collator,
             )
 
         trainer.train() # Execute training
         
         if train_args['save_model']:
-            trainer.save_model(f'./results/model_{train_args["title"]}') # Save trained model
+            trainer.save_model(f'./results/model_{train_args["title"]}') # Save trained model
+
+    # Save model
+    def save(self, save_dir: str=None) -> None:
+        '''
+        Save the model on demand
+
+        Args:
+        save_dir: relative path of the file. If directory is not provided, the default directory is set to ".results/model_<model_name>"
+
+        Returns:
+        None. File is saved at the specified location
+        '''
+        if save_dir is None:
+            save_dir = f'./results/model_{self.model_name}'
+        self.model_hf.save_pretrained(save_dir)
```

### Comparing `panml-0.0.13/panml/base_models/openai.py` & `panml-0.0.14/panml/core/llm/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 import pandas as pd
+import torch
 from typing import Union
 import openai
 
 # OpenAI model class
 class OpenAIModelPack:
     '''
     OpenAI model pack class
     '''
     def __init__(self, model: str, api_key: str) -> None:
-        self.model = model
+        self.model_name = model
         self.model_embedding = 'text-embedding-ada-002'
         openai.api_key = api_key
     
     # Generate text of single model call
     @staticmethod
-    def _predict(model: str, text: str, temperature: float, max_tokens: int, top_p: float, n: int, 
+    def _predict(model_name: str, text: str, temperature: float, max_tokens: int, top_p: float, n: int, 
                  frequency_penalty: float, presence_penalty: float, display_probability: bool, logprobs: int, 
                  chat_role: str) -> dict[str, str]:
         '''
         Base function for text generation using OpenAI models
         '''
         output_context = {
             'text': None,
@@ -29,47 +30,47 @@
             'text-davinci-002', 
             'text-davinci-003',
         ]
         chat_completion_models = [
             'gpt-3.5-turbo',
             'gpt-3.5-turbo-0301',
         ]
-        if model in completion_models:
+        if model_name in completion_models:
             response = openai.Completion.create(
-                model=model,
+                model=model_name,
                 prompt=text,
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
                 n=n,
                 frequency_penalty=frequency_penalty,
                 presence_penalty=presence_penalty,
                 logprobs=logprobs
             )
             output_context['text'] = response['choices'][0]['text']
             
-        elif model in chat_completion_models:
+        elif model_name in chat_completion_models:
             response = openai.ChatCompletion.create(
-                model=model,
+                model=model_name,
                 messages = [
                     {'role': chat_role, 'content': text}
                 ],
                 temperature=temperature,
                 max_tokens=max_tokens,
                 top_p=top_p,
                 n=n,
                 frequency_penalty=frequency_penalty,
                 presence_penalty=presence_penalty,
             )
             output_context['text'] = response['choices'][0]['message']['content']
         else:
-            raise ValueError(f'{model} is not currently supported in this package')
+            raise ValueError(f'{model_name} is not currently supported in this package')
 
         # Get probability of output tokens
-        if display_probability and model in completion_models:
+        if display_probability and model_name in completion_models:
             tokens = response["choices"][0]['logprobs']['tokens']
             token_logprobs = response["choices"][0]['logprobs']['token_logprobs']
             output_context['probability'] = [{'token': token, 'probability': torch.exp(torch.Tensor([logprob])).item()} for token, logprob in zip(tokens, token_logprobs)]
 
             # Calculate perplexity of output
             output_context['perplexity'] = (1/torch.prod(torch.tensor([torch.exp(torch.Tensor([logprob])).item() for logprob in token_logprobs])).item())**(1/len(tokens))
 
@@ -124,15 +125,15 @@
 
             # Set the query text to previous output to carry on the prompt loop
             if count > 0:
                 text = output_context['text']
             text = f"{mod['prepend']} \n {text} \n {mod['append']}"
 
             # Call model for text generation
-            output_context = self._predict(self.model, text, temperature=temperature, max_tokens=max_tokens, top_p=top_p,
+            output_context = self._predict(self.model_name, text, temperature=temperature, max_tokens=max_tokens, top_p=top_p,
                                            n=n, frequency_penalty=frequency_penalty, presence_penalty=presence_penalty,
                                            display_probability=display_probability, logprobs=logprobs, chat_role=chat_role)
 
             # Terminate loop for next prompt when context contains no meaningful words (less than 2)
             response_words = output_context['text'].replace('\n', '').replace(' ', '')
             if len(response_words) < 2:
                 break
@@ -160,16 +161,16 @@
         langauge: programming language of the code to be generated
         max_tokens: max number of tokens to be generated from OpenAI API
    
         Returns: 
         text of generated code
         '''
         # Catch input exceptions
-        if self.model != 'text-davinci-002' and self.model != 'text-davinci-003':
-            raise ValueError(f"The specified model is '{self.model}'. Only 'text-davinci-002' and 'text-davinci-002' are supported in this package for code generation")
+        if self.model_name != 'text-davinci-002' and self.model_name != 'text-davinci-003':
+            raise ValueError(f"The specified model is '{self.model_name}'. Only 'text-davinci-002' and 'text-davinci-002' are supported in this package for code generation")
         if not isinstance(text, str):
             raise TypeError('Input text needs to be of type: string')
         if not isinstance(x, int) and not isinstance(x, float) and \
             not isinstance(x, str) and not isinstance(x, pd.DataFrame):
             raise TypeError('Input x needs to be of type: int, float, str or pandas dataframe')
         if not isinstance(variable_names, dict):
             raise TypeError('Input variable names needs to be of type: dict')
```

### Comparing `panml-0.0.13/panml/models.py` & `panml-0.0.14/panml/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 # Dependencies for data processing and general machine learning implementations
 import torch
 from typing import Union
 
 # Dependencies for specialised language model implementations
 from transformers import AutoTokenizer
-from panml.base_models.huggingface import HuggingFaceModelPack
-from panml.base_models.openai import OpenAIModelPack
+from panml.core.llm.huggingface import HuggingFaceModelPack
+from panml.core.llm.openai import OpenAIModelPack
         
 # Entry model pack class           
 class ModelPack:
     '''
     Main model pack class
     '''
     def __init__(self, model: str, tokenizer: AutoTokenizer=None, input_block_size: int=20, padding_length: int=100, 
-                 tokenizer_batch: bool=False, source: str='huggingface', api_key: str=None) -> None:
+                 tokenizer_batch: bool=False, source: str='huggingface', api_key: str=None, model_args={}) -> None:
         self.padding_length = padding_length
         self.tokenizer = tokenizer
         self.model = model
         self.input_block_size = input_block_size
         self.tokenizer_batch = tokenizer_batch
         self.source = source
         self.api_key = api_key
+        self.model_args = model_args
         
         # Accepted models from sources
         self.supported_models = {
             'huggingface': [
                 'distilgpt2', 
                 'gpt2',
                 'gpt2-medium',
@@ -39,22 +40,25 @@
                 'cerebras/Cerebras-GPT-590M',
                 'cerebras/Cerebras-GPT-1.3B',
                 'cerebras/Cerebras-GPT-2.7B',
                 'cerebras/Cerebras-GPT-6.7B',
                 'cerebras/Cerebras-GPT-13B',
                 'EleutherAI/gpt-neo-2.7B',
                 'EleutherAI/gpt-j-6B',
+                'togethercomputer/GPT-JT-6B-v1',
+                'togethercomputer/GPT-NeoXT-Chat-Base-20B',
                 'StabilityAI/stablelm-base-alpha-3b',
                 'StabilityAI/stablelm-base-alpha-7b',
                 'StabilityAI/stablelm-tuned-alpha-3b',
                 'StabilityAI/stablelm-tuned-alpha-7b',
                 'h2oai/h2ogpt-oasst1-512-12b',
                 'h2oai/h2ogpt-oasst1-512-20b',
                 'Salesforce/codegen-350M-multi',
                 'Salesforce/codegen-2B-multi',
+                'bigcode/starcoder',
             ],
             'openai': [
                 'text-davinci-002', 
                 'text-davinci-003',
                 'gpt-3.5-turbo',
                 'gpt-3.5-turbo-0301',
             ],
@@ -71,19 +75,19 @@
         if self.source not in self.supported_sources:
             raise ValueError('The specified source is not recognized. Supported sources are: ' + ' '.join([f"{s}" for s in self.supported_sources]))
 
         # HuggingFace Hub model call
         if self.source == 'huggingface':
             if self.model not in self.supported_models['huggingface']:
                 raise ValueError('The specified model is currently not supported in this package. Supported HuggingFace Hub models are: ' + ' '.join([f"{m}" for m in self.supported_models['huggingface']]))
-            self.instance = HuggingFaceModelPack(self.model, self.input_block_size, self.padding_length, self.tokenizer_batch, self.source)
+            self.instance = HuggingFaceModelPack(self.model, self.input_block_size, self.padding_length, self.tokenizer_batch, self.source, self.model_args)
 
         # Locally trained model call of HuggingFace Hub model
         elif self.source == 'local':
-            self.instance = HuggingFaceModelPack(self.model, self.input_block_size, self.padding_length, self.tokenizer_batch, self.source)
+            self.instance = HuggingFaceModelPack(self.model, self.input_block_size, self.padding_length, self.tokenizer_batch, self.source, self.model_args)
 
         # OpenAI model call
         elif self.source == 'openai':
             if self.model not in self.supported_models['openai']:
                 raise ValueError('The specified model currently is not supported in this pacckage. Supported OpenAI models are: ' + ' '.join([f"{m}" for m in self.supported_models['openai']]))
             if self.api_key is None:
                 raise ValueError('api key has not been specified for OpenAI model call')
```

### Comparing `panml-0.0.13/panml/search.py` & `panml-0.0.14/panml/search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Dependencies for data processing and general machine learning implementations
 import torch
 import torch.nn.functional as F
 from typing import Union
 
 # Dependencies for vector search
-from panml.base_models.faiss import FAISSVectorEngine
+from panml.core.clustering.faiss import FAISSVectorEngine
 
 # Entry vector engine class           
 class VectorEngine:
     '''
     Main vector engine class
     '''
     def __init__(self, model: str='all-MiniLM-L6-v2', source: str='faiss', api_key: str=None) -> None:
```

### Comparing `panml-0.0.13/panml.egg-info/PKG-INFO` & `panml-0.0.14/panml.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panml
-Version: 0.0.13
+Version: 0.0.14
 Summary: PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.
 Home-page: https://github.com/Pan-ML/panml
 Author: PanML team
 Author-email: teampanml@gmail.com
 License: MIT
 Keywords: generative AI,generative model,machine learning,large language model,LLM,prompt engineering,fine tuning,prompt tuning,retrieval augmentation,AI safety,AI alignment
 Platform: UNKNOWN
```

### Comparing `panml-0.0.13/setup.py` & `panml-0.0.14/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 setup(
   name = 'panml', # package name     
   packages = find_packages(exclude=['test']), # package name
-  version = '0.0.13', # version
+  version = '0.0.14', # version
   license = 'MIT', # license
   description = 'PanML is a generative AI/ML development toolkit designed for ease of use and fast experimentation.', # short description about the package
   long_description = 'PanML aims to make analysis and experimentation of generative AI/ML models more accessible, by providing a simple and consistent interface to foundation models for Data Scientists, Machine Learning Engineers and Software Developers. \
                       The package provides various assistive tools to work with generative language models, such as prompt engineering, fine tuning and others. \
                       \n\nQuick start guide: https://github.com/Pan-ML/panml/wiki/1.-Quick-start-guide \
                       \n\nDocumentation/Wiki: https://github.com/Pan-ML/panml/wiki', # long description
   author = 'PanML team', # team name
@@ -21,17 +21,18 @@
         'numpy>=1.22.4',
         'openai>=0.27.6',
         'pandas>=2.0.1',
         'tokenizers>=0.13.3',
         'datasets>=2.12.0',
         'torch>=2.0.0',
         'tqdm>=4.65.0',
-        'transformers>=4.29.1',
+        'transformers<=4.27.4',
         'faiss-cpu>=1.7.4',
         'sentence-transformers>=2.2.2',
+        'accelerate<=0.19.0',
       ],
   classifiers=[
     'Development Status :: 4 - Beta', # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of the package
     'Intended Audience :: Science/Research', # Define the audience type
     'Intended Audience :: Developers',
     'Intended Audience :: Education',
     'Intended Audience :: Information Technology',
```

