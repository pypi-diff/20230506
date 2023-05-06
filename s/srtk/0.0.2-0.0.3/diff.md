# Comparing `tmp/srtk-0.0.2.tar.gz` & `tmp/srtk-0.0.3.tar.gz`

## Comparing `srtk-0.0.2.tar` & `srtk-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,54 @@
--rw-r--r--   0        0        0     8300 2020-02-02 00:00:00.000000 srtk-0.0.2/graphs-for-paper.ipynb
--rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 srtk-0.0.2/requirements.txt
--rw-r--r--   0        0        0     4679 2020-02-02 00:00:00.000000 srtk-0.0.2/sample_commands.ipynb
--rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 srtk-0.0.2/test.pdf
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 srtk-0.0.2/train_qald.ipynb
--rw-r--r--   0        0        0    23773 2020-02-02 00:00:00.000000 srtk-0.0.2/train_wd_simple.ipynb
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 srtk-0.0.2/.github/workflows/pytest.yml
-lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/resources/wikimapper/index_enwiki.db -> /home/wiss/liao/shen/flamingo-gnn/data/kilt/index_enwiki-latest-uncased.db
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/__init__.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/cli.py
--rw-r--r--   0        0        0     4201 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/link.py
--rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocess.py
--rw-r--r--   0        0        0    14027 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/retrieve.py
--rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/train.py
--rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/visualize.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/entity_linking/freebase.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/knowledge_graph/__init__.py
--rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/knowledge_graph/freebase.py
--rw-r--r--   0        0        0     2875 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/knowledge_graph/graph_base.py
--rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/knowledge_graph/wikidata.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/__init__.py
--rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/load_dataset.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/merge_ground.py
--rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/negative_sampling.py
--rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/score_path.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/preprocessing/search_path.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/scorer/__init__.py
--rw-r--r--   0        0        0     5052 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/scorer/encoder.py
--rw-r--r--   0        0        0     3211 2020-02-02 00:00:00.000000 srtk-0.0.2/src/srtk/scorer/scorer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/test_encoder.py
--rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/test_freebase.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/test_scorer.py
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 srtk-0.0.2/tests/test_wikidata.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/1.get_started.ipynb
--rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/2.end_to_end_subgraph_retrieval.ipynb
--rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/3.weak_train_wikidata.ipynb
--rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/4.weak_train_freebase.ipynb
--rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/5.supervised_train_wikidata.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.2/tutorials/6.extend_to_new_kg.ipynb
--rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 srtk-0.0.2/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 srtk-0.0.2/LICENSE
--rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 srtk-0.0.2/README.md
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 srtk-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 srtk-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     8400 2020-02-02 00:00:00.000000 srtk-0.0.3/graphs-for-paper.ipynb
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 srtk-0.0.3/linked.jsonl
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 srtk-0.0.3/question.jsonl
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 srtk-0.0.3/requirements.txt
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 srtk-0.0.3/sample_commands.ipynb
+-rw-r--r--   0        0        0    10348 2020-02-02 00:00:00.000000 srtk-0.0.3/test.pdf
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 srtk-0.0.3/train_qald.ipynb
+-rw-r--r--   0        0        0    23772 2020-02-02 00:00:00.000000 srtk-0.0.3/train_wd_simple.ipynb
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 srtk-0.0.3/.github/workflows/pytest.yml
+lrwxr-xr-x   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/resources/wikimapper/index_enwiki.db -> /home/wiss/liao/shen/flamingo-gnn/data/kilt/index_enwiki-latest-uncased.db
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/__init__.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/cli.py
+-rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/link.py
+-rw-r--r--   0        0        0     5420 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocess.py
+-rw-r--r--   0        0        0    15562 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/retrieve.py
+-rw-r--r--   0        0        0     5755 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/train.py
+-rw-r--r--   0        0        0      757 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/utils.py
+-rw-r--r--   0        0        0     4646 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/visualize.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/entity_linking/__init__.py
+-rw-r--r--   0        0        0     2196 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/entity_linking/dbpedia.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/entity_linking/freebase.py
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/entity_linking/wikidata.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/__init__.py
+-rw-r--r--   0        0        0     6593 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/dbpedia.py
+-rw-r--r--   0        0        0     8254 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/freebase.py
+-rw-r--r--   0        0        0     2877 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/graph_base.py
+-rw-r--r--   0        0        0    10620 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/knowledge_graph/wikidata.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/__init__.py
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/load_dataset.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/merge_ground.py
+-rw-r--r--   0        0        0    10074 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/negative_sampling.py
+-rw-r--r--   0        0        0     4081 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/score_path.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/preprocessing/search_path.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/scorer/__init__.py
+-rw-r--r--   0        0        0     6803 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/scorer/encoder.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 srtk-0.0.3/src/srtk/scorer/scorer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_dbpedia.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_encoder.py
+-rw-r--r--   0        0        0     2991 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_freebase.py
+-rw-r--r--   0        0        0      731 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_link.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_scorer.py
+-rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 srtk-0.0.3/tests/test_wikidata.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/1.get_started.ipynb
+-rw-r--r--   0        0        0    25547 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/2.end_to_end_subgraph_retrieval.ipynb
+-rw-r--r--   0        0        0    24937 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/3.weak_train_wikidata.ipynb
+-rw-r--r--   0        0        0    17127 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/4.weak_train_freebase.ipynb
+-rw-r--r--   0        0        0    22909 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/5.supervised_train_wikidata.ipynb
+-rw-r--r--   0        0        0     6352 2020-02-02 00:00:00.000000 srtk-0.0.3/tutorials/6.extend_to_new_kg.ipynb
+-rw-r--r--   0        0        0     1954 2020-02-02 00:00:00.000000 srtk-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 srtk-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5374 2020-02-02 00:00:00.000000 srtk-0.0.3/README.md
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 srtk-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6187 2020-02-02 00:00:00.000000 srtk-0.0.3/PKG-INFO
```

### Comparing `srtk-0.0.2/graphs-for-paper.ipynb` & `srtk-0.0.3/graphs-for-paper.ipynb`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.994049935630818%*

 * *Differences: {"'cells'": '{2: {\'execution_count\': 1, \'source\': {insert: [(3, "retrieve_subgraph_dir = '*

 * *            '\'artifacts/subgraphs/wikidata-simple-question-t5-e0\'\\n"), (4, "trained_model_dir = '*

 * *            '\'artifacts/models/wd_simple_t5_e10\'\\n"), (5, "test_scored_path = '*

 * *            'os.path.join(intermediate_dir, \'scores_valid.jsonl\')")], delete: [5, 4, 3]}}, 3: '*

 * *            "{'execution_count': 2, 'outputs': {0: {'text': ['Retrieving subgraphs: "*

 * *            "100%|█████████████████| 2210/2210 [0 […]*

```diff
@@ -16,49 +16,49 @@
                 "## Wikidata Simple Question\n",
                 "\n",
                 "Under beam size 2, 5, 10, 20, how the coverage and the graph size vary?"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 3,
+            "execution_count": 1,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import os\n",
                 "\n",
                 "intermediate_dir = 'data/wikidata-simplequestions/intermediate'\n",
-                "retrieve_subgraph_dir = 'artifacts/subgraphs/wikidata-simple-question-llr'\n",
-                "trained_model_dir = 'artifacts/models/wd_simple_e5'\n",
-                "test_scored_path = os.path.join(intermediate_dir, 'scores_test.jsonl')"
+                "retrieve_subgraph_dir = 'artifacts/subgraphs/wikidata-simple-question-t5-e0'\n",
+                "trained_model_dir = 'artifacts/models/wd_simple_t5_e10'\n",
+                "test_scored_path = os.path.join(intermediate_dir, 'scores_valid.jsonl')"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 4,
+            "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Retrieving subgraphs: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 4296/4296 [01:35<00:00, 44.87it/s]\n",
-                        "Retrieved subgraphs saved to to artifacts/subgraphs/wikidata-simple-question-llr/e5-b-2.jsonl\n",
-                        "Answer recall: 0.08612662942271881 (370 / 4296)\n"
+                        "Retrieving subgraphs: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 2210/2210 [03:30<00:00, 10.48it/s]\n",
+                        "Retrieved subgraphs saved to to artifacts/subgraphs/wikidata-simple-question-t5-e0/e5-b-1.jsonl\n",
+                        "Answer recall: 0.9638009049773756 (2130 / 2210)\n"
                     ]
                 }
             ],
             "source": [
-                "for beam_width in [2]:\n",
+                "for beam_width in [1]:\n",
                 "    retrieved_subgraph_path = os.path.join(retrieve_subgraph_dir, f'e5-b-{beam_width}.jsonl')\n",
                 "    !srtk retrieve -i $test_scored_path \\\n",
                 "        -o $retrieved_subgraph_path \\\n",
                 "        -e http://localhost:1234/api/endpoint/sparql \\\n",
                 "        -kg wikidata \\\n",
-                "        --scorer-model-path $trained_model_dir \\\n",
+                "        --scorer-model-path drt/wikidata-simplequestions \\\n",
                 "        --beam-width $beam_width \\\n",
                 "        --max-depth 1 \\\n",
                 "        --evaluate"
             ]
         },
         {
             "cell_type": "code",
@@ -86,42 +86,42 @@
                 "    --beam-width $beam_width \\\n",
                 "    --max-depth 1 \\\n",
                 "    --evaluate"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 2,
+            "execution_count": 14,
             "metadata": {},
             "outputs": [],
             "source": [
                 "import srsly\n",
                 "import statistics"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 6,
+            "execution_count": 16,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[0.1980912477, 0.4979050279, 0.8251862197000001, 0.969972067]\n",
-                        "[1.6464152700186219, 5.9946461824953445, 12.184590316573557, 17.55214152700186]\n"
+                        "[0.963800905, 0.9728506787000001, 0.9760180995000001, 0.9796380090000001, 0.9805429864]\n",
+                        "[1.616289592760181, 2.4624434389140273, 6.160633484162896, 12.227149321266968, 18.228054298642533]\n"
                     ]
                 }
             ],
             "source": [
-                "wikidata_sq_subgraph_path_pattern = 'artifacts/subgraphs/wikidata-simple-question-old/e5-b-{beam}.jsonl'\n",
-                "metric_path_pattern = 'artifacts/subgraphs/wikidata-simple-question-old/e5-b-{beam}.metric'\n",
+                "wikidata_sq_subgraph_path_pattern = 'artifacts/subgraphs/wikidata-simple-question-e10/e5-b-{beam}.jsonl'\n",
+                "metric_path_pattern = 'artifacts/subgraphs/wikidata-simple-question-e10/e5-b-{beam}.metric'\n",
                 "subgraph_means = []\n",
                 "recalls = []\n",
-                "for beam in [2, 5, 10, 20]:\n",
+                "for beam in [1, 2, 5, 10, 20]:\n",
                 "    subgraph_path = wikidata_sq_subgraph_path_pattern.format(beam=beam)\n",
                 "    metric_path = metric_path_pattern.format(beam=beam)\n",
                 "    subgraphs = srsly.read_jsonl(subgraph_path)\n",
                 "    metric = srsly.read_json(metric_path)\n",
                 "    avg_n_triplets = statistics.mean([len(sg['triplets']) for sg in subgraphs])\n",
                 "    recalls.append(metric['recall'])\n",
                 "    subgraph_means.append(avg_n_triplets)\n",
@@ -143,21 +143,21 @@
             "metadata": {},
             "source": [
                 "## WebQSP"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 5,
+            "execution_count": 8,
             "metadata": {},
             "outputs": [],
             "source": [
                 "formatted_data_dir = 'data/webqsp/formatted'\n",
                 "retrieve_subgraph_dir = 'artifacts/subgraphs/webqsp'\n",
-                "webqsp_model_dir = 'artifacts/models/scorer-freebase'\n",
+                "webqsp_model_dir = 'artifacts/models/webqsp'\n",
                 "formatted_test_path = os.path.join(formatted_data_dir, 'test.jsonl')"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": 6,
             "metadata": {},
@@ -167,46 +167,46 @@
                     "output_type": "stream",
                     "text": [
                         "Retrieving subgraphs:   8%|\u2588\u258c                | 133/1582 [01:36<08:38,  2.79it/s]"
                     ]
                 }
             ],
             "source": [
-                "for beam_width in [2, 5, 10, 20]:\n",
+                "for beam_width in [1, 2, 5, 10, 20]:\n",
                 "    retrieve_subgraph_path = os.path.join(retrieve_subgraph_dir, f'e5-b{beam_width}.jsonl')\n",
                 "    !srtk retrieve --input $formatted_test_path \\\n",
                 "        --output $retrieve_subgraph_path \\\n",
                 "        --sparql-endpoint http://localhost:3001/sparql \\\n",
                 "        --knowledge-graph freebase \\\n",
                 "        --scorer-model-path $webqsp_model_dir \\\n",
                 "        --beam-width $beam_width \\\n",
                 "        --max-depth 2 \\\n",
                 "        --evaluate"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 7,
+            "execution_count": 17,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "[0.8343868521000001, 0.8609355247, 0.9121365360000001, 0.9348925411000001]\n",
-                        "[62.09924146649811, 66.23451327433628, 150.12010113780025, 298.5575221238938]\n"
+                        "[0.5619469027, 0.8343868521000001, 0.8609355247, 0.9121365360000001, 0.9348925411000001]\n",
+                        "[11.38621997471555, 62.09924146649811, 66.23451327433628, 150.12010113780025, 298.5575221238938]\n"
                     ]
                 }
             ],
             "source": [
                 "wikidata_sq_subgraph_path_pattern = 'artifacts/subgraphs/webqsp/e5-b{beam}.jsonl'\n",
                 "metric_path_pattern = 'artifacts/subgraphs/webqsp/e5-b{beam}.metric'\n",
                 "subgraph_means = []\n",
                 "recalls = []\n",
-                "for beam in [2, 5, 10, 20]:\n",
+                "for beam in [1, 2, 5, 10, 20]:\n",
                 "    subgraph_path = wikidata_sq_subgraph_path_pattern.format(beam=beam)\n",
                 "    metric_path = metric_path_pattern.format(beam=beam)\n",
                 "    subgraphs = srsly.read_jsonl(subgraph_path)\n",
                 "    metric = srsly.read_json(metric_path)\n",
                 "    avg_n_triplets = statistics.mean([len(sg['triplets']) for sg in subgraphs])\n",
                 "    recalls.append(metric['recall'])\n",
                 "    subgraph_means.append(avg_n_triplets)\n",
```

### Comparing `srtk-0.0.2/sample_commands.ipynb` & `srtk-0.0.3/sample_commands.ipynb`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9945963541666667%*

 * *Differences: {"'cells'": "{1: {'outputs': {0: {'text': ['Entity linking data/samples/question.jsonl: 100%|█| "*

 * *            "1/1 [00:00<00:00,  1.52it/s]\\n', 'Entity linking result saved to "*

 * *            "data/samples/linked-oop.jsonl\\n']}}, 'source': {insert: [(0, '!srtk link --input "*

 * *            "data/samples/question.jsonl \\\\\\n'), (1, '    --knowledge-graph wikidata \\\\\\n'), "*

 * *            "(2, '    --output data/samples/linked-oop.jsonl \\\\\\n')], delete: [1, 0]}}, 3: "*

 * *            "{'execution_count': 5, 'ou […]*

```diff
@@ -13,23 +13,23 @@
             "execution_count": 2,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Entity linking data/samples/question.jsonl: 100%|\u2588| 1/1 [00:00<00:00,  1.69it/s]\n",
-                        "0 / 1 grounded entities not converted to Wikidata qids\n",
-                        "Entity linking result saved to data/samples/linked.jsonl\n"
+                        "Entity linking data/samples/question.jsonl: 100%|\u2588| 1/1 [00:00<00:00,  1.52it/s]\n",
+                        "Entity linking result saved to data/samples/linked-oop.jsonl\n"
                     ]
                 }
             ],
             "source": [
-                "!srtk link-wikidata --input data/samples/question.jsonl \\\n",
-                "    --output data/samples/linked.jsonl \\\n",
+                "!srtk link --input data/samples/question.jsonl \\\n",
+                "    --knowledge-graph wikidata \\\n",
+                "    --output data/samples/linked-oop.jsonl \\\n",
                 "    --ground-on question \\\n",
                 "    --el-endpoint http://127.0.0.1:1235 \\\n",
                 "    --wikimapper-db resources/wikimapper/index_enwiki.db"
             ]
         },
         {
             "attachments": {},
@@ -37,46 +37,46 @@
             "metadata": {},
             "source": [
                 "retrieve"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 20,
+            "execution_count": 5,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Retrieving subgraphs: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:03<00:00,  3.56s/it]\n",
+                        "Retrieving subgraphs: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:05<00:00,  5.03s/it]\n",
                         "Retrieved subgraphs saved to to data/samples/subgraph.jsonl\n"
                     ]
                 }
             ],
             "source": [
                 "!srtk retrieve --input data/samples/linked.jsonl \\\n",
                 "\t\t--output data/samples/subgraph.jsonl \\\n",
                 "\t\t--sparql-endpoint http://localhost:1234/api/endpoint/sparql \\\n",
                 "\t\t--knowledge-graph wikidata \\\n",
-                "\t\t--scorer-model-path artifacts/models/wd_simple_e10 \\\n",
-                "\t\t--beam-width 3 \\\n",
+                "\t\t--scorer-model-path drt/wikidata-simplequestions \\\n",
+                "\t\t--beam-width 2 \\\n",
                 "\t\t--max-depth 1"
             ]
         },
         {
             "cell_type": "code",
-            "execution_count": 19,
+            "execution_count": 6,
             "metadata": {},
             "outputs": [
                 {
                     "name": "stdout",
                     "output_type": "stream",
                     "text": [
-                        "Visualizing graphs: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:00<00:00, 21.80it/s]\n",
+                        "Visualizing graphs: 100%|\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588\u2588| 1/1 [00:00<00:00, 25.88it/s]\n",
                         "Visualized graphs outputted to data/samples.\n"
                     ]
                 }
             ],
             "source": [
                 "!srtk visualize --input data/samples/subgraph.jsonl \\\n",
                 "    --output-dir data/samples \\\n",
```

### Comparing `srtk-0.0.2/test.pdf` & `srtk-0.0.3/test.pdf`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/train_qald.ipynb` & `srtk-0.0.3/train_qald.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/train_wd_simple.ipynb` & `srtk-0.0.3/train_wd_simple.ipynb`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998387096774194%*

 * *Differences: {"'cells'": "{23: {'source': {insert: [(1, '    -v "*

 * *            "data/wikidata-simplequestions/dataset/test.jsonl \\\\\\n'), (7, '    --max-epochs "*

 * *            "10')], delete: [7, 1]}}}"}*

```diff
@@ -437,21 +437,21 @@
                         "\u001b[34m\u001b[1mwandb\u001b[0m: Synced 6 W&B file(s), 0 media file(s), 0 artifact file(s) and 0 other file(s)\n",
                         "\u001b[34m\u001b[1mwandb\u001b[0m: Find logs at: \u001b[35m\u001b[1martifacts/wandb/run-20230428_233419-vtg7f3h7/logs\u001b[0m\n"
                     ]
                 }
             ],
             "source": [
                 "!CUDA_VISIBLE_DEVICES=3 srtk train -t data/wikidata-simplequestions/dataset/train.jsonl \\\n",
-                "    -v data/wikidata-simplequestions/dataset/valid.jsonl \\\n",
+                "    -v data/wikidata-simplequestions/dataset/test.jsonl \\\n",
                 "    --model-name-or-path roberta-base \\\n",
                 "    --output-dir artifacts/models/wd_simple_e10 \\\n",
                 "    --accelerator gpu \\\n",
                 "    --learning-rate 1e-5 \\\n",
                 "    --batch-size 96 \\\n",
-                "    --max-epochs 20"
+                "    --max-epochs 10"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
             "source": [
```

### Comparing `srtk-0.0.2/.github/workflows/pytest.yml` & `srtk-0.0.3/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/cli.py` & `srtk-0.0.3/src/srtk/cli.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/link.py` & `srtk-0.0.3/src/srtk/link.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,82 +1,49 @@
 """Entity linking
 This step links the entity mentions in the question to the entities in the Wikidata knowledge graph.
 It inference on the REL endpoint.
 """
 import argparse
-import requests
-import socket
 from pathlib import Path
 
 import srsly
 from tqdm import tqdm
 
-from wikimapper import WikiMapper
-
-
-def socket_reachable(host, port):
-    """
-    Check if a socket is reachable
-    """
-    try:
-        s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        s.settimeout(2) # set a timeout value for the socket
-        s.connect((host, port))
-        s.close()
-        return True
-    except Exception as err:
-        print(err)
-        return False
+from .entity_linking import WikidataLinker, DBpediaLinker
+from .utils import socket_reachable
 
 
 def link(args):
-    try:
-        host = args.el_endpoint.split(':')[-2].split('/')[-1]
-        port = int(args.el_endpoint.split(':')[-1])
-    except Exception as exc:
-        raise ValueError(f"Can't parse the endpoint {args.el_endpoint}") from exc
-    if not socket_reachable(host, port):
+    """Link the entities in the questions to the Wikidata knowledge graph"""
+    if not socket_reachable(args.el_endpoint):
         raise RuntimeError(f"Can't reach the endpoint {args.el_endpoint}")
-    mapper = WikiMapper(args.wikimapper_db)
 
-    with open(args.input, "r", encoding="utf-8") as f:
+    if args.knowledge_graph == 'wikidata':
+        linker = WikidataLinker(args.el_endpoint, args.wikimapper_db)
+    elif args.knowledge_graph == 'dbpedia':
+        linker = DBpediaLinker(args.el_endpoint)
+    else:
+        raise NotImplementedError(f"Knowledge graph {args.knowledge_graph} not implemented")
+
+    with open(args.input, 'r', encoding='utf-8') as f:
         total_lines = len(f.readlines())
     questions = srsly.read_jsonl(args.input)
-    cnt_qid_not_found = 0
-    cnt_total_ground = 0
+    cnt_id_not_found = 0
+    cnt_id_found = 0
     all_linked = []
     for question in tqdm(questions, total=total_lines, desc=f"Entity linking {args.input}"):
-        document = {
-            'text': question[args.ground_on],
-        }
-        api_results = requests.post(args.el_endpoint, json=document, timeout=60).json()
-        cnt_total_ground += len(api_results)
-        qids = []
-        spans = []
-        entities = []
-        for result in api_results:
-            start_pos, mention_length, mention, entity, disambiguation_cofidence, mention_detection_confidence, tag = result
-            qid = mapper.title_to_id(entity)
-            span = (start_pos, start_pos + mention_length)
-            if qid is None:
-                cnt_qid_not_found += 1
-            else:
-                qids.append(qid)
-                entities.append(entity)
-                spans.append(span)
-        linked = {
-            "question": question[args.ground_on],
-            "question_entities": qids,
-            "spans": spans,
-            "entity_names": entities
-        }
-        if "id" in question:
-            linked["id"] = question["id"]
+        linked = linker.annotate(question[args.ground_on])
+        cnt_id_found += len(linked["question_entities"])
+        if 'not_converted_entities' in linked:
+            cnt_id_not_found += len(linked['not_converted_entities'])
+        if 'id' in question:
+            linked['id'] = question['id']
         all_linked.append(linked)
-    print(f"{cnt_qid_not_found} / {cnt_total_ground} grounded entities not converted to Wikidata qids")
+    if cnt_id_not_found > 0:
+        print(f"{cnt_id_not_found} / {cnt_id_found + cnt_id_not_found} grounded entities not converted to ids")
     # check whether the folder exists
     folder_path = Path(args.output).parent
     if not folder_path.exists():
         folder_path.mkdir(parents=True)
         print(f"Folder {folder_path} created")
     Path(args.output).parent.mkdir(parents=True, exist_ok=True)
     srsly.write_jsonl(args.output, all_linked)
@@ -87,19 +54,20 @@
     """Add entity linking arguments to the parser"""
     parser.description = '''Entity linking on Wikidata.
     The input is a jsonl file. The field of interest is specified by the argument --ground-on.
     The output is a jsonl file, each line is a dict with keys: id, question_entities, spans, entity_names.
     '''
     parser.add_argument('-i', '--input', type=str, help='Input file path, in which the question is stored')
     parser.add_argument('-o', '--output', type=str, help='Output file path, in which the entity linking result is stored')
-    parser.add_argument('-e', '--el-endpoint', type=str, default='http://127.0.0.1:1235', help='REL endpoint')
-    parser.add_argument('-kg', '--knowledge-graph', type=str, default='wikidata', choices=['wikidata'],
+    parser.add_argument('-e', '--el-endpoint', type=str, default='http://127.0.0.1:1235', help='Entity linking endpoint \
+                        (default: http://127.0.0.1:1235 <local REL endpoint>)')
+    parser.add_argument('-kg', '--knowledge-graph', type=str, default='wikidata', choices=['wikidata', 'dbpedia'],
                         help='Knowledge graph to link to, only wikidata is supported now')
     parser.add_argument('--wikimapper-db', type=str, default='resources/wikimapper/index_enwiki.db', help='Wikimapper database path')
     parser.add_argument('--ground-on', type=str, default='question', help='The key to ground on, the corresponding text will be sent to the REL endpoint for entity linking')
-    
+
 
 if __name__ == '__main__':
     parser = argparse.ArgumentParser()
     add_arguments(parser)
     args = parser.parse_args()
     link(args)
```

### Comparing `srtk-0.0.2/src/srtk/preprocess.py` & `srtk-0.0.3/src/srtk/preprocess.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/retrieve.py` & `srtk-0.0.3/src/srtk/retrieve.py`

 * *Files 9% similar despite different names*

```diff
@@ -39,19 +39,19 @@
         self.kg = kg
 
     def retrive_subgraph(self, entity, path):
         '''Retrive subgraph entities and triplets by traversing from an entity following
         a relation path hop by hop.
 
         Args:
-            entity: the source node
-            path: a list of relations
+            entity (str): the identifier of the source node
+            path (list[str]): a list of relation identifiers
 
         Returns:
-            entities: a list of entities
+            entities: a list of entity identifiers
             triplets: a list of triplets
         '''
         entities, triplets = set(), set()
         tracked_entities = set((entity,))
         for relation in path:
             next_hops = set()
             if relation == END_REL:
@@ -64,46 +64,69 @@
             tracked_entities = next_hops
         return list(entities), list(triplets)
 
     def deduce_leaves(self, entity, path):
         """Deduce leaves from an entity following a path hop by hop.
 
         Args:
-            entity: the source node
-            path: a list of relations
+            entity (str): the identifier of the source node
+            path (list[str]): a list of relation identifiers
 
         Returns:
-            leaves: a list of leaves that are n-hop away from the source node,
+            set[str]: a set of leave identifiers that are n-hop away from the source node,
                 where n is the length of the path
         """
         leaves = set((entity,))
         for relation in path:
             if relation == END_REL:
                 continue
             leaves = set().union(*(self.kg.deduce_leaves(leaf, (relation,)) for leaf in leaves))
         return leaves
 
     def deduce_leaf_relations(self, entity, path):
         """Deduce leaf relations from an entity following a path hop by hop.
 
         Args:
-            entity: the source node
-            path: a list of relations
+            entity (str): the identifier of the source node
+            path (list[str]): a list of relation identifiers
 
         Returns:
-            relations: a list of relations that are n-hop away from the source node,
+            tuple[str]: a tuple of relations that are n-hop away from the source node,
                 where n is the length of the path
         """
         leaves = self.deduce_leaves(entity, path)
         relations = set().union(*(self.kg.get_neighbor_relations(leaf) for leaf in leaves))
         # Special filter relation for freebase
         if self.kg.name == 'freebase':
             relations = [r for r in relations if r.split('.')[0] not in ['kg', 'common']]
         return tuple(relations)
 
+    def get_relation_label(self, identifier):
+        """Get the relation label of an entity or a relation.
+
+        It serves as a proxy to the knowledge graph's get_label function. For freebase,
+        we directly use the identifier as the label. For others, we return the retrieved
+        label if it exists, otherwise return the identifier.
+
+        Args:
+            identifier (str): the identifier of an entity or a relation
+
+        Returns:
+            str: the label of the entity or the relation
+        """
+        # For freebase, the relation identifier contains enough information
+        if self.kg.name == 'freebase':
+            return identifier
+        if identifier == END_REL:
+            return END_REL
+        label =  self.kg.get_label(identifier)
+        if label is None:
+            return identifier
+        return label
+
 
 class Retriever:
     '''Retriever retrieves subgraphs from a knowledge graph with a question and its
     linked entities. The retrieval process takes the semantic information of the question
     and the expanding path into consideration.
     '''
     def __init__(self, kg: KnowledgeGraphBase, scorer: Scorer, beam_width: int, max_depth: int):
@@ -113,20 +136,20 @@
         self.max_depth = max_depth
         self.num_entity_threshold = 1000
 
     def retrieve_subgraph_triplets(self, sample: Dict[str, Any]):
         """Retrieve triplets as subgraphs from paths.
 
         Args:
-            sample: a sample from the dataset, which contains at least the following fields:
+            sample (dict): a sample from the dataset, which contains at least the following fields:
                 question: a string
                 question_entities: a list of entities
 
         Returns:
-            triplets: a list of triplets
+            list(tuple): a list of triplets
         """
         question = sample['question']
         triplets = []
         for question_entity in sample['question_entities']:
             path_score_list = self.beam_search_path(question, question_entity)
             n_nodes = 0
             for relations, _ in path_score_list:
@@ -143,19 +166,19 @@
 
     def beam_search_path(self, question: str, question_entity: str):
         '''This function reimplement RUC's paper's solution. In the search process, only the history
         paths are recorded; each new relation is looked up via looking up the end relations from the
         question entities following a history path.
 
         Args:
-            question (str)
+            question (str): a natural language question
             question_entity (str): a grounded question entity
 
         Returns:
-            path_score_list (list[Path]): a list of (path, score) tuples
+            list[Path]: path score list, a list of (path, score) tuples
         '''
         candidate_paths = [Path()]  # path and its score
         result_paths = []
         depth = 0
 
         while candidate_paths and len(result_paths) < self.beam_width and depth < self.max_depth:
             next_relations_batched = []
@@ -186,33 +209,43 @@
 
         Args:
             question (str)
             paths (list[Path]): a list of current paths
             relations_batched (list[list[str]]): a list of next relations for each path
 
         Returns:
-            scored_paths (list[Path]): a list of newly expanded and scored paths
+            list[Path]: scored_paths, a list of newly expanded and scored paths
         '''
         scored_paths = []
         score_matrix = []
         for path, next_relations in zip(paths, relations_batched):
-            scores = self.scorer.batch_score(question, tuple(path.prev_relations), tuple(next_relations))
+            prev_relation_labels = tuple(self.kgh.get_relation_label(r) for r in path.prev_relations)
+            next_relation_labels = tuple(self.kgh.get_relation_label(r) for r in next_relations)
+            scores = self.scorer.batch_score(question, prev_relation_labels, next_relation_labels)
             score_matrix.append(scores)
 
         for i, (path, next_relations) in enumerate(zip(paths, relations_batched)):
             for j, relation in enumerate(next_relations):
                 new_prev_relations = path.prev_relations + (relation,)
                 score = float(score_matrix[i][j]) + path.score
                 scored_paths.append(Path(new_prev_relations, score))
         return scored_paths
 
 
 def calculate_hit_and_miss(retrieved_path):
     """Calculate the recall of answer entities in retrieved triplets,
     if answer_entities exists in each sample.
+    
+    Args:
+        retrieved_path (str): path to the retrieved triplets
+    
+    Returns:
+        tuple(int, int): number of samples that have at least one answer entity in retrieved triplets,
+            and number of samples that have no answer entity in retrieved triplets
+        
     """
     retrieval = srsly.read_jsonl(retrieved_path)
     hit = 0
     miss = 0
     for sample in retrieval:
         if 'answer_entities' not in sample:
             continue
```

### Comparing `srtk-0.0.2/src/srtk/train.py` & `srtk-0.0.3/src/srtk/train.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/visualize.py` & `srtk-0.0.3/src/srtk/visualize.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/knowledge_graph/freebase.py` & `srtk-0.0.3/src/srtk/knowledge_graph/freebase.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/knowledge_graph/graph_base.py` & `srtk-0.0.3/src/srtk/knowledge_graph/graph_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         Returns:
             list[str]: list of leaves. Each leaf is a QID.
         """
         raise NotImplementedError
 
     @abstractmethod
     def get_neighbor_relations(self, src: str, hop: int, limit: int) -> List[str]:
-        """Get relations between src and dst.
+        """Get n-hop neighbor relations of src.
 
         Args:
             src (str): source entity
             hop (int, optional): hop of the relations. Defaults to 1.
             limit (int, optional): limit of the number of relations.
 
         Returns:
```

### Comparing `srtk-0.0.2/src/srtk/knowledge_graph/wikidata.py` & `srtk-0.0.3/src/srtk/knowledge_graph/wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/preprocessing/load_dataset.py` & `srtk-0.0.3/src/srtk/preprocessing/load_dataset.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/preprocessing/merge_ground.py` & `srtk-0.0.3/src/srtk/preprocessing/merge_ground.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/preprocessing/negative_sampling.py` & `srtk-0.0.3/src/srtk/preprocessing/negative_sampling.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/preprocessing/score_path.py` & `srtk-0.0.3/src/srtk/preprocessing/score_path.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/preprocessing/search_path.py` & `srtk-0.0.3/src/srtk/preprocessing/search_path.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/src/srtk/scorer/scorer.py` & `srtk-0.0.3/src/srtk/scorer/scorer.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,17 +6,21 @@
 from .encoder import LitSentenceEncoder
 
 
 class Scorer:
     """Scorer for relation paths."""
 
     def __init__(self, pretrained_name_or_path, device=None):
-        self.model = LitSentenceEncoder(pretrained_name_or_path)
-        config = self.model.config
-        self.tokenizer = AutoTokenizer.from_pretrained(config._name_or_path)
+        self.tokenizer = AutoTokenizer.from_pretrained(pretrained_name_or_path)
+        # Set pooling method to average if the model does not have a CLS token.
+        if self.tokenizer.cls_token is None:
+            pool_method = 'avg'
+        else:
+            pool_method = 'cls'
+        self.model = LitSentenceEncoder(pretrained_name_or_path, pool=pool_method)
         if device:
             self.model = self.model.to(device)
 
     @lru_cache
     def score(self, question, prev_relations, next_relation):
         """Score a relation path.
```

### Comparing `srtk-0.0.2/tests/test_encoder.py` & `srtk-0.0.3/tests/test_encoder.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,32 +5,38 @@
 
 
 @pytest.fixture
 def model():
     return LitSentenceEncoder('smallbenchnlp/roberta-small')
 
 
-def test_pooler(model):
-    if hasattr(model, 'average_pool'):
-        pooler = model.average_pool
-    elif hasattr(model, 'cls_pool'):
-        pooler = model.cls_pool
-    else:
-        pytest.skip('No pooler found')
+def examine_single_pooler(pooler):
     # Test pooler without batch size
     hidden_states = torch.randn(10, 256)
     attention_mask = torch.ones(10)
     pooled = pooler(hidden_states, attention_mask)
     assert pooled.shape == (256,)
     # Test pooler with batch size
     hidden_states = torch.randn(2, 10, 256)
     attention_mask = torch.ones(2, 10)
     pooled = pooler(hidden_states, attention_mask)
     assert pooled.shape == (2, 256)
 
+def test_avg_pooler(model):
+    if hasattr(model, 'avg_pool'):
+        examine_single_pooler(model.avg_pool)
+    else:
+        pytest.skip('No avg pooler found')
+
+def test_cls_pooler(model):
+    if hasattr(model, 'cls_pool'):
+        examine_single_pooler(model.cls_pool)
+    else:
+        pytest.skip('No cls pooler found')
+
 def test_compute_sentence_similarity(model):
     # Test batched similarity
     query = torch.randn(2, 1, 10, 256)
     samples = torch.randn(2, 3, 10, 256)
     similarity = model.compute_sentence_similarity(query, samples)
     assert similarity.shape == (2, 3)
     # Test single pair similarity
```

### Comparing `srtk-0.0.2/tests/test_freebase.py` & `srtk-0.0.3/tests/test_freebase.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/tests/test_scorer.py` & `srtk-0.0.3/tests/test_scorer.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/tests/test_wikidata.py` & `srtk-0.0.3/tests/test_wikidata.py`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/tutorials/1.get_started.ipynb` & `srtk-0.0.3/tutorials/1.get_started.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/tutorials/2.end_to_end_subgraph_retrieval.ipynb` & `srtk-0.0.3/tutorials/2.end_to_end_subgraph_retrieval.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/tutorials/3.weak_train_wikidata.ipynb` & `srtk-0.0.3/tutorials/3.weak_train_wikidata.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/tutorials/4.weak_train_freebase.ipynb` & `srtk-0.0.3/tutorials/4.weak_train_freebase.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/tutorials/5.supervised_train_wikidata.ipynb` & `srtk-0.0.3/tutorials/5.supervised_train_wikidata.ipynb`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/.gitignore` & `srtk-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/LICENSE` & `srtk-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/README.md` & `srtk-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `srtk-0.0.2/pyproject.toml` & `srtk-0.0.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt"]
 build-backend = "hatchling.build"
 
 [project]
 name = "srtk"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Yuanchun Shen", email="y.c.shen@tum.de" },
 ]
 description = "A toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `srtk-0.0.2/PKG-INFO` & `srtk-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: srtk
-Version: 0.0.2
+Version: 0.0.3
 Summary: A toolkit for semantic-relevant subgraph retrieval from large-scale knowledge graphs.
 Project-URL: Homepage, https://github.com/happen2me/subgraph-retrieval-toolkit
 Project-URL: Bug Tracker, https://github.com/happen2me/subgraph-retrieval-toolkit/issues
 Author-email: Yuanchun Shen <y.c.shen@tum.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

